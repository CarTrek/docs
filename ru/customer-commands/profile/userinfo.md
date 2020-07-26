# Получение состояния пользователя

В случае отсутствия в данный момент заказа у пользователя order содержит null. Варианты состояния заказа: “Book”, “Drive”, “Park”.

## Запрос

    POST /profile/userinfo HTTP/1.1
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
  "isLoggedIn": true,
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
        "lat": 55.51954,
        "lon": 37.3503342,
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
      "state": "Drive",
      "stateDuration": 809,
      "totalCost": "0,0"
    },
    "carTicket": null,
    "promoCode": "XJBOY0",
    "notifications": [],
    "accessLevel": "Operator"
  }
}
```