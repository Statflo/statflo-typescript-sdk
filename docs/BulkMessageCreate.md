
# BulkMessageCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`userId` | number
`templateId` | string
`campaignId` | number
`locationId` | number
`deliveryStatus` | string
`provider` | string
`content` | string
`dateAdded` | Date

## Example

```typescript
import type { BulkMessageCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "userId": null,
  "templateId": null,
  "campaignId": null,
  "locationId": null,
  "deliveryStatus": null,
  "provider": null,
  "content": null,
  "dateAdded": null,
} satisfies BulkMessageCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BulkMessageCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


