
# UserMetadata


## Properties

Name | Type
------------ | -------------
`id` | number
`user` | [User](User.md)
`metadata` | string
`value` | string
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { UserMetadata } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "user": null,
  "metadata": null,
  "value": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies UserMetadata

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UserMetadata
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


