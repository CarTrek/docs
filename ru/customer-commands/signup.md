#Регистрация нового пользователя

После регистрации нового пользователя текущий сеанс автоматически становится авторизованным. В ответ на запрос регистрации нового пользователя возвращается структура, содержащая идентификатор нового пользователя.

## Запрос

```
POST /sign-up HTTP/1.1
Host: test.cartrek.online
Connection: keep-alive
Content-Length: 4052
Accept: application/json, text/plain, */*
User-Agent: Mozilla/5.0 (Windows NT 6.3; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.2924.87 Safari/537.36
Content-Type: multipart/form-data; boundary=----WebKitFormBoundaryaFHeenGod6AfRNmF
Referer: https://main.cartrek.online/Content/sign-up/index.html
Accept-Encoding: gzip, deflate, br
Accept-Language: ru-RU,ru;q=0.8,en-US;q=0.6,en;q=0.4,de;q=0.2,sq;q=0.2
Cookie: sessid=LmYF4ch2N1KqEsGMX1RmXzkC2EsMlcjSsiDpCB8S8u8c1raQZJQjdFtVCWNztVOv; CurrentCulture=ru-RU

------WebKitFormBoundaryaFHeenGod6AfRNmF
Content-Disposition: form-data; name="model"
{"email":"test@example.com","name":"","patronymic":"","surname":"","mobilePhoneNumber":"0000000011","password":"123123","passwordConfirmation":"123123"}
------WebKitFormBoundaryaFHeenGod6AfRNmF
Content-Disposition: form-data; name="passportScan1"; filename="download.png"
Content-Type: image/png
[двоичные данные файла изображения]
------WebKitFormBoundaryaFHeenGod6AfRNmF
Content-Disposition: form-data; name="passportScan2"; filename="download.png"
Content-Type: image/png
[двоичные данные файла изображения]
------WebKitFormBoundaryaFHeenGod6AfRNmF
Content-Disposition: form-data; name="driversLicence1"; filename="download.png"
Content-Type: image/png
[двоичные данные файла изображения]
------WebKitFormBoundaryaFHeenGod6AfRNmF
Content-Disposition: form-data; name="driversLicence2"; filename="download.png"
Content-Type: image/png
[двоичные данные файла изображения]
------WebKitFormBoundaryaFHeenGod6AfRNmF
Content-Disposition: form-data; name="driversSelfie"; filename="download.png"
Content-Type: image/png
[двоичные данные файла изображения]
------WebKitFormBoundaryaFHeenGod6AfRNmF--
```

## Ответ

```json
{
    "guid": "44d3e465-64d7-4aae-9b83-225e3663179a",
    "email": "test@example.com"
}
```