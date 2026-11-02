
# RcsAgentMetadataCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`rcsAgentId` | number
`metadata` | string
`value` | object
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { RcsAgentMetadataCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "rcsAgentId": null,
  "metadata": null,
  "value": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies RcsAgentMetadataCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RcsAgentMetadataCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


