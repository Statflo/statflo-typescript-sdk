
# ContentSharingCategory


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`description` | string
`displayOrder` | number
`dealer` | [Dealer](Dealer.md)
`createdAt` | Date
`updatedAt` | Date
`links` | [Array&lt;ContentSharingLink&gt;](ContentSharingLink.md)

## Example

```typescript
import type { ContentSharingCategory } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "name": null,
  "description": null,
  "displayOrder": null,
  "dealer": null,
  "createdAt": null,
  "updatedAt": null,
  "links": null,
} satisfies ContentSharingCategory

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ContentSharingCategory
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


