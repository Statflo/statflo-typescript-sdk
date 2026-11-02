
# CarrierStatisticCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`type` | number
`accountId` | string
`accountName` | string
`approach` | string
`phoneNumber` | string
`contactName` | string
`totalSubscriber` | number
`potentialRenewal` | number
`campaignDateAdded` | Date
`campaignId` | string

## Example

```typescript
import type { CarrierStatisticCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "type": null,
  "accountId": null,
  "accountName": null,
  "approach": null,
  "phoneNumber": null,
  "contactName": null,
  "totalSubscriber": null,
  "potentialRenewal": null,
  "campaignDateAdded": null,
  "campaignId": null,
} satisfies CarrierStatisticCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CarrierStatisticCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


