
# CampaignPropertyUpdate


## Properties

Name | Type
------------ | -------------
`id` | number
`dealerId` | number
`campaignId` | number
`campaignPriority` | number
`displayPriority` | number
`carryoverUnattempted` | number
`visibilityCrm` | number
`visibilityReport` | number

## Example

```typescript
import type { CampaignPropertyUpdate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "dealerId": null,
  "campaignId": null,
  "campaignPriority": null,
  "displayPriority": null,
  "carryoverUnattempted": null,
  "visibilityCrm": null,
  "visibilityReport": null,
} satisfies CampaignPropertyUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CampaignPropertyUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


