# Получение изображения модели автомобиля

В качестве идентификатора изображения необходимо передавать значение поля modelImageId, полученного из api/cars или profile/userinfo.
В ответ выдаётся содержимое файла изображения.

## Запрос

    GET /CarModel/Image/e896317f-cbd3-486f-91bd-a6ca001a696d HTTP/1.1
    Cookie: sessid=xC9tq10dbYt0X1zeROheVFUHxA6aVjWM299hOHCaUHg72cPWUgZHYFLss26p6iH3
    Accept-Language: en-US
    Host: 192.168.1.35:4000
    Connection: Keep-Alive
    Accept-Encoding: gzip
    User-Agent: okhttp/2.7.0

## Ответ

Файл изображения.