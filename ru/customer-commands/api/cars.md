# Получение списка автомобилей

Обратите внимание, что для неавторизованных сеансов возвращается сокращённая версия данных об автомобилях.

## Запрос

    GET /api/cars HTTP/1.1
    Cookie: sessid=xC9tq10dbYt0X1zeROheVFUHxA6aVjWM299hOHCaUHg72cPWUgZHYFLss26p6iH3
    Accept-Language: en-US
    Host: 192.168.1.35:4000
    Connection: Keep-Alive
    Accept-Encoding: gzip
    User-Agent: okhttp/2.7.0

## Ответ

```json
{
  "cars": [
    {
      "Id": "29686ea2-a698-45eb-97df-a776016d4e44",
      "Color": "Синий",
      "RegNumber": "АК4321ВВ",
      "Cdi": "7703222222",
      "Lat": 55.5196075,
      "Lon": 37.35072,
      "FuelLevel": null,
      "FuelDistance": null,
      "ModelId": "74566814-0ecb-4dd8-b9cd-a70d011c8be5",
      "ModelImageId": "e5f038bd-8cfa-46a2-af5c-a70d014caa88",
      "Brand": "Hyundai",
      "Model": "Solaris",
      "TransmissionType": 2,
      "Discount": 0
    }
  ]
}
```