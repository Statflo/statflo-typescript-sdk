
# AccountNumberCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`location` | string
`userId` | number
`phoneNumber` | string

## Example

```typescript
import type { AccountNumberCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "location": null,
  "userId": null,
  "phoneNumber": null,
} satisfies AccountNumberCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as AccountNumberCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


