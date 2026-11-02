
# DealerExternalId


## Properties

Name | Type
------------ | -------------
`id` | string
`dealer` | [Dealer](Dealer.md)
`provider` | string
`fieldName` | string
`fieldValue` | string
`recordSource` | string
`dateCreated` | Date
`updatedAt` | Date

## Example

```typescript
import type { DealerExternalId } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "dealer": null,
  "provider": null,
  "fieldName": null,
  "fieldValue": null,
  "recordSource": null,
  "dateCreated": null,
  "updatedAt": null,
} satisfies DealerExternalId

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DealerExternalId
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


