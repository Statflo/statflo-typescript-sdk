
# BulkMessage


## Properties

Name | Type
------------ | -------------
`id` | number
`user` | [User](User.md)
`dealer` | [Dealer](Dealer.md)
`template` | [MessageTemplate](MessageTemplate.md)
`campaign` | [Campaign](Campaign.md)
`location` | [Location](Location.md)
`deliveryStatus` | string
`provider` | string
`content` | string
`dateAdded` | Date

## Example

```typescript
import type { BulkMessage } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "user": null,
  "dealer": null,
  "template": null,
  "campaign": null,
  "location": null,
  "deliveryStatus": null,
  "provider": null,
  "content": null,
  "dateAdded": null,
} satisfies BulkMessage

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as BulkMessage
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


