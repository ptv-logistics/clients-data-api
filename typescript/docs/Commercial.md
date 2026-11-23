
# Commercial

Properties of a vehicle from a commercial point of view.

## Properties

Name | Type
------------ | -------------
`manufacturer` | string
`model` | string
`variant` | string
`launchYear` | number

## Example

```typescript
import type { Commercial } from ''

// TODO: Update the object below with actual values
const example = {
  "manufacturer": FunnyTrucks Inc.,
  "model": FT1,
  "variant": null,
  "launchYear": 2020,
} satisfies Commercial

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Commercial
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


