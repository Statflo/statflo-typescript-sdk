
# LocationExternalIdUpdate


## Properties

Name | Type
------------ | -------------
`id` | string
`locationId` | number
`provider` | string
`fieldName` | string
`fieldValue` | string
`recordSource` | string
`dateCreated` | Date
`dateUpdated` | Date

## Example

```typescript
import type { LocationExternalIdUpdate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "locationId": null,
  "provider": null,
  "fieldName": null,
  "fieldValue": null,
  "recordSource": null,
  "dateCreated": null,
  "dateUpdated": null,
} satisfies LocationExternalIdUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LocationExternalIdUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


