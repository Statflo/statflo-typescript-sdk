
# ContactUpdate


## Properties

Name | Type
------------ | -------------
`id` | number
`accountName` | string
`accountId` | string
`contactName` | string
`streetNumber` | string
`streetName` | string
`city` | string
`province` | string
`country` | string
`zipCode` | string
`phoneNumber` | string
`phoneExtension` | string
`email` | string
`primaryContact` | boolean
`dateAdded` | Date
`dateCreated` | Date
`dateUpdated` | Date
`jobTitle` | string
`source` | string
`sourceId` | number
`customerId` | string
`oldBan` | string
`smsCapable` | boolean
`flag` | string
`optedOut` | object
`communicationMethods` | object
`firstName` | string
`preferredLanguage` | string

## Example

```typescript
import type { ContactUpdate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "accountName": null,
  "accountId": null,
  "contactName": null,
  "streetNumber": null,
  "streetName": null,
  "city": null,
  "province": null,
  "country": null,
  "zipCode": null,
  "phoneNumber": null,
  "phoneExtension": null,
  "email": null,
  "primaryContact": null,
  "dateAdded": null,
  "dateCreated": null,
  "dateUpdated": null,
  "jobTitle": null,
  "source": null,
  "sourceId": null,
  "customerId": null,
  "oldBan": null,
  "smsCapable": null,
  "flag": null,
  "optedOut": null,
  "communicationMethods": null,
  "firstName": null,
  "preferredLanguage": null,
} satisfies ContactUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as ContactUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


