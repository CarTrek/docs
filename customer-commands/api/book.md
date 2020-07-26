# Бронирование автомобиля

Создаёт заказ для текущего авторизованного пользователя.

## Запрос

    POST /api/book/e9e9a3cf-d6f9-4011-9352-a712015a35c8 HTTP/1.1
    Cookie: sessid=xC9tq10dbYt0X1zeROheVFUHxA6aVjWM299hOHCaUHg72cPWUgZHYFLss26p6iH3
    Accept-Language: en-US
    Content-Type: text/plain; charset=utf-8
    Content-Length: 0
    Host: 192.168.1.35:4000
    Connection: Keep-Alive
    Accept-Encoding: gzip
    User-Agent: okhttp/2.7.0

К запросу можно добавить параметры для трекинга рекламных кампаний:

    pid={идентификатор партнера}&c={имя рекламной кампании}
    &clickid={идентификатор клика/заказа на стороне партнера}

## Ответ

```json
{
  "result": "OkCarIsBooked",
  "response": {
    "userMessage": "Машина успешно забронирована.",
    "code": 0,
    "isSuccess": true
  },
  "user": {
    "customerIsBlocked": false,
    "customersBalance": "4500.0",
    "email": "sas@cartrek.online",
    "hasBankCard": true,
    "id": "f65db756-ed50-4269-869d-a6fe0153cc08",
    "isValidatedBySecurity": true,
    "name": "Александр Сергеевич Слободчиков",
    "order": {
      "car": {
        "brand": "Hyundai",
        "color": "Синий",
        "fuelLevel": null,
        "fuelDistance": null,
        "id": "29686ea2-a698-45eb-97df-a776016d4e44",
        "lat": 55.5195045,
        "lon": 37.347847,
        "model": "Solaris",
        "modelImageId": "e5f038bd-8cfa-46a2-af5c-a70d014caa88",
        "regNumber": "АК4321ВВ",
        "bluetooth": {
          "code": null,
          "checkAcc": true,
          "checkDoors": true,
          "doorsInvertred": false
        }
      },
      "freeBookSeconds": 1200,
      "overrunCost": "0,0",
      "overrunForCurrentOrderInKm": 0,
      "overrunPriceFor1Km": "0,0",
      "rate": "0,0",
      "state": "Book",
      "stateDuration": 0,
      "totalCost": "0,0"
    },
    "carTicket": null,
    "promoCode": "XJBOY0",
    "notifications": [],
    "accessLevel": "Operator"
  }
}
```