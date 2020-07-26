# Аутентификация

Обратите внимание, что при аутентификации не создаётся `sessid`. Идентификатор сеанса есть в любом запросе. После успешного выполнения аутентификации текущему сеансу на сервере сопоставляется польхователь.

## Запрос

```
POST /profile/signin HTTP/1.1
Host: test.cartrek.online
Connection: keep-alive
Content-Length: 48
Accept: application/json, text/plain, */*
User-Agent: Mozilla/5.0 (Windows NT 6.3; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36
Content-Type: application/json;charset=UTF-8
Accept-Encoding: gzip, deflate, br
Accept-Language: ru-RU
Cookie: sessid=R29gobJW49om2ILKnbwbL0ynysnpxHilfMK9s5l9A5qfaGd4KDLSjxjRCVr7xdiv; 
```

## Ответ

```json
{
    "email": "test@example.com",
    "password": "123123"
}
```
