
# RoadDirectionType

The direction of the road the attributes apply to.  * `POLYLINE_DIRECTION` - Describes the direction from the start node to the end node of the polyline of the road.  * `REVERSE_POLYLINE_DIRECTION` - Describes the direction from the end node to the start node of the polyline of the road.  * `BOTH` - Describes both directions.  If the selection contains more than one road and the direction is different from _BOTH_, an error will be returned.

## Properties

Name | Type
------------ | -------------

## Example

```typescript
import type { RoadDirectionType } from ''

// TODO: Update the object below with actual values
const example = {
} satisfies RoadDirectionType

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RoadDirectionType
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


