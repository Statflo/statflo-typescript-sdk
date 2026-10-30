# CampaignActionApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**campaignActionCreate**](CampaignActionApi.md#campaignactioncreate) | **POST** /v4/api/campaign-action |  |
| [**campaignActionDelete**](CampaignActionApi.md#campaignactiondelete) | **DELETE** /v4/api/campaign-action/{id} |  |
| [**campaignActionGet**](CampaignActionApi.md#campaignactionget) | **GET** /v4/api/campaign-action/{id} |  |
| [**campaignActionSearch**](CampaignActionApi.md#campaignactionsearch) | **GET** /v4/api/campaign-action |  |
| [**campaignActionUpdate**](CampaignActionApi.md#campaignactionupdate) | **PUT** /v4/api/campaign-action/{id} |  |



## campaignActionCreate

> CampaignAction campaignActionCreate(campaignActionCreate)



Create a campaign action.

### Example

```ts
import {
  Configuration,
  CampaignActionApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignActionCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignActionApi(config);

  const body = {
    // CampaignActionCreate (optional)
    campaignActionCreate: ...,
  } satisfies CampaignActionCreateRequest;

  try {
    const data = await api.campaignActionCreate(body);
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
| **campaignActionCreate** | [CampaignActionCreate](CampaignActionCreate.md) |  | [Optional] |

### Return type

[**CampaignAction**](CampaignAction.md)

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


## campaignActionDelete

> campaignActionDelete(id)



Remove a campaign action.

### Example

```ts
import {
  Configuration,
  CampaignActionApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignActionDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignActionApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies CampaignActionDeleteRequest;

  try {
    const data = await api.campaignActionDelete(body);
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


## campaignActionGet

> CampaignAction campaignActionGet(id)



Retrieve a campaign action.

### Example

```ts
import {
  Configuration,
  CampaignActionApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignActionGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignActionApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies CampaignActionGetRequest;

  try {
    const data = await api.campaignActionGet(body);
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

[**CampaignAction**](CampaignAction.md)

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


## campaignActionSearch

> CampaignActionPaginationResponse campaignActionSearch(filter, query, page, perPage, sort)



Search campaign actions.

### Example

```ts
import {
  Configuration,
  CampaignActionApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignActionSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignActionApi(config);

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
  } satisfies CampaignActionSearchRequest;

  try {
    const data = await api.campaignActionSearch(body);
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

[**CampaignActionPaginationResponse**](CampaignActionPaginationResponse.md)

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


## campaignActionUpdate

> CampaignAction campaignActionUpdate(id, campaignActionUpdate)



Update a campaign action.

### Example

```ts
import {
  Configuration,
  CampaignActionApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignActionUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignActionApi(config);

  const body = {
    // string
    id: id_example,
    // CampaignActionUpdate (optional)
    campaignActionUpdate: ...,
  } satisfies CampaignActionUpdateRequest;

  try {
    const data = await api.campaignActionUpdate(body);
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
| **campaignActionUpdate** | [CampaignActionUpdate](CampaignActionUpdate.md) |  | [Optional] |

### Return type

[**CampaignAction**](CampaignAction.md)

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

