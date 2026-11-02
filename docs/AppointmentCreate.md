
# AppointmentCreate


## Properties

Name | Type
------------ | -------------
`id` | string
`dealerId` | number
`timeline` | [Timeline](Timeline.md)
`timelineId` | number
`accountId` | string
`user` | [User](User.md)
`userId` | number
`dateFrom` | Date
`dateTo` | Date
`location` | [AppointmentLocation](AppointmentLocation.md)
`locationId` | string
`note` | string
`dateCreated` | Date
`notifiedAt` | Date
`confirmedAt` | Date

## Example

```typescript
import type { AppointmentCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "dealerId": null,
  "timeline": null,
  "timelineId": null,
  "accountId": null,
  "user": null,
  "userId": null,
  "dateFrom": null,
  "dateTo": null,
  "location": null,
  "locationId": null,
  "note": null,
  "dateCreated": null,
  "notifiedAt": null,
  "confirmedAt": null,
} satisfies AppointmentCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AppointmentCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


