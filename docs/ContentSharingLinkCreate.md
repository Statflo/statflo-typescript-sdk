
# ContentSharingLinkCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`dealerId` | number
`categoryId` | number
`language` | string
`name` | string
`description` | string
`url` | string
`image` | string
`status` | boolean
`displayOrder` | number
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { ContentSharingLinkCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "dealerId": null,
  "categoryId": null,
  "language": null,
  "name": null,
  "description": null,
  "url": null,
  "image": null,
  "status": null,
  "displayOrder": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies ContentSharingLinkCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ContentSharingLinkCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


