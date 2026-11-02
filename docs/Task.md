
# Task


## Properties

Name | Type
------------ | -------------
`name` | string
`description` | string
`status` | string
`userAssigned` | [User](User.md)
`priority` | number
`dueDate` | Date
`id` | number
`type` | number
`user` | [User](User.md)
`dealer` | [Dealer](Dealer.md)
`accountId` | string
`dateAdded` | Date
`dateCreated` | Date
`dateUpdated` | Date
`recordSource` | string
`recordOwned` | number

## Example

```typescript
import type { Task } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "name": null,
  "description": null,
  "status": null,
  "userAssigned": null,
  "priority": null,
  "dueDate": null,
  "id": null,
  "type": null,
  "user": null,
  "dealer": null,
  "accountId": null,
  "dateAdded": null,
  "dateCreated": null,
  "dateUpdated": null,
  "recordSource": null,
  "recordOwned": null,
} satisfies Task

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Task
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


