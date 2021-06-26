## Simulator input/output profile (flatfile)

| data element | data format option | format |
| --------------- | --------------- | --------------- |
| gpsterminalid | character | Not Applicable |
| lat | number | #.###### |
| long | number | #.###### |
| temperature | number | #.## |
| speed | number | #.## |
| fueltotal | number | #.## |
| distancetotal | number | #.## |
| fueldiff | number | #.## |
| distancediff | number | #.## |
| fuelefficiency | number | #.## |
| timestamp | datetime | yyyy-MM-dd'T'HH:mm:ss.SSS'Z' |

## Simulator map Function Inputs

| Input name | Input type |
| --------------- | --------------- |
| gpsterminalidinput | character |
| latitudeinput | Float |
| longitudeinput | Float |
| temperatureinput | Float |
| fueltotalinput | Float |
| distancetotalinput | Float |
| timestamp | datetime

## Simulator map Function Outputs

| Output name |
| --------------- |
| gpsterminalidoutput |
| latitudeoutput |
| longitudeoutput |
| temperatureoutput |
| speedoutput |
| fueltotaloutput |
| distancetotaloutput |
| fueldiffoutput |
| distanceoutput |
| fuelefficiencyoutput |
| timestampoutput |

## Processor Map Input Profile (Flatfile)

> **NOTE** timestamp format is retained as character as incoming messages are received as string and then transformed to JSON, wherein date/time formats are not understood by JSON.. So we retain timestamp value as type "character"

| data element | data format option | format |
| --------------- | --------------- | --------------- |
| gpsterminalid | character | Not Applicable |
| lat | number | #.###### |
| long | number | #.###### |
| temperature | number | #.## |
| speed | number | #.## |
| fueltotal | number | #.## |
| distancetotal | number | #.## |
| fueldiff | number | #.## |
| distancediff | number | #.## |
| fuelefficiency | number | #.## |
| timestamp | character | Not Applicable |

## gpsinventory-http-req/res-profile (JSON)

| data element | data format option | format |
| --------------- | --------------- | --------------- |
| gpsterminalId | character | Not Applicable |
| customerId | character | Not Applicable |
| customerName | character | Not Applicable |
| driverId | character | Not Applicable |
| driverName | character | Not Applicable |
| vehicleNumber | character | Not Applicable |
| vehicleCategory | character | Not Applicable |
| distanceTotal | number | #.## |
| fuelTotal | number | #.## |
| lat | number | #.###### |
| lon | number | #.###### |
