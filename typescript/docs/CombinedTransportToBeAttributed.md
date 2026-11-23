
# CombinedTransportToBeAttributed


## Properties

Name | Type
------------ | -------------
`start` | [Location](Location.md)
`destination` | [Location](Location.md)
`polyline` | string
`name` | string
`attributes` | [CombinedTransportAttributes](CombinedTransportAttributes.md)
`unmatchedAfterMapUpdate` | boolean
`description` | string

## Example

```typescript
import type { CombinedTransportToBeAttributed } from ''

// TODO: Update the object below with actual values
const example = {
  "start": null,
  "destination": null,
  "polyline": null,
  "name": null,
  "attributes": null,
  "unmatchedAfterMapUpdate": null,
  "description": null,
} satisfies CombinedTransportToBeAttributed

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CombinedTransportToBeAttributed
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


