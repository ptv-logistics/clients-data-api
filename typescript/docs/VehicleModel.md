
# VehicleModel


## Properties

Name | Type
------------ | -------------
`id` | string
`predefinedProfile` | string
`vehicleType` | string
`commercial` | [Commercial](Commercial.md)
`engine` | [Engine](Engine.md)
`battery` | [Battery](Battery.md)

## Example

```typescript
import type { VehicleModel } from ''

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "predefinedProfile": null,
  "vehicleType": null,
  "commercial": null,
  "engine": null,
  "battery": null,
} satisfies VehicleModel

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as VehicleModel
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


