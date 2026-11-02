
# User


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
`phoneNumber` | string
`timezone` | string
`theme` | number
`userActive` | boolean
`inboundAvailable` | boolean
`jobTitle` | string
`acceptedTermsConditions` | boolean
`appointmentReminderEmail` | boolean
`dealer` | [Dealer](Dealer.md)
`carrier` | [Carrier](Carrier.md)
`role` | [Role](Role.md)
`userPermissions` | [Array&lt;UserPermission&gt;](UserPermission.md)
`userTeams` | [Array&lt;UserTeam&gt;](UserTeam.md)
`userMetadata` | [Array&lt;UserMetadata&gt;](UserMetadata.md)
`dateAdded` | Date
`campaignVisibility` | number
`permissions` | Array&lt;number&gt;

## Example

```typescript
import type { User } from '@statflo/statflo-typescript-sdk'

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
  "phoneNumber": null,
  "timezone": null,
  "theme": null,
  "userActive": null,
  "inboundAvailable": null,
  "jobTitle": null,
  "acceptedTermsConditions": null,
  "appointmentReminderEmail": null,
  "dealer": null,
  "carrier": null,
  "role": null,
  "userPermissions": null,
  "userTeams": null,
  "userMetadata": null,
  "dateAdded": null,
  "campaignVisibility": null,
  "permissions": null,
} satisfies User

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as User
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


