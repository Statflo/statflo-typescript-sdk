
# ContentSharingLink


## Properties

Name | Type
------------ | -------------
`id` | number
`dealer` | [Dealer](Dealer.md)
`category` | [ContentSharingCategory](ContentSharingCategory.md)
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
import type { ContentSharingLink } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "dealer": null,
  "category": null,
  "language": null,
  "name": null,
  "description": null,
  "url": null,
  "image": null,
  "status": null,
  "displayOrder": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies ContentSharingLink

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ContentSharingLink
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


