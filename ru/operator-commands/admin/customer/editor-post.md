# Изменение конфигурации клиента

## Запрос

    POST /admin/customer/editor/f65db756-ed50-4269-869d-a6fe0153cc08 HTTP/1.1
    Host: test.cartrek.online
    Connection: keep-alive
    Content-Length: 3881
    Pragma: no-cache
    Cache-Control: no-cache
    Accept: application/json, text/plain, */*
    User-Agent: Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36
    Content-Type: application/json;charset=UTF-8
    Accept-Encoding: gzip, deflate, br
    Accept-Language: ru-RU,ru;q=0.9,en-US;q=0.8,en;q=0.7,de;q=0.6,sq;q=0.5
    Cookie: sessid=2cJxqqs1Wrx9b6XiOhQwq5seianHfZKpOB3kV8;

```json
{
  "allowFreeRide": true,
  "surname": "Слободчиков",
  "name": "Александр",
  "patronymic": "Сергеевич",
  "email": "sas@example.com",
  "phone": "+79050000000",
  "comment": "test 1111",
  "password": null,
  "isApproved": true,
  "isBlocked": false,
  "birthDate": "",
  "passportDate": "",
  "passportIssued": null,
  "passportNumber": null,
  "homeAddress": null,
  "driverSince": "",
  "driversLicenceDate": "",
  "driversLicenceNumber": null,
  "result": "ok",
  "id": "f65db756-ed50-4269-869d-a6fe0153cc08",
  "isAdmin": true,
  "isFree": true,
  "underSupervision": true,
  "tags": [
    {
      "Id": "3d6646d6-61ec-483c-8214-a749017528cf",
    }
  ],
  "ownPromoCode": "XJBOY0",
  "Organizations": [
    {
      "Id": "d0806288-b74b-4363-aa4c-a70300f285e6",
    }
  ]
}
```

## Ответ

```json
{
    "result": "ok"
}
```