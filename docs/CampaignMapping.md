
# CampaignMapping


## Properties

Name | Type
------------ | -------------
`id` | number
`carrier` | [Carrier](Carrier.md)
`campaign` | [Campaign](Campaign.md)
`fileName` | string
`dateAdded` | Date

## Example

```typescript
import type { CampaignMapping } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "carrier": null,
  "campaign": null,
  "fileName": null,
  "dateAdded": null,
} satisfies CampaignMapping

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CampaignMapping
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


