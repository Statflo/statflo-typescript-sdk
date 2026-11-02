
# ContentSharingRecommendedCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`campaign` | [Campaign](Campaign.md)
`campaignId` | number
`link` | [ContentSharingLink](ContentSharingLink.md)
`contentId` | number
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { ContentSharingRecommendedCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "campaign": null,
  "campaignId": null,
  "link": null,
  "contentId": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies ContentSharingRecommendedCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ContentSharingRecommendedCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


