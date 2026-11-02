
# MessageMediaCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`messageId` | number
`url` | string
`contentType` | string
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { MessageMediaCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "messageId": null,
  "url": null,
  "contentType": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies MessageMediaCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MessageMediaCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


