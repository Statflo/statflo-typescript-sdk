
# NotificationLogCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`dealerId` | number
`userId` | number
`payload` | object
`channel` | string
`type` | string
`recordSource` | string
`entity` | string
`entityId` | object
`externalId` | string
`deliveredAt` | Date
`createdAt` | Date

## Example

```typescript
import type { NotificationLogCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "dealerId": null,
  "userId": null,
  "payload": null,
  "channel": null,
  "type": null,
  "recordSource": null,
  "entity": null,
  "entityId": null,
  "externalId": null,
  "deliveredAt": null,
  "createdAt": null,
} satisfies NotificationLogCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as NotificationLogCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


