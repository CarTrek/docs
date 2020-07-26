# Деавторизация

После выполнения операции идентификатор сеанса `sessid` остаётся валидным, но отвязывается на сервере от пользователя.
    
## Запрос

    POST /profile/signout HTTP/1.1
    Cookie: sessid=xC9tq10dbYt0X1zejWM299hOHCaUHg72cPWUgZHYFLss26p6iH3
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
    "message": "ok"
}
```