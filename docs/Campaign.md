
# Campaign


## Properties

Name | Type
------------ | -------------
`id` | number
`campaignNickname` | string
`totangoName` | string
`type` | string
`frequency` | string
`lifetime` | string
`method` | string
`carrierAllowed` | boolean
`accountType` | string
`dncScrub` | boolean
`reportingPeriodType` | string
`reportingPeriodBefore` | number
`reportingPeriodAfter` | number
`transactionEarliest` | string
`transactionLatest` | string
`productTypes` | string
`source` | string
`campaignMetadata` | [Array&lt;CampaignMetadata&gt;](CampaignMetadata.md)
`campaignMappings` | [Array&lt;CampaignMapping&gt;](CampaignMapping.md)
`campaignProperties` | [Array&lt;CampaignProperty&gt;](CampaignProperty.md)

## Example

```typescript
import type { Campaign } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "campaignNickname": null,
  "totangoName": null,
  "type": null,
  "frequency": null,
  "lifetime": null,
  "method": null,
  "carrierAllowed": null,
  "accountType": null,
  "dncScrub": null,
  "reportingPeriodType": null,
  "reportingPeriodBefore": null,
  "reportingPeriodAfter": null,
  "transactionEarliest": null,
  "transactionLatest": null,
  "productTypes": null,
  "source": null,
  "campaignMetadata": null,
  "campaignMappings": null,
  "campaignProperties": null,
} satisfies Campaign

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Campaign
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


