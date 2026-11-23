
# CombinedTransportsResponse

The combined transports selected by the input parameters.

## Properties

Name | Type
------------ | -------------
`combinedTransports` | [Array&lt;CombinedTransport&gt;](CombinedTransport.md)
`warnings` | [Array&lt;Warning&gt;](Warning.md)

## Example

```typescript
import type { CombinedTransportsResponse } from ''

// TODO: Update the object below with actual values
const example = {
  "combinedTransports": null,
  "warnings": null,
} satisfies CombinedTransportsResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CombinedTransportsResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


