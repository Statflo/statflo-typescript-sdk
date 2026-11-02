
# MessageDeliveryStatus


## Properties

Name | Type
------------ | -------------
`id` | number
`message` | [Message](Message.md)
`postback` | object
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { MessageDeliveryStatus } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "message": null,
  "postback": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies MessageDeliveryStatus

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as MessageDeliveryStatus
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


