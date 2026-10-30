
# UserCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`username` | string
`firstName` | string
`lastName` | string
`company` | string
`email` | string
`password` | string
`language` | string
`salesRepId` | string
`externalLocationId` | string
`districtId` | number
`regionId` | number
`lastLogin` | Date
`phoneNumber` | string
`timezone` | string
`theme` | number
`token` | string
`tokenParagon` | string
`userActive` | boolean
`inboundAvailable` | boolean
`jobTitle` | string
`acceptedTermsConditions` | boolean
`appointmentReminderEmail` | boolean
`dealerId` | number
`roleId` | number
`dateAdded` | Date
`campaignVisibility` | number
`permissions` | Array&lt;number&gt;

## Example

```typescript
import type { UserCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "username": null,
  "firstName": null,
  "lastName": null,
  "company": null,
  "email": null,
  "password": null,
  "language": null,
  "salesRepId": null,
  "externalLocationId": null,
  "districtId": null,
  "regionId": null,
  "lastLogin": null,
  "phoneNumber": null,
  "timezone": null,
  "theme": null,
  "token": null,
  "tokenParagon": null,
  "userActive": null,
  "inboundAvailable": null,
  "jobTitle": null,
  "acceptedTermsConditions": null,
  "appointmentReminderEmail": null,
  "dealerId": null,
  "roleId": null,
  "dateAdded": null,
  "campaignVisibility": null,
  "permissions": null,
} satisfies UserCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UserCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


