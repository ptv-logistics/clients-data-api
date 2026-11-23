
# CombinedTransportByText

The parameters to search for in the combined transport data. This parameter is mutually exclusive with **position**.

## Properties

Name | Type
------------ | -------------
`query` | string
`allowedCountries` | string

## Example

```typescript
import type { CombinedTransportByText } from ''

// TODO: Update the object below with actual values
const example = {
  "query": null,
  "allowedCountries": null,
} satisfies CombinedTransportByText

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CombinedTransportByText
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


