
# CombinedTransport


## Properties

Name | Type
------------ | -------------
`polyline` | string
`name` | string
`duration` | number
`type` | string
`start` | [CombinedTransportLocation](CombinedTransportLocation.md)
`destination` | [CombinedTransportLocation](CombinedTransportLocation.md)
`allowedFor` | string
`waypointsParameter` | string

## Example

```typescript
import type { CombinedTransport } from ''

// TODO: Update the object below with actual values
const example = {
  "polyline": null,
  "name": null,
  "duration": null,
  "type": null,
  "start": null,
  "destination": null,
  "allowedFor": null,
  "waypointsParameter": combinedTransport=54.5009693,11.2273406,54.6604379,11.3608932,
} satisfies CombinedTransport

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CombinedTransport
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


