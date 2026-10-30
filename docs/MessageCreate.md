
# MessageCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`userId` | number
`conversationId` | number
`content` | string
`action` | string
`provider` | string
`referenceId` | string
`deliveryStatus` | string
`ipAddress` | string
`associatedAppPhoneNumber` | string
`associatedAppPhoneNumberType` | string
`messageTemplateId` | string
`bulkMessageId` | number
`dateAdded` | Date
`dateSent` | Date

## Example

```typescript
import type { MessageCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "userId": null,
  "conversationId": null,
  "content": null,
  "action": null,
  "provider": null,
  "referenceId": null,
  "deliveryStatus": null,
  "ipAddress": null,
  "associatedAppPhoneNumber": null,
  "associatedAppPhoneNumberType": null,
  "messageTemplateId": null,
  "bulkMessageId": null,
  "dateAdded": null,
  "dateSent": null,
} satisfies MessageCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MessageCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


