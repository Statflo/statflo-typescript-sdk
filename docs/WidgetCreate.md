
# WidgetCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`carrierId` | number
`dealerId` | number
`name` | string
`label` | string
`url` | string
`type` | string
`priority` | number
`nativeRemote` | string
`nativeModule` | string

## Example

```typescript
import type { WidgetCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "carrierId": null,
  "dealerId": null,
  "name": null,
  "label": null,
  "url": null,
  "type": null,
  "priority": null,
  "nativeRemote": null,
  "nativeModule": null,
} satisfies WidgetCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WidgetCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


