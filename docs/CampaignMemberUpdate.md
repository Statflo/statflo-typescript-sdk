
# CampaignMemberUpdate


## Properties

Name | Type
------------ | -------------
`id` | number
`accountId` | string
`phoneNumber` | string
`accountName` | string
`campaignId` | number
`startDate` | Date
`endDate` | Date
`secondaryDealerId` | string
`campaignNickname` | string
`source` | string
`dateCreated` | Date
`excludeDnc` | string
`excludeDncDate` | Date
`excludeKill` | string
`excludeDuplicate` | string
`excludeTerminated` | string
`excludeTerminatedDate` | Date
`excludePrepaid` | string
`excludeNoDealerMatch` | string
`excludeArchived` | string
`excludeLegacy` | string

## Example

```typescript
import type { CampaignMemberUpdate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "accountId": null,
  "phoneNumber": null,
  "accountName": null,
  "campaignId": null,
  "startDate": null,
  "endDate": null,
  "secondaryDealerId": null,
  "campaignNickname": null,
  "source": null,
  "dateCreated": null,
  "excludeDnc": null,
  "excludeDncDate": null,
  "excludeKill": null,
  "excludeDuplicate": null,
  "excludeTerminated": null,
  "excludeTerminatedDate": null,
  "excludePrepaid": null,
  "excludeNoDealerMatch": null,
  "excludeArchived": null,
  "excludeLegacy": null,
} satisfies CampaignMemberUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CampaignMemberUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


