# Получение трека атвомобиля

Есть возможность получать выборки путевых точек машин с ограничением по дате и времени и географическим координатам.

## Запрос

    GET /admin/waypoints/full/car/c30a1460-e3f9-6fc7-8422-a96e00f6cdc9?w=37.3216724395752&s=55.669844096237284&e=37.655210494995124&n=55.718226789012704&dateFrom=2019-01-21T11:00:00.000Z&dateTo=2019-01-22T12:00:00.000Z&count=1000 HTTP/1.1
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


w - западная граница для запроса
s - южная граница для запроса
e - восточная граница для запроса
n - северная граница дл запроса

dateFrom - дата и время начала выборки
dateЕTo- дата и время окончания выборки

count - приблизительное максимальне окличество точек в выборке. В ответе максимальное число точек может отличаться на 10%. 


## Ответ

``` json
[
  {
    "Id": 5222350,
    "Car": null,
    "Order": null,
    "DateTimeUtc": "2019-01-21T11:00:02",
    "Lat": 33405543,
    "Lon": 22482159,
    "Alt": 183,
    "Azimuth": 312,
    "Speed": 0,
    "FuelLevel": 99,
    "IsLocked": null,
    "IsDoorsClosed": null,
    "IsEngineStarted": null,
    "IsImmobilized": null,
    "IsIgnitionOn": null,
    "GsmLevel": 75,
    "BatteryLevel": null,
    "IsParked": null,
    "IsCharging": null,
    "Mileage": 5029.97656,
    "MileageCAN": null,
    "IsOnline": null,
    "FuelConsumption": null,
    "EngineSpeed": -1,
    "Voltage": 13.619,
    "RezervVoltage": null,
    "LightsOn": false,
    "HandBrakeOn": false
  }
]
```

*Примечание* Координаты Lat и Lon передаются в целочисленном виде. Для получения значений в градусах целочисленные значения необходимо разделить на 600,000.