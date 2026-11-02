
# CarrierCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`country` | string
`logo` | string

## Example

```typescript
import type { CarrierCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "name": null,
  "country": null,
  "logo": null,
} satisfies CarrierCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as CarrierCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


