
# ApiChange


## Properties

Name | Type
------------ | -------------
`type` | [ApiChangeType](ApiChangeType.md)
`date` | Date
`description` | string
`api` | string
`version` | string
`link` | string

## Example

```typescript
import type { ApiChange } from ''

// TODO: Update the object below with actual values
const example = {
  "type": null,
  "date": null,
  "description": null,
  "api": null,
  "version": null,
  "link": null,
} satisfies ApiChange

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ApiChange
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


