
# UserActivityLogCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`activityPerformed` | string
`dateAdded` | Date
`module` | string
`code` | string

## Example

```typescript
import type { UserActivityLogCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "activityPerformed": null,
  "dateAdded": null,
  "module": null,
  "code": null,
} satisfies UserActivityLogCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UserActivityLogCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


