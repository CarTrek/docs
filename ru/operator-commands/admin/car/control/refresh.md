# Получить состояние автомобиля

## Запрос

    POST /admin/car/control/refresh/b34fbcda-6311-456c-80c2-a7e601131165 HTTP/1.1
    Host: test.cartrek.online
    Connection: keep-alive
    Content-Length: 0
    Pragma: no-cache
    Cache-Control: no-cache
    Accept: application/json, text/plain, */*
    User-Agent: Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36
    Accept-Encoding: gzip, deflate, br
    Accept-Language: ru-RU,ru;q=0.9,en-US;q=0.8,en;q=0.7,de;q=0.6,sq;q=0.5
    Cookie: sessid=2cJxqqs1oX4ALBqXKCQkaysjAoDJ7toPQCkV8

## Ответ

```json
{
  "carState": {
    "isOnline": true,
    "isLocked": true,
    "carProfile": 1,
    "fuelLevel": 32,
    "speed": 0,
    "engineSpeed": -1,
    "alt": 165,
    "gsmLevel": 46,
    "gsmChannel": 1,
    "visibleSatellitesNum": 19,
    "isCoordinatesValid": true,
    "mileage": 3197.236,
    "mileageCAN": null,
    "isEngineStarted": false,
    "isIgnitionOn": false,
    "uptime": "1д. 12:56:23",
    "lightsOn": false,
    "handBrakeOn": true,
    "immoOn": true,
    "voltage": 13.018,
    "rezervVoltage": 4.154
  },
  "rentState": {
    "orderStage": 2,
    "customerId": "f223e480-c356-4f82-8342-a8530017b75a",
    "customerName": "Иван Михайлович Сидоров",
    "orderStartDateTime": "2017-12-24T16:05:39.0000000+03:00",
    "orderStartDateTimeString": "24.12.2017 16:05:39",
    "customerPhoneNumber": "+79250000000",
    "orderTotalMinutes": 36513
  }
}

```