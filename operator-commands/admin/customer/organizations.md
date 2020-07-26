# Получение списка организаций клиента

## Запрос

    GET /admin/customer/organizations/f65db756-ed50-4269-869d-a6fe0153cc08 HTTP/1.1
    Connection: keep-alive
    Pragma: no-cache
    Cache-Control: no-cache
    Accept: application/json, text/plain, */*
    User-Agent: Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36
    Accept-Encoding: gzip, deflate, br
    Accept-Language: ru-RU,ru;q=0.9,en-US;q=0.8,en;q=0.7,de;q=0.6,sq;q=0.5
    Cookie: sessid=2cJfZKpOB3oX4ALBqXKCQkaysjAoDJ7toPQCkV8;

## Ответ

```json
{
  "Organizations": [
    {
      "Id": "d0806288-b74b-4363-aa4c-a70300f285e6",
      "DisplayName": "Разработчики",
      "InOrganization": true
    },
    {
      "Id": "0eb11213-0a10-422f-8390-a70d009ab23a",
      "DisplayName": "Тест",
      "InOrganization": false
    }
  ]
}
```