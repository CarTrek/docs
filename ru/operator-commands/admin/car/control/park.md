# Перевести заказ в режим парковки

Принудительно переводит заказ в режим парковки.

## Запрос

    POST /admin/car/control/park/29686ea2-a698-45eb-97df-a776016d4e44 HTTP/1.1
    Connection: keep-alive
    Content-Length: 0
    Pragma: no-cache
    Cache-Control: no-cache
    Accept: application/json, text/plain, */*
    User-Agent: Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36
    Accept-Encoding: gzip, deflate, br
    Accept-Language: ru-RU,ru;q=0.9,en-US;q=0.8,en;q=0.7,de;q=0.6,sq;q=0.5
    Cookie: sessid=2cJxqqs1Wrx9b6XiOhQwq5sei;

## Ответ

```json
{
    "response": "Автомобиль переведён в режим парковки."
}
```