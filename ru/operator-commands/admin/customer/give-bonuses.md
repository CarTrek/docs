# Начисление бонусов клиенту
## Запрос

    POST /admin/billing/bonus/f65db756-ed50-4269-869d-a6fe0153cc08?amount=100&reason=refueling HTTP/1.1
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

amount - число бонусов в рублях (в этом примере 100 рбулей)
reason - произвольный текст с описанием причины начисления бонусов

Обратите внимание, что при начислении бонусов может отправляться SMS-уведомелние клиенту.

## Ответ

В ответе - страница списка всех начилений бонусов клиенту.

```json
{
  "rows": [
    {
      "Id": "e6339b62-07b1-4c85-aac9-a9ad00b48fcc",
      "Amount": "100,00",
      "DateTime": "2019-01-22T11:08:19",
      "Description": "Компенсация",
      "Initiator": "Александр Сергеевич Слободчиков",
      "UserName": "Слободчиков Александр Сергеевич",
      "UserId": "f650b726-ed50-b269-869d-adfe0153cc08",
      "BalanceBefore": "250,00",
      "BalanceAfter": "350,00",
      "BalanceBeforeValue": 25000,
      "BalanceAfterValue": 35000
    }
  ],
  "numberOfPages": 2,
  "page": 0
}
```