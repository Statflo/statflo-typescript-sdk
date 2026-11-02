
# Carrier


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`country` | string
`logo` | string
`dealers` | [Array&lt;Dealer&gt;](Dealer.md)
`brands` | [Array&lt;Brand&gt;](Brand.md)

## Example

```typescript
import type { Carrier } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "name": null,
  "country": null,
  "logo": null,
  "dealers": null,
  "brands": null,
} satisfies Carrier

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Carrier
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


