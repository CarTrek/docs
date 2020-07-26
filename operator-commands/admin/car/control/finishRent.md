# Завершить аренду

Принудительное завершение аренды. Позволяет завершить аренду, даже если машина находится за пределамми зоны парковки, а так же вне зависимости от состояния оборудования.

## Запрос

    POST /admin/car/control/finishRent/29686ea2-a698-45eb-97df-a776016d4e44 HTTP/1.1
    Connection: keep-alive
    Content-Length: 0
    Pragma: no-cache
    Cache-Control: no-cache
    Accept: application/json, text/plain, */*
    User-Agent: Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36
    Accept-Encoding: gzip, deflate, br
    Accept-Language: ru-RU,ru;q=0.9,en-US;q=0.8,en;q=0.7,de;q=0.6,sq;q=0.5
    Cookie:sessid=2cJxqqs1WoX4ALBqXKCQkaysjAoDJ7toPQCkV8;

## Ответ

```json
{
    "response":"Заказ успешно завершён."
}
```