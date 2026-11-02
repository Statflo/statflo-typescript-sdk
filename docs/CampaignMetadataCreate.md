
# CampaignMetadataCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`dealerId` | number
`campaignId` | number
`metadata` | string
`value` | object
`dateAdded` | Date

## Example

```typescript
import type { CampaignMetadataCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "dealerId": null,
  "campaignId": null,
  "metadata": null,
  "value": null,
  "dateAdded": null,
} satisfies CampaignMetadataCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CampaignMetadataCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


