# Получение данных клиента

## Запрос

    GET /admin/customer/editor/f65db756-ed50-4269-869d-a6fe0153cc08 HTTP/1.1
    Connection: keep-alive
    Pragma: no-cache
    Cache-Control: no-cache
    Accept: application/json, text/plain, */*
    User-Agent: Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36
    Accept-Encoding: gzip, deflate, br
    Accept-Language: ru-RU,ru;q=0.9,en-US;q=0.8,en;q=0.7,de;q=0.6,sq;q=0.5
    Cookie: sessid=2cJxqqs1Wrx9b6XiOhQwq5seiaZKpOB3oX4kV8;

## Ответ

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
  "commonCustomer": null,
  "organizations": null,
  "imageScanSrc1": "/admin/customer/documents/Image/cb07b1c2-838c-4be2-ba34-a6fe0153cbcb",
  "imageScanSrc2": "/admin/customer/documents/Image/77a501e7-0202-4458-8416-a6fe0153cbde",
  "imageScanSrc3": "/admin/customer/documents/Image/04d90429-874f-49c7-8f8c-a6fe0153cbec",
  "imageScanSrc4": "/admin/customer/documents/Image/3f98afff-7d48-4e66-b2a4-a6fe0153cbf5",
  "imageScanSrc5": "/admin/customer/documents/Image/71005639-02d8-41d9-9355-a6fe0153cbff",
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
  "displayName": "Слободчиков Александр Сергеевич",
  "customersBalance": 4500,
  "isAdmin": true,
  "isFree": true,
  "underSupervision": true,
  "bankCards": null,
  "tags": [
    {
      "id": "3d6646d6-61ec-483c-8214-a749017528cf"
    }
  ],
  "youtellClientId": "ba6ffb26-7b15-476b-9dc8-a75200be72f4",
  "comments": [],
  "rating": null,
  "ownPromoCode": "XJBOY0"
}
```