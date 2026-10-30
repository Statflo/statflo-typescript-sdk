
# Team


## Properties

Name | Type
------------ | -------------
`id` | number
`name` | string
`children` | [Array&lt;Team&gt;](Team.md)
`parent` | [Team](Team.md)
`permissions` | [Array&lt;Permission&gt;](Permission.md)
`dealer` | [Dealer](Dealer.md)
`owner` | [User](User.md)
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { Team } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "name": null,
  "children": null,
  "parent": null,
  "permissions": null,
  "dealer": null,
  "owner": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies Team

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Team
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


