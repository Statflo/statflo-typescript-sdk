
# RcsAgentMetadata


## Properties

Name | Type
------------ | -------------
`id` | number
`rcsAgent` | [RcsAgent](RcsAgent.md)
`metadata` | string
`value` | object
`carrier` | [Carrier](Carrier.md)
`dealer` | [Dealer](Dealer.md)
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { RcsAgentMetadata } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "rcsAgent": null,
  "metadata": null,
  "value": null,
  "carrier": null,
  "dealer": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies RcsAgentMetadata

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RcsAgentMetadata
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


