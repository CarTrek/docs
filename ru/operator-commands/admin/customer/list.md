# Получение списка клиентов

## Запрос

    GET /admin/customer/list/?mode=ALL&page=0&count=50&sort=CreationDate&dir=desc&search=sas&fromDate=2017-01-15T21:00:00.000Z&toDate=2017-01-17T21:00:00.000Z HTTP/1.1
    Connection: keep-alive
    Pragma: no-cache
    Cache-Control: no-cache
    Accept: application/json, text/plain, */*
    User-Agent: Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36
    Accept-Encoding: gzip, deflate, br
    Accept-Language: ru-RU,ru;q=0.9,en-US;q=0.8,en;q=0.7,de;q=0.6,sq;q=0.5
    Cookie: sessid=2cJxqqs1Wrx9b6XiOhQwq5seianHfZKpOB3oX4A;

## Ответ

```json
{
  "rows": [
    {
      "Id": "f65db756-ed50-4269-869d-a6fe0153cc08",
      "DisplayName": "Слободчиков Александр Сергеевич",
      "Name": "Александр",
      "Surname": "Слободчиков",
      "Patronymic": "Сергеевич",
      "Email": "sas@cartrek.online",
      "CustomersBalance": 4500,
      "Comment": "test 1111",
      "FullComment": "test 1111",
      "Phone": "+79050000000",
      "IsApproved": true,
      "IsBlocked": false,
      "IsAdmin": true,
      "IsFree": true,
      "CreationDate": "17.01.2017 23:37:09",
      "Run24Hours": 13,
      "ReferalsCount": 0,
      "OwnPromoCode": "XJBOY0",
      "FriendsPromoCode": null,
      "Car": {
        "Id": "29686ea2-a698-45eb-97df-a776016d4e44",
        "Brand": "Hyundai",
        "Model": "Solaris",
        "RegNumber": "АК4321ВВ"
      },
      "Tags": [
        {
          "Id": "3d6646d6-61ec-483c-8214-a749017528cf",
          "Name": "Разработчик",
          "Color": "#F44336",
          "Comment": null
        }
      ],
      "UnderSupervision": true,
      "SumNSubStatus": 0,
      "CanRescheduleSumNSubCheck": false,
      "CanStartSumNSubCheck": false
    }
  ],
  "numberOfPages": 1
}
```