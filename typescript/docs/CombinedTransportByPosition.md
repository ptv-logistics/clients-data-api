
# CombinedTransportByPosition

The position around which to search for the start location of a combined transport. This parameter is mutually exclusive with **text**.

## Properties

Name | Type
------------ | -------------
`latitude` | number
`longitude` | number
`radius` | number

## Example

```typescript
import type { CombinedTransportByPosition } from ''

// TODO: Update the object below with actual values
const example = {
  "latitude": 49.480301,
  "longitude": 6.110667,
  "radius": null,
} satisfies CombinedTransportByPosition

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CombinedTransportByPosition
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


