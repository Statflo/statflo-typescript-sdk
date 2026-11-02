
# CampaignCreate


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
`visibilityCrm` | number
`visibilityReport` | number

## Example

```typescript
import type { CampaignCreate } from '@statflo/statflo-typescript-sdk'

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
  "visibilityCrm": null,
  "visibilityReport": null,
} satisfies CampaignCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CampaignCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


