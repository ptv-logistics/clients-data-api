
# PenaltyOptions

Options to configure default penalties for specific road categories or road types. Penalties influence the route calculation by making certain roads more or less attractive.

## Properties

Name | Type
------------ | -------------
`byRoadCategory` | Array&lt;number&gt;
`deliveryOnly` | number
`residentsOnly` | number
`toll` | number
`ferries` | number
`railShuttles` | number

## Example

```typescript
import type { PenaltyOptions } from ''

// TODO: Update the object below with actual values
const example = {
  "byRoadCategory": null,
  "deliveryOnly": null,
  "residentsOnly": null,
  "toll": null,
  "ferries": null,
  "railShuttles": null,
} satisfies PenaltyOptions

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as PenaltyOptions
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


