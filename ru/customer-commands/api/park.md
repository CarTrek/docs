# Перевести аренду в режим парковки / закрыть автомобиль

Закрывает арендованный автомобиль и переводит текущий заказ в режим парковки.

## Запрос

    POST /api/park/ HTTP/1.1
    Cookie: sessid=xC9tq10dbYt0X16aVjWM299hOHCaUHg72cPWUgZHYFLss26p6iH3
    Accept-Language: en-US
    Content-Type: text/plain; charset=utf-8
    Content-Length: 0
    Host: 192.168.1.35:4000
    Connection: Keep-Alive
    Accept-Encoding: gzip
    User-Agent: okhttp/2.7.0

## Ответ

```json
{
  "result": "OkCarIsParked",
  "response": {
    "userMessage": "Автомобиль переведён в режим парковки.",
    "code": 0,
    "isSuccess": true
  },
  "user": {
    "customerIsBlocked": false,
    "customersBalance": "0.4",
    "email": "sas@cartrek.online",
    "hasBankCard": true,
    "id": "8521b4cf-2cfa-4256-b6fb-a84500ca9b83",
    "isValidatedBySecurity": true,
    "name": "Александр Сергеевич Слободчиков",
    "order": {
      "car": {
        "brand": "Renault",
        "color": "Белый",
        "fuelLevel": 22,
        "fuelDistance": 91,
        "id": "016aec94-d06c-41ca-8ad8-a85001368a03",
        "lat": 55.7496033,
        "lon": 37.7538376,
        "model": "Logan",
        "modelImageId": "78547bea-c82d-4d17-9ebe-a848009f78f0",
        "regNumber": "А747ВТ799",
        "bluetooth": null
      },
      "freeBookSeconds": 1200,
      "overrunCost": "0,0",
      "overrunForCurrentOrderInKm": 0,
      "overrunPriceFor1Km": "0,0",
      "rate": "0,0",
      "state": "Park",
      "stateDuration": 43,
      "totalCost": "0,0"
    },
    "carTicket": null,
    "promoCode": "PROMO",
    "notifications": [],
    "accessLevel": "Operator"
  }
}
```