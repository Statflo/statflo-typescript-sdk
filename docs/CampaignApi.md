# CampaignApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**campaignCreate**](CampaignApi.md#campaigncreate) | **POST** /v4/api/campaign |  |
| [**campaignDelete**](CampaignApi.md#campaigndelete) | **DELETE** /v4/api/campaign/{id} |  |
| [**campaignGet**](CampaignApi.md#campaignget) | **GET** /v4/api/campaign/{id} |  |
| [**campaignSearch**](CampaignApi.md#campaignsearch) | **GET** /v4/api/campaign |  |
| [**campaignUpdate**](CampaignApi.md#campaignupdate) | **PUT** /v4/api/campaign/{id} |  |



## campaignCreate

> Campaign campaignCreate(campaignCreate)



Create a campaign.

### Example

```ts
import {
  Configuration,
  CampaignApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignApi(config);

  const body = {
    // CampaignCreate (optional)
    campaignCreate: ...,
  } satisfies CampaignCreateRequest;

  try {
    const data = await api.campaignCreate(body);
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
| **campaignCreate** | [CampaignCreate](CampaignCreate.md) |  | [Optional] |

### Return type

[**Campaign**](Campaign.md)

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


## campaignDelete

> campaignDelete(id)



Remove a campaign.

### Example

```ts
import {
  Configuration,
  CampaignApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies CampaignDeleteRequest;

  try {
    const data = await api.campaignDelete(body);
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


## campaignGet

> Campaign campaignGet(id)



Retrieve a campaign

### Example

```ts
import {
  Configuration,
  CampaignApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies CampaignGetRequest;

  try {
    const data = await api.campaignGet(body);
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

[**Campaign**](Campaign.md)

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


## campaignSearch

> CampaignPaginationResponse campaignSearch(filter, query, page, perPage, sort)



Search campaigns.

### Example

```ts
import {
  Configuration,
  CampaignApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignApi(config);

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
  } satisfies CampaignSearchRequest;

  try {
    const data = await api.campaignSearch(body);
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

[**CampaignPaginationResponse**](CampaignPaginationResponse.md)

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


## campaignUpdate

> Campaign campaignUpdate(id, campaignUpdate)



Update a campaign.

### Example

```ts
import {
  Configuration,
  CampaignApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignApi(config);

  const body = {
    // string
    id: id_example,
    // CampaignUpdate (optional)
    campaignUpdate: ...,
  } satisfies CampaignUpdateRequest;

  try {
    const data = await api.campaignUpdate(body);
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
| **campaignUpdate** | [CampaignUpdate](CampaignUpdate.md) |  | [Optional] |

### Return type

[**Campaign**](Campaign.md)

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

