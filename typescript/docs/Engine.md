
# Engine

Physical and legal properties of the engine of a vehicle. It is null for an unpowered vehicle.

## Properties

Name | Type
------------ | -------------
`engineType` | [EngineType](EngineType.md)
`maximumSpeed` | number
`ecoSpeed` | number
`emissionStandard` | [EmissionStandard](EmissionStandard.md)
`power` | number
`officialRange` | number

## Example

```typescript
import type { Engine } from ''

// TODO: Update the object below with actual values
const example = {
  "engineType": null,
  "maximumSpeed": null,
  "ecoSpeed": null,
  "emissionStandard": null,
  "power": null,
  "officialRange": null,
} satisfies Engine

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Engine
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


