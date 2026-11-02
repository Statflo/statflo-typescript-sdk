
# RcsAgentBusinessCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`industry` | string
`legalName` | string
`entityType` | string
`stockExchange` | string
`stockSymbol` | string
`registrationNumber` | string
`registrationIssuingCountryIsoCode` | string
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { RcsAgentBusinessCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "industry": null,
  "legalName": null,
  "entityType": null,
  "stockExchange": null,
  "stockSymbol": null,
  "registrationNumber": null,
  "registrationIssuingCountryIsoCode": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies RcsAgentBusinessCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RcsAgentBusinessCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


