# CampaignPropertyApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**campaignPropertyCreate**](CampaignPropertyApi.md#campaignpropertycreate) | **POST** /v4/api/campaign-property |  |
| [**campaignPropertyDelete**](CampaignPropertyApi.md#campaignpropertydelete) | **DELETE** /v4/api/campaign-property/{id} |  |
| [**campaignPropertyGet**](CampaignPropertyApi.md#campaignpropertyget) | **GET** /v4/api/campaign-property/{id} |  |
| [**campaignPropertySearch**](CampaignPropertyApi.md#campaignpropertysearch) | **GET** /v4/api/campaign-property |  |
| [**campaignPropertyUpdate**](CampaignPropertyApi.md#campaignpropertyupdate) | **PUT** /v4/api/campaign-property/{id} |  |



## campaignPropertyCreate

> CampaignProperty campaignPropertyCreate(campaignPropertyCreate)



Create a campaign property.

### Example

```ts
import {
  Configuration,
  CampaignPropertyApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignPropertyCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignPropertyApi(config);

  const body = {
    // CampaignPropertyCreate (optional)
    campaignPropertyCreate: ...,
  } satisfies CampaignPropertyCreateRequest;

  try {
    const data = await api.campaignPropertyCreate(body);
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
| **campaignPropertyCreate** | [CampaignPropertyCreate](CampaignPropertyCreate.md) |  | [Optional] |

### Return type

[**CampaignProperty**](CampaignProperty.md)

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


## campaignPropertyDelete

> campaignPropertyDelete(id)



Remove a campaign property.

### Example

```ts
import {
  Configuration,
  CampaignPropertyApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignPropertyDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignPropertyApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies CampaignPropertyDeleteRequest;

  try {
    const data = await api.campaignPropertyDelete(body);
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


## campaignPropertyGet

> CampaignProperty campaignPropertyGet(id)



Retrieve a campaign property.

### Example

```ts
import {
  Configuration,
  CampaignPropertyApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignPropertyGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignPropertyApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies CampaignPropertyGetRequest;

  try {
    const data = await api.campaignPropertyGet(body);
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

[**CampaignProperty**](CampaignProperty.md)

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


## campaignPropertySearch

> CampaignPropertyPaginationResponse campaignPropertySearch(filter, query, page, perPage, sort)



Search campaign properties.

### Example

```ts
import {
  Configuration,
  CampaignPropertyApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignPropertySearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignPropertyApi(config);

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
  } satisfies CampaignPropertySearchRequest;

  try {
    const data = await api.campaignPropertySearch(body);
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

[**CampaignPropertyPaginationResponse**](CampaignPropertyPaginationResponse.md)

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


## campaignPropertyUpdate

> CampaignProperty campaignPropertyUpdate(id, campaignPropertyUpdate)



Update a campaign property.

### Example

```ts
import {
  Configuration,
  CampaignPropertyApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignPropertyUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignPropertyApi(config);

  const body = {
    // string
    id: id_example,
    // CampaignPropertyUpdate (optional)
    campaignPropertyUpdate: ...,
  } satisfies CampaignPropertyUpdateRequest;

  try {
    const data = await api.campaignPropertyUpdate(body);
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
| **campaignPropertyUpdate** | [CampaignPropertyUpdate](CampaignPropertyUpdate.md) |  | [Optional] |

### Return type

[**CampaignProperty**](CampaignProperty.md)

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

