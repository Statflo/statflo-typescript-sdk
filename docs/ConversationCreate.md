
# ConversationCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`contactId` | number
`accountId` | string
`lastReadMessageId` | number
`status` | number
`textkitId` | string
`opportunityScore` | number
`insightsWidgetPayload` | object
`dateAdded` | Date

## Example

```typescript
import type { ConversationCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "contactId": null,
  "accountId": null,
  "lastReadMessageId": null,
  "status": null,
  "textkitId": null,
  "opportunityScore": null,
  "insightsWidgetPayload": null,
  "dateAdded": null,
} satisfies ConversationCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ConversationCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


