
# AccountCredentialCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`accountSid` | string
`authToken` | string
`secondaryBusinessProfileSid` | string
`addressSid` | string
`supportingDocumentSid` | string
`customerProfileBusinessInformationSid` | string
`authorizedRepresentativeSid` | string
`messagingServiceId` | string

## Example

```typescript
import type { AccountCredentialCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "accountSid": null,
  "authToken": null,
  "secondaryBusinessProfileSid": null,
  "addressSid": null,
  "supportingDocumentSid": null,
  "customerProfileBusinessInformationSid": null,
  "authorizedRepresentativeSid": null,
  "messagingServiceId": null,
} satisfies AccountCredentialCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AccountCredentialCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


