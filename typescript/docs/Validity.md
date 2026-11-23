
# Validity

The periods during which the attributes are valid. If both time intervals and weekly schedule are specified, the attributes are valid only during the weekly schedule within the time intervals. If there is no such period, the attributes are never valid. If not specified, the attributes are always valid.

## Properties

Name | Type
------------ | -------------
`timeIntervals` | [Array&lt;TimeInterval&gt;](TimeInterval.md)
`weeklySchedule` | [Array&lt;WeeklyScheduleInterval&gt;](WeeklyScheduleInterval.md)

## Example

```typescript
import type { Validity } from ''

// TODO: Update the object below with actual values
const example = {
  "timeIntervals": null,
  "weeklySchedule": null,
} satisfies Validity

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Validity
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


