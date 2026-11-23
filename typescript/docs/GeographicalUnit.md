
# GeographicalUnit

Base type for a geographical unit. Depending on how the data are built up a country can have subdivisions, e.g. a state in the US, or not. 

## Properties

Name | Type
------------ | -------------
`code` | string
`country` | string
`state` | string
`continent` | [Continent](Continent.md)
`features` | [MapFeatures](MapFeatures.md)

## Example

```typescript
import type { GeographicalUnit } from ''

// TODO: Update the object below with actual values
const example = {
  "code": null,
  "country": null,
  "state": null,
  "continent": null,
  "features": null,
} satisfies GeographicalUnit

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as GeographicalUnit
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


