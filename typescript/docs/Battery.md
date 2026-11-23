
# Battery

Physical properties of the battery regarding capacity and charging. It is null for an unpowered vehicle.  Relevant for `range calculation`.

## Properties

Name | Type
------------ | -------------
`totalCapacity` | number
`acChargingPower` | number
`dcChargingPower` | number
`plugs` | Array&lt;string&gt;

## Example

```typescript
import type { Battery } from ''

// TODO: Update the object below with actual values
const example = {
  "totalCapacity": null,
  "acChargingPower": null,
  "dcChargingPower": null,
  "plugs": ["CCS 2","Type 2"],
} satisfies Battery

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Battery
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


