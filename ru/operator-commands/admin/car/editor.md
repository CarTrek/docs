# Получить конфигурацию автомобиля

## Запрос

    GET /admin/car/editor/b34fbcda-6311-456c-80c2-a7e601131165 HTTP/1.1
    Host: test.cartrek.online
    Connection: keep-alive
    Pragma: no-cache
    Cache-Control: no-cache
    Accept: application/json, text/plain, */*
    User-Agent: Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36
    Accept-Encoding: gzip, deflate, br
    Accept-Language: ru-RU,ru;q=0.9,en-US;q=0.8,en;q=0.7,de;q=0.6,sq;q=0.5
    Cookie: sessid=2cJxqqs1Wrx9b6kaysjAoDJ7toPQCkV8

## Ответ

```json
{
  "Id": "b34fbcda-6311-456c-80c2-a7e601131165",
  "DisplayName": "VW Polo 9411",
  "CarModelDisplayName": "VW Polo",
  "CarModel": {
    "displayName": "VW Polo",
    "id": "5d472799-f687-4fba-8a71-a70300f0a624"
  },
  "RegNumber": "9411",
  "Active": true,
  "TrackerId": "Cartrek.FuelX2Signal.9411",
  "Phone1": "",
  "Phone2": "",
  "BluetoothAllowed": false,
  "Color": "Черный",
  "Comment": "10.10 тест",
  "TransmissionType": 0,
  "TroubleBodyIsDamagedCount": 0,
  "TroubleBrokenWindowCount": 0,
  "TroubleCarIsDirtyCount": 0,
  "TroubleTireIsFlatCount": 0,
  "LastRepairDateTime": "2017-11-18T11:52:28+03:00",
  "LastTroubleBodyIsDamaged": null,
  "LastTroubleBrokenWindow": null,
  "LastTroubleCarIsDirtyTime": null,
  "LastTroubleTireIsFlat": null,
  "CommentsCount": 0,
  "Reserve": null,
  "Discount": false,
  "StartMileage": 15469,
  "MilageBeforeChange": 15469,
  "Tags": [],
  "Cdi": null
}

```