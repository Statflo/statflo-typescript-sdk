
# ReassignRep


## Properties

Name | Type
------------ | -------------
`id` | number
`dealer` | [Dealer](Dealer.md)
`user` | [User](User.md)
`newExternalUserId` | string
`oldExternalUserId` | string
`newExternalLocationId` | string
`oldExternalLocationId` | string
`accountName` | string
`accountId` | string
`dateChanged` | Date
`reason` | string
`oldBan` | string

## Example

```typescript
import type { ReassignRep } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "dealer": null,
  "user": null,
  "newExternalUserId": null,
  "oldExternalUserId": null,
  "newExternalLocationId": null,
  "oldExternalLocationId": null,
  "accountName": null,
  "accountId": null,
  "dateChanged": null,
  "reason": null,
  "oldBan": null,
} satisfies ReassignRep

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ReassignRep
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


