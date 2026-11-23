
# TollSystem

Contains information about the toll system such as the name, operator and especially the different tariff versions that are currently available.

## Properties

Name | Type
------------ | -------------
`name` | string
`operator` | string
`tariffVersions` | [Array&lt;TariffVersion&gt;](TariffVersion.md)

## Example

```typescript
import type { TollSystem } from ''

// TODO: Update the object below with actual values
const example = {
  "name": null,
  "operator": null,
  "tariffVersions": null,
} satisfies TollSystem

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TollSystem
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


