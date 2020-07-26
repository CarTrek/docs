# Получение списка заказов

## Запрос

    GET /admin/order/list/?carId=undefined&userId=undefined&mode=active&page=0&count=50&search=sas HTTP/1.1
    Connection: keep-alive
    Pragma: no-cache
    Cache-Control: no-cache
    Accept: application/json, text/plain, */*
    User-Agent: Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36
    Accept-Encoding: gzip, deflate, br
    Accept-Language: ru-RU,ru;q=0.9,en-US;q=0.8,en;q=0.7,de;q=0.6,sq;q=0.5
    Cookie: sessid=2cJxqqs1Wrx9ZKpOB3oX4ALBqXKCQkaysjAoDJ7toPQCkV8;

## Ответ

```json
{
  "rows": [
    {
      "BookDateTime": "18.01.2018 23:31:57",
      "CarId": "29686ea2-a698-45eb-97df-a776016d4e44",
      "CarRegNumber": "АК4321ВВ",
      "Customer": "Слободчиков Александр Сергеевич",
      "CustomerId": "f65db756-ed50-4269-869d-a6fe0153cc08",
      "CustomerUnderSupervision": true,
      "DriveMinutes": 933,
      "EndDateTime": "Ещё не завершён",
      "FreeBookMinutes": 1,
      "Id": "08b178e3-a105-4b9e-93b2-a86c01525e67",
      "OrderStage": "Использование",
      "ParkMinutes": 0,
      "TotalCost": "109,37",
      "TotalRun": 30
    }
  ],
  "numberOfPages": 1
}
```