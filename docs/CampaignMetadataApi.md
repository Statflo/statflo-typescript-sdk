# CampaignMetadataApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**campaignMetadataCreate**](CampaignMetadataApi.md#campaignmetadatacreate) | **POST** /v4/api/campaign-metadata |  |
| [**campaignMetadataDelete**](CampaignMetadataApi.md#campaignmetadatadelete) | **DELETE** /v4/api/campaign-metadata/{id} |  |
| [**campaignMetadataGet**](CampaignMetadataApi.md#campaignmetadataget) | **GET** /v4/api/campaign-metadata/{id} |  |
| [**campaignMetadataSearch**](CampaignMetadataApi.md#campaignmetadatasearch) | **GET** /v4/api/campaign-metadata |  |
| [**campaignMetadataUpdate**](CampaignMetadataApi.md#campaignmetadataupdate) | **PUT** /v4/api/campaign-metadata/{id} |  |



## campaignMetadataCreate

> CampaignMetadata campaignMetadataCreate(campaignMetadataCreate)



Create a campaign metadata.

### Example

```ts
import {
  Configuration,
  CampaignMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignMetadataCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignMetadataApi(config);

  const body = {
    // CampaignMetadataCreate (optional)
    campaignMetadataCreate: ...,
  } satisfies CampaignMetadataCreateRequest;

  try {
    const data = await api.campaignMetadataCreate(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **campaignMetadataCreate** | [CampaignMetadataCreate](CampaignMetadataCreate.md) |  | [Optional] |

### Return type

[**CampaignMetadata**](CampaignMetadata.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
| **400** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## campaignMetadataDelete

> campaignMetadataDelete(id)



Remove a campaign metadata.

### Example

```ts
import {
  Configuration,
  CampaignMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignMetadataDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignMetadataApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies CampaignMetadataDeleteRequest;

  try {
    const data = await api.campaignMetadataDelete(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Success |  -  |
| **400** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## campaignMetadataGet

> CampaignMetadata campaignMetadataGet(id)



Retrieve a campaign metadata.

### Example

```ts
import {
  Configuration,
  CampaignMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignMetadataGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignMetadataApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies CampaignMetadataGetRequest;

  try {
    const data = await api.campaignMetadataGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | `string` |  | [Defaults to `undefined`] |

### Return type

[**CampaignMetadata**](CampaignMetadata.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
| **400** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## campaignMetadataSearch

> CampaignMetadataPaginationResponse campaignMetadataSearch(filter, query, page, perPage, sort)



Search campaign metadata.

### Example

```ts
import {
  Configuration,
  CampaignMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignMetadataSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignMetadataApi(config);

  const body = {
    // { [key: string]: any; } (optional)
    filter: Object,
    // string (optional)
    query: query_example,
    // number (optional)
    page: 56,
    // number (optional)
    perPage: 56,
    // string (optional)
    sort: sort_example,
  } satisfies CampaignMetadataSearchRequest;

  try {
    const data = await api.campaignMetadataSearch(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **filter** | `{ [key: string]: any; }` |  | [Optional] |
| **query** | `string` |  | [Optional] [Defaults to `undefined`] |
| **page** | `number` |  | [Optional] [Defaults to `undefined`] |
| **perPage** | `number` |  | [Optional] [Defaults to `undefined`] |
| **sort** | `string` |  | [Optional] [Defaults to `undefined`] |

### Return type

[**CampaignMetadataPaginationResponse**](CampaignMetadataPaginationResponse.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
| **400** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## campaignMetadataUpdate

> CampaignMetadata campaignMetadataUpdate(id, campaignMetadataUpdate)



Update a campaign metadata.

### Example

```ts
import {
  Configuration,
  CampaignMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignMetadataUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignMetadataApi(config);

  const body = {
    // string
    id: id_example,
    // CampaignMetadataUpdate (optional)
    campaignMetadataUpdate: ...,
  } satisfies CampaignMetadataUpdateRequest;

  try {
    const data = await api.campaignMetadataUpdate(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **id** | `string` |  | [Defaults to `undefined`] |
| **campaignMetadataUpdate** | [CampaignMetadataUpdate](CampaignMetadataUpdate.md) |  | [Optional] |

### Return type

[**CampaignMetadata**](CampaignMetadata.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
| **400** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

