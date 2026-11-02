
# Dealer


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`countryCode` | string
`calendarFormat` | number
`status` | [DealerStatus](DealerStatus.md)
`website` | string
`addressLine1` | string
`addressLine2` | string
`city` | string
`province` | string
`postalCode` | string
`carrier` | [Carrier](Carrier.md)
`permissions` | [Array&lt;Permission&gt;](Permission.md)
`dealerFeatures` | [Array&lt;DealerAllowedFeature&gt;](DealerAllowedFeature.md)
`features` | Array&lt;number&gt;

## Example

```typescript
import type { Dealer } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "name": null,
  "countryCode": null,
  "calendarFormat": null,
  "status": null,
  "website": null,
  "addressLine1": null,
  "addressLine2": null,
  "city": null,
  "province": null,
  "postalCode": null,
  "carrier": null,
  "permissions": null,
  "dealerFeatures": null,
  "features": null,
} satisfies Dealer

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Dealer
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


