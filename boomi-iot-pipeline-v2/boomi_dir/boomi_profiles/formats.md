## Simulator input/output profile (data elements, data types, formats)

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

## Simulator Function Inputs

| Input name | Input type |
| --------------- | --------------- |
| gpsterminalidinput | character |
| latitudeinput | Float |
| longitudeinput | Float |
| temperatureinput | Float |
| fueltotalinput | Float |
| distancetotalinput | Float |
| timestamp | datetime

## Simulator Function Outputs

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


