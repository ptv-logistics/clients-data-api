
# CombinedTransportLocation

Represents the start or destination location of a combined transport, e.g. the port. The fields **latitude** and **longitude**  can be used as input for combined transport waypoints in the method **calculateRoutePost** of the Routing API.

## Properties

Name | Type
------------ | -------------
`latitude` | number
`longitude` | number
`name` | string
`countryCode` | string

## Example

```typescript
import type { CombinedTransportLocation } from ''

// TODO: Update the object below with actual values
const example = {
  "latitude": 49.480301,
  "longitude": 6.110667,
  "name": null,
  "countryCode": null,
} satisfies CombinedTransportLocation

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CombinedTransportLocation
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


