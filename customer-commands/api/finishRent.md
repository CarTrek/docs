# Завершить аренду / отменить бронь

Завершает текущую аренду.

## Запрос

    POST /api/finishRent/ HTTP/1.1
    Cookie: sessid=xC9tq10dbYt0X1zeROheVFUHxA6aVjWM299hOHCaUHg72cPWUgZHYFLss26p6iH3
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
  "result": "OkOrderFinished",
  "response": {
    "rideReport": {
      "parkTotalInKops": 0,
      "parkMinutes": 0,
      "driveTotalInKops": 0,
      "driveMinutes": 0,
      "totalInKops": 0,
      "totalToPay": 0,
      "bonusesUsedInKops": 0,
      "freeBookMinutes": 0,
      "totalRun": 0,
      "runIncluded": 90,
      "overrunRate": 0,
      "overrun": 0,
      "overrunCost": 0
    },
    "userMessage": "Заказ успешно завершён.",
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
    "order": null,
    "carTicket": null,
    "promoCode": "PROMO",
    "notifications": [],
    "accessLevel": "Operator"
  },
  "rideReport": {
    "parkTotalInKops": 0,
    "parkMinutes": 0,
    "driveTotalInKops": 0,
    "driveMinutes": 0,
    "totalInKops": 0,
    "totalToPay": 0,
    "bonusesUsedInKops": 0,
    "freeBookMinutes": 0,
    "totalRun": 0,
    "runIncluded": 90,
    "overrunRate": 0,
    "overrun": 0,
    "overrunCost": 0
  }
}
```