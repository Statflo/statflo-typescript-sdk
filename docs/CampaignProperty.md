
# CampaignProperty


## Properties

Name | Type
------------ | -------------
`id` | number
`dealer` | [Dealer](Dealer.md)
`campaign` | [Campaign](Campaign.md)
`campaignPriority` | number
`displayPriority` | number
`carryoverUnattempted` | number
`visibilityCrmStatus` | [CampaignVisibility](CampaignVisibility.md)
`visibilityReportStatus` | [CampaignVisibility](CampaignVisibility.md)
`messageTemplateAssignments` | [Array&lt;MessageTemplateAssignment&gt;](MessageTemplateAssignment.md)

## Example

```typescript
import type { CampaignProperty } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "dealer": null,
  "campaign": null,
  "campaignPriority": null,
  "displayPriority": null,
  "carryoverUnattempted": null,
  "visibilityCrmStatus": null,
  "visibilityReportStatus": null,
  "messageTemplateAssignments": null,
} satisfies CampaignProperty

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CampaignProperty
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


