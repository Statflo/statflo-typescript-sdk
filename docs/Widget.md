
# Widget


## Properties

Name | Type
------------ | -------------
`id` | number
`carrier` | [Carrier](Carrier.md)
`dealer` | [Dealer](Dealer.md)
`name` | string
`label` | string
`url` | string
`type` | string
`priority` | number
`metadata` | [Array&lt;WidgetMetadata&gt;](WidgetMetadata.md)

## Example

```typescript
import type { Widget } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "carrier": null,
  "dealer": null,
  "name": null,
  "label": null,
  "url": null,
  "type": null,
  "priority": null,
  "metadata": null,
} satisfies Widget

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as Widget
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


