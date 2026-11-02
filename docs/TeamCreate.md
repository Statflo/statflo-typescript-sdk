
# TeamCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`permissionIds` | Array&lt;number&gt;
`parentId` | number
`ownerId` | number
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { TeamCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "name": null,
  "permissionIds": null,
  "parentId": null,
  "ownerId": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies TeamCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as TeamCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


