
# UserActivityLogUpdate


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
import type { UserActivityLogUpdate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "activityPerformed": null,
  "dateAdded": null,
  "module": null,
  "code": null,
} satisfies UserActivityLogUpdate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as UserActivityLogUpdate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


