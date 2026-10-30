
# RcsAgentUseCaseCreate


## Properties

Name | Type
------------ | -------------
`id` | number
`organicWebsiteTrafficMonthly` | number
`hasExistingShortCodeTraffic` | boolean
`existingShortCodeNumber` | string
`existingShortCodeTrafficMonthly` | number
`rbmTrafficForecastMonthly` | number
`campaignOverview` | string
`messagingFlow` | string
`helpSampleMessage` | string
`stopSampleMessage` | string
`messageServiceType` | string
`accessInstructions` | string
`optInDescription` | string
`optOutDescription` | string
`screenshotUrls` | Array&lt;string&gt;
`triggerEventDescription` | string
`description` | string
`videoUrls` | Array&lt;string&gt;
`createdAt` | Date
`updatedAt` | Date

## Example

```typescript
import type { RcsAgentUseCaseCreate } from '@statflo/statflo-typescript-sdk'

// TODO: Update the object below with actual values
const example = {
  "id": null,
  "organicWebsiteTrafficMonthly": null,
  "hasExistingShortCodeTraffic": null,
  "existingShortCodeNumber": null,
  "existingShortCodeTrafficMonthly": null,
  "rbmTrafficForecastMonthly": null,
  "campaignOverview": null,
  "messagingFlow": null,
  "helpSampleMessage": null,
  "stopSampleMessage": null,
  "messageServiceType": null,
  "accessInstructions": null,
  "optInDescription": null,
  "optOutDescription": null,
  "screenshotUrls": null,
  "triggerEventDescription": null,
  "description": null,
  "videoUrls": null,
  "createdAt": null,
  "updatedAt": null,
} satisfies RcsAgentUseCaseCreate

console.log(example)

// Convert the instance to a JSON string
const exampleJSON: string = JSON.stringify(example)
console.log(exampleJSON)

// Parse the JSON string back to an object
const exampleParsed = JSON.parse(exampleJSON) as RcsAgentUseCaseCreate
console.log(exampleParsed)
```

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


