
# ContactConsentLog


## Properties

Name | Type
------------ | -------------
`id` | number
`contact` | [Contact](Contact.md)
`timestamp` | Date
`change` | object
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { ContactConsentLog } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "contact": null,
  "timestamp": null,
  "change": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies ContactConsentLog

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ContactConsentLog
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


