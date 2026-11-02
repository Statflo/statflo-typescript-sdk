
# WidgetMetadataCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`widgetId` | number
`metadata` | string
`value` | object

## Example

```typescript
import type { WidgetMetadataCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "widgetId": null,
  "metadata": null,
  "value": null,
} satisfies WidgetMetadataCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as WidgetMetadataCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


