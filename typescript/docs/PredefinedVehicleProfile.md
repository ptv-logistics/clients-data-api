
# PredefinedVehicleProfile


## Properties

Name | Type
------------ | -------------
`name` | string
`description` | string
`region` | [RegionType](RegionType.md)
`vehicle` | [Vehicle](Vehicle.md)
`currency` | string
`monetaryCostOptions` | [MonetaryCostOptions](MonetaryCostOptions.md)
`routeOptions` | [RouteOptions](RouteOptions.md)

## Example

```typescript
import type { PredefinedVehicleProfile } from ''

// TODO: Update the object below with actual values
const example = {
  "name": null,
  "description": null,
  "region": null,
  "vehicle": null,
  "currency": null,
  "monetaryCostOptions": null,
  "routeOptions": null,
} satisfies PredefinedVehicleProfile

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PredefinedVehicleProfile
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


