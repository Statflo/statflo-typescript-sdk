
# ContactActionUpdate


## Properties

Name | Type
------------ | -------------
`messageContent` | string
`messageTo` | string
`messageFrom` | string
`actionTaken` | string
`subject` | string
`sourceId` | string
`nextSteps` | string
`nextDate` | Date
`outcomeReason` | string
`messageTemplateId` | string
`id` | number
`type` | number
`accountId` | string
`dateAdded` | Date
`dateCreated` | Date
`dateUpdated` | Date
`recordSource` | string
`recordOwned` | number

## Example

```typescript
import type { ContactActionUpdate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "messageContent": null,
  "messageTo": null,
  "messageFrom": null,
  "actionTaken": null,
  "subject": null,
  "sourceId": null,
  "nextSteps": null,
  "nextDate": null,
  "outcomeReason": null,
  "messageTemplateId": null,
  "id": null,
  "type": null,
  "accountId": null,
  "dateAdded": null,
  "dateCreated": null,
  "dateUpdated": null,
  "recordSource": null,
  "recordOwned": null,
} satisfies ContactActionUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ContactActionUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


