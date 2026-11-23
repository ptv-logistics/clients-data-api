
# MapInformationResponse


## Properties

Name | Type
------------ | -------------
`features` | [Features](Features.md)
`geographicalUnits` | [Array&lt;GeographicalUnit&gt;](GeographicalUnit.md)

## Example

```typescript
import type { MapInformationResponse } from ''

// TODO: Update the object below with actual values
const example = {
  "features": null,
  "geographicalUnits": null,
} satisfies MapInformationResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MapInformationResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


