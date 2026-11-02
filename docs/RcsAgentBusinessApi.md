# RcsAgentBusinessApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**rcsAgentBusinessCreate**](RcsAgentBusinessApi.md#rcsagentbusinesscreate) | **POST** /v4/api/rcs-agent-business |  |
| [**rcsAgentBusinessDelete**](RcsAgentBusinessApi.md#rcsagentbusinessdelete) | **DELETE** /v4/api/rcs-agent-business/{id} |  |
| [**rcsAgentBusinessGet**](RcsAgentBusinessApi.md#rcsagentbusinessget) | **GET** /v4/api/rcs-agent-business/{id} |  |
| [**rcsAgentBusinessSearch**](RcsAgentBusinessApi.md#rcsagentbusinesssearch) | **GET** /v4/api/rcs-agent-business |  |
| [**rcsAgentBusinessUpdate**](RcsAgentBusinessApi.md#rcsagentbusinessupdate) | **PUT** /v4/api/rcs-agent-business/{id} |  |



## rcsAgentBusinessCreate

> RcsAgentBusiness rcsAgentBusinessCreate(rcsAgentBusinessCreate)



Create an rcs agent business.

### Example

```ts
import {
  Configuration,
  RcsAgentBusinessApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentBusinessCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentBusinessApi(config);

  const body = {
    // RcsAgentBusinessCreate (optional)
    rcsAgentBusinessCreate: ...,
  } satisfies RcsAgentBusinessCreateRequest;

  try {
    const data = await api.rcsAgentBusinessCreate(body);
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
| **rcsAgentBusinessCreate** | [RcsAgentBusinessCreate](RcsAgentBusinessCreate.md) |  | [Optional] |

### Return type

[**RcsAgentBusiness**](RcsAgentBusiness.md)

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


## rcsAgentBusinessDelete

> rcsAgentBusinessDelete(id)



Remove an rcs agent business.

### Example

```ts
import {
  Configuration,
  RcsAgentBusinessApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentBusinessDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentBusinessApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies RcsAgentBusinessDeleteRequest;

  try {
    const data = await api.rcsAgentBusinessDelete(body);
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


## rcsAgentBusinessGet

> RcsAgentBusiness rcsAgentBusinessGet(id)



Retrieve an rcs agent business.

### Example

```ts
import {
  Configuration,
  RcsAgentBusinessApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentBusinessGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentBusinessApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies RcsAgentBusinessGetRequest;

  try {
    const data = await api.rcsAgentBusinessGet(body);
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

[**RcsAgentBusiness**](RcsAgentBusiness.md)

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


## rcsAgentBusinessSearch

> RcsAgentBusinessPaginationResponse rcsAgentBusinessSearch(filter, query, page, perPage, sort)



Search rcs agent businesses.

### Example

```ts
import {
  Configuration,
  RcsAgentBusinessApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentBusinessSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentBusinessApi(config);

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
  } satisfies RcsAgentBusinessSearchRequest;

  try {
    const data = await api.rcsAgentBusinessSearch(body);
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

[**RcsAgentBusinessPaginationResponse**](RcsAgentBusinessPaginationResponse.md)

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


## rcsAgentBusinessUpdate

> RcsAgentBusiness rcsAgentBusinessUpdate(id, rcsAgentBusinessUpdate)



Update an rcs agent business.

### Example

```ts
import {
  Configuration,
  RcsAgentBusinessApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentBusinessUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentBusinessApi(config);

  const body = {
    // string
    id: id_example,
    // RcsAgentBusinessUpdate (optional)
    rcsAgentBusinessUpdate: ...,
  } satisfies RcsAgentBusinessUpdateRequest;

  try {
    const data = await api.rcsAgentBusinessUpdate(body);
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
| **rcsAgentBusinessUpdate** | [RcsAgentBusinessUpdate](RcsAgentBusinessUpdate.md) |  | [Optional] |

### Return type

[**RcsAgentBusiness**](RcsAgentBusiness.md)

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

