# Получить список доступных тарифов и абонементов

Возвращает список доступных авторизованному пользователю тарифов для забронированного автомобиля.

## Запрос

    GET /api/rates HTTP/1.1
    Cookie: sessid=xC9tq10dbYt0X1zeROheVFUHxA6aVjWM299hOHCaUHg72cPWUgZHYFLss26p6iH3
    Accept-Language: en-US
    Host: 192.168.1.35:4000
    Connection: Keep-Alive
    Accept-Encoding: gzip
    User-Agent: okhttp/2.7.0

## Ответ

```json
{
  "perMinuteRates": [
    {
      "id": "34c82ef5-a27c-4b8a-9efd-a85a00d9e456",
      "name": "Поминутный тариф",
      "parkRate": 50,
      "driveRate": 600,
      "fromHour": 21,
      "toHour": 20,
      "runIncluded": 90,
      "overrunCostPerKm": 700
    }
  ],
  "ratePacks": [
    {
      "id": "66d1bb57-4731-4a78-9bab-a852008138f8",
      "name": "Суточный тариф",
      "costInKops": 200000,
      "minutesIncluded": 1439,
      "runIncluded": 150,
      "overrunCostPerKm": 700
    }
  ]
}
```