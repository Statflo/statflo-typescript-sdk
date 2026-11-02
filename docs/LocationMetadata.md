
# LocationMetadata


## Properties

Name | Type
------------ | -------------
`id` | number
`dealer` | [Dealer](Dealer.md)
`location` | [Location](Location.md)
`metadata` | string
`value` | object

## Example

```typescript
import type { LocationMetadata } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "dealer": null,
  "location": null,
  "metadata": null,
  "value": null,
} satisfies LocationMetadata

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as LocationMetadata
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


