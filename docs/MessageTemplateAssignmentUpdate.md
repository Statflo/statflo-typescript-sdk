
# MessageTemplateAssignmentUpdate


## Properties

Name | Type
------------ | -------------
`id` | string
`propertyId` | number
`templateId` | string
`dealerId` | number
`priority` | number
`assignDate` | Date
`dateUpdate` | Date
`unassignDate` | Date

## Example

```typescript
import type { MessageTemplateAssignmentUpdate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "propertyId": null,
  "templateId": null,
  "dealerId": null,
  "priority": null,
  "assignDate": null,
  "dateUpdate": null,
  "unassignDate": null,
} satisfies MessageTemplateAssignmentUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MessageTemplateAssignmentUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


