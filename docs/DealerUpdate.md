
# DealerUpdate


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`countryCode` | string
`calendarFormat` | number
`website` | string
`addressLine1` | string
`addressLine2` | string
`city` | string
`province` | string
`postalCode` | string
`features` | Array&lt;number&gt;

## Example

```typescript
import type { DealerUpdate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "name": null,
  "countryCode": null,
  "calendarFormat": null,
  "website": null,
  "addressLine1": null,
  "addressLine2": null,
  "city": null,
  "province": null,
  "postalCode": null,
  "features": null,
} satisfies DealerUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as DealerUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


