
# CallActivityCreate


## Properties

Name | Type
------------ | -------------
`callTo` | string
`content` | string
`title` | string
`actionTaken` | string
`nextSteps` | string
`nextDate` | Date
`callOutcome` | string
`outcomeLocation` | string
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
import type { CallActivityCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "callTo": null,
  "content": null,
  "title": null,
  "actionTaken": null,
  "nextSteps": null,
  "nextDate": null,
  "callOutcome": null,
  "outcomeLocation": null,
  "id": null,
  "type": null,
  "accountId": null,
  "dateAdded": null,
  "dateCreated": null,
  "dateUpdated": null,
  "recordSource": null,
  "recordOwned": null,
} satisfies CallActivityCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CallActivityCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


