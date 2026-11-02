
# RcsAgentBusinessPaginationResponse


## Properties

Name | Type
------------ | -------------
`items` | [Array&lt;RcsAgentBusiness&gt;](RcsAgentBusiness.md)
`pagination` | [Pagination](Pagination.md)
`aggregations` | { [key: string]: any; }

## Example

```typescript
import type { RcsAgentBusinessPaginationResponse } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "items": null,
  "pagination": null,
  "aggregations": null,
} satisfies RcsAgentBusinessPaginationResponse

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RcsAgentBusinessPaginationResponse
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


