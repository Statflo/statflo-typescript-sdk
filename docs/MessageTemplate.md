
# MessageTemplate


## Properties

Name | Type
------------ | -------------
`id` | string
`carrier` | [Carrier](Carrier.md)
`dealer` | [Dealer](Dealer.md)
`templateName` | string
`language` | string
`metadata` | object
`template` | object
`campaign` | [Campaign](Campaign.md)
`priority` | number
`messageTemplateAssignments` | [Array&lt;MessageTemplateAssignment&gt;](MessageTemplateAssignment.md)
`categories` | [Array&lt;MessageTemplateCategory&gt;](MessageTemplateCategory.md)
`dateCreated` | Date

## Example

```typescript
import type { MessageTemplate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "carrier": null,
  "dealer": null,
  "templateName": null,
  "language": null,
  "metadata": null,
  "template": null,
  "campaign": null,
  "priority": null,
  "messageTemplateAssignments": null,
  "categories": null,
  "dateCreated": null,
} satisfies MessageTemplate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MessageTemplate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


