# DefaultApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**postV4ApiCampaignMappingSearch**](DefaultApi.md#postv4apicampaignmappingsearch) | **POST** /v4/api/campaign-mapping |  |
| [**postV4ApiCarrierSearch**](DefaultApi.md#postv4apicarriersearch) | **POST** /v4/api/carrier |  |
| [**postV4ApiDealerSearch**](DefaultApi.md#postv4apidealersearch) | **POST** /v4/api/dealer |  |
| [**postV4ApiFeatureSearch**](DefaultApi.md#postv4apifeaturesearch) | **POST** /v4/api/feature |  |



## postV4ApiCampaignMappingSearch

> postV4ApiCampaignMappingSearch()



### Example

```ts
import {
  Configuration,
  DefaultApi,
} from '@statflo/statflo-typescript-sdk';
import type { PostV4ApiCampaignMappingSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DefaultApi(config);

  try {
    const data = await api.postV4ApiCampaignMappingSearch();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

`void` (Empty response body)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## postV4ApiCarrierSearch

> postV4ApiCarrierSearch()



### Example

```ts
import {
  Configuration,
  DefaultApi,
} from '@statflo/statflo-typescript-sdk';
import type { PostV4ApiCarrierSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DefaultApi(config);

  try {
    const data = await api.postV4ApiCarrierSearch();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

`void` (Empty response body)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## postV4ApiDealerSearch

> postV4ApiDealerSearch()



### Example

```ts
import {
  Configuration,
  DefaultApi,
} from '@statflo/statflo-typescript-sdk';
import type { PostV4ApiDealerSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DefaultApi(config);

  try {
    const data = await api.postV4ApiDealerSearch();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

`void` (Empty response body)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## postV4ApiFeatureSearch

> postV4ApiFeatureSearch()



### Example

```ts
import {
  Configuration,
  DefaultApi,
} from '@statflo/statflo-typescript-sdk';
import type { PostV4ApiFeatureSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DefaultApi(config);

  try {
    const data = await api.postV4ApiFeatureSearch();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

`void` (Empty response body)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

