
# RoadAttributes

The attributes assigned to each of the selected roads.

## Properties

Name | Type
------------ | -------------
`prohibited` | boolean
`allowed` | boolean
`relativeSpeed` | number
`weightLimit` | number
`heightLimit` | number
`widthLimit` | number

## Example

```typescript
import type { RoadAttributes } from ''

// TODO: Update the object below with actual values
const example = {
  "prohibited": null,
  "allowed": null,
  "relativeSpeed": 70,
  "weightLimit": null,
  "heightLimit": null,
  "widthLimit": null,
} satisfies RoadAttributes

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RoadAttributes
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


