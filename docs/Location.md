
# Location


## Properties

Name | Type
------------ | -------------
`id` | number
`externalDealerId` | string
`dealer` | [Dealer](Dealer.md)
`district` | [District](District.md)
`externalLocationId` | string
`salesforceLocationId` | string
`name` | string
`addressLine1` | string
`addressLine2` | string
`city` | string
`state` | string
`zipCode` | string
`country` | string
`phone` | string
`fax` | string
`website` | string
`manager` | string
`managerPhone` | string
`managerEmail` | string
`locator` | string
`address` | string
`outlet` | string
`fullAddress` | string

## Example

```typescript
import type { Location } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "externalDealerId": null,
  "dealer": null,
  "district": null,
  "externalLocationId": null,
  "salesforceLocationId": null,
  "name": null,
  "addressLine1": null,
  "addressLine2": null,
  "city": null,
  "state": null,
  "zipCode": null,
  "country": null,
  "phone": null,
  "fax": null,
  "website": null,
  "manager": null,
  "managerPhone": null,
  "managerEmail": null,
  "locator": null,
  "address": null,
  "outlet": null,
  "fullAddress": null,
} satisfies Location

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Location
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


