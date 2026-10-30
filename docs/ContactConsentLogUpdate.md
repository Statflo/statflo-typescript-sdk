
# ContactConsentLogUpdate


## Properties

Name | Type
------------ | -------------
`id` | number
`contactId` | number
`timestamp` | Date
`change` | object
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { ContactConsentLogUpdate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "contactId": null,
  "timestamp": null,
  "change": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies ContactConsentLogUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ContactConsentLogUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


