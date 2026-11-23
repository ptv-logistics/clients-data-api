
# CustomRoadAttributeScenario

A custom road attribute scenario.

## Properties

Name | Type
------------ | -------------
`id` | string
`name` | string
`description` | string
`roadsToBeAttributed` | [Array&lt;RoadsToBeAttributed&gt;](RoadsToBeAttributed.md)
`combinedTransportsToBeAttributed` | [Array&lt;CombinedTransportToBeAttributed&gt;](CombinedTransportToBeAttributed.md)
`shared` | boolean
`active` | boolean
`revision` | number

## Example

```typescript
import type { CustomRoadAttributeScenario } from ''

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "name": null,
  "description": null,
  "roadsToBeAttributed": null,
  "combinedTransportsToBeAttributed": null,
  "shared": null,
  "active": null,
  "revision": null,
} satisfies CustomRoadAttributeScenario

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CustomRoadAttributeScenario
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


