
# RoleUpdate


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`displayInApp` | boolean
`order` | number
`restrictBySalesRepId` | boolean
`restrictByOutletId` | boolean
`restrictByRegionId` | boolean
`restrictByDistrictId` | boolean
`linkedFeatureFlag` | number

## Example

```typescript
import type { RoleUpdate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "name": null,
  "displayInApp": null,
  "order": null,
  "restrictBySalesRepId": null,
  "restrictByOutletId": null,
  "restrictByRegionId": null,
  "restrictByDistrictId": null,
  "linkedFeatureFlag": null,
} satisfies RoleUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RoleUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


