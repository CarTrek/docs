# Получение минутных тарифов

Используется для запроса актуального минутного тарифа. Актуальный тариф выбирается сервером для конкретного автомобиля на основании времени суток, дня недели, модели, пробега, типа трансмиссии автомобиля, групп доступа текущего пользователя и автомобиля (перечень параметров может расширяться в будущем). Стоимости в ответе указываются в копейках.

## Запрос

    GET /api/rates/perminute/current?carId=e9e9a3cf-d6f9-4011-9352-a712015a35c8 HTTP/1.1
    Cookie: sessid=xC9tq10dbYt0X1zeROheVFUHxA6aVjWM291hOHCaUHg72cPWUgZdYFLss26p6iH3
    Accept-Language: en-US
    Host: 192.168.1.35:4000
    Connection: Keep-Alive
    Accept-Encoding: gzip
    User-Agent: okhttp/2.7.0

## Ответ

```json
{
  "rate": {
    "id": "0d2426e5-020f-41b2-ad8d-a82e0152f8a4",
    "name": "Минутный тариф",
    "hourFrom": 20,
    "hourTo": 15,
    "bookRate": 0,
    "parkRate": 100,
    "driveRate": 200,
    "runIncluded": 3,
    "overrunCostPerKm": 400,
    "fromHour": 20,
    "toHour": 15,
    "applyToTransmissionType": 0,
    "minMileage": null,
    "maxMileage": null,
    "models": null,
    "discount": 0,
    "idleTimeFromSeconds": null,
    "idleTimeToSeconds": null
  }
}
```