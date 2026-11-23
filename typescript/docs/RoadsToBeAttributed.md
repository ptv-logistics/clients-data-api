
# RoadsToBeAttributed


## Properties

Name | Type
------------ | -------------
`points` | string
`polylines` | Array&lt;string&gt;
`direction` | [RoadDirectionType](RoadDirectionType.md)
`attributes` | [RoadAttributes](RoadAttributes.md)
`validity` | [Validity](Validity.md)
`unmatchedAfterMapUpdate` | boolean
`description` | string

## Example

```typescript
import type { RoadsToBeAttributed } from ''

// TODO: Update the object below with actual values
const example = {
  "points": null,
  "polylines": null,
  "direction": null,
  "attributes": null,
  "validity": null,
  "unmatchedAfterMapUpdate": null,
  "description": null,
} satisfies RoadsToBeAttributed

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RoadsToBeAttributed
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


