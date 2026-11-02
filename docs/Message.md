
# Message


## Properties

Name | Type
------------ | -------------
`id` | number
`user` | [User](User.md)
`conversation` | [Conversation](Conversation.md)
`content` | string
`action` | string
`provider` | string
`referenceId` | string
`deliveryStatus` | string
`ipAddress` | string
`associatedAppPhoneNumber` | string
`associatedAppPhoneNumberType` | string
`messageTemplate` | [MessageTemplate](MessageTemplate.md)
`bulkMessage` | [BulkMessage](BulkMessage.md)
`dateAdded` | Date
`dateSent` | Date
`media` | [Array&lt;MessageMedia&gt;](MessageMedia.md)

## Example

```typescript
import type { Message } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "user": null,
  "conversation": null,
  "content": null,
  "action": null,
  "provider": null,
  "referenceId": null,
  "deliveryStatus": null,
  "ipAddress": null,
  "associatedAppPhoneNumber": null,
  "associatedAppPhoneNumberType": null,
  "messageTemplate": null,
  "bulkMessage": null,
  "dateAdded": null,
  "dateSent": null,
  "media": null,
} satisfies Message

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Message
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


