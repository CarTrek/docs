# Получить полный список автомобилей

## Запрос

    GET /admin/car/list/forMap HTTP/1.1
    Host: test.cartrek.online
    Connection: keep-alive
    Pragma: no-cache
    Cache-Control: no-cache
    Accept: application/json, text/plain, */*
    User-Agent: Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36
    Accept-Encoding: gzip, deflate, br
    Accept-Language: ru-RU,ru;q=0.9,en-US;q=0.8,en;q=0.7,de;q=0.6,sq;q=0.5
    Cookie: sessid=2cJxqqs1Wrx9b7toPQCkV8

## Ответ

```json
[
  {
    "Id": "7342bd1e-4e21-4daa-a114-a86700e17099",
    "CarModelId": "d364488e-e15b-406c-8b03-a75200da081a",
    "TrackerId": "Cartrek.Logan2Signal.555",
    "IsOnline": true,
    "IsLocked": true,
    "FuelLevel": 90,
    "GsmLevel": 75,
    "Lat": 33538272,
    "Lon": 22515128,
    "CarModel": "Smart ForTwo",
    "RegNumber": "В716ВМ799",
    "IsAvailableForRent": true,
    "Phone1": "+",
    "Phone2": "+79693658846",
    "BluetoothAllowed": false,
    "Color": "Белый",
    "Comment": null,
    "IsPersisted": true,
    "Uptime": "4.18:28:16.7947505",
    "Mileage": 0.637490749,
    "FuelConsumption": null,
    "EngineSpeed": -1,
    "Speed": 0,
    "RentState": "",
    "CustomersName": "",
    "CustomersPhoneNumber": "",
    "Voltage": 11.989,
    "RezervVoltage": 4.162,
    "TransmissionType": 2,
    "LightsOn": false,
    "HandBrakeOn": false,
    "Organizations": [
      {
        "Id": "df48dee4-4fe9-4f20-9499-a8670100510e"
      }
    ],
    "CustomersId": ""
  }
]

```