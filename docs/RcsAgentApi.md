# RcsAgentApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**rcsAgentCreate**](RcsAgentApi.md#rcsagentcreate) | **POST** /v4/api/rcs-agent |  |
| [**rcsAgentDelete**](RcsAgentApi.md#rcsagentdelete) | **DELETE** /v4/api/rcs-agent/{id} |  |
| [**rcsAgentGet**](RcsAgentApi.md#rcsagentget) | **GET** /v4/api/rcs-agent/{id} |  |
| [**rcsAgentSearch**](RcsAgentApi.md#rcsagentsearch) | **GET** /v4/api/rcs-agent |  |
| [**rcsAgentUpdate**](RcsAgentApi.md#rcsagentupdate) | **PUT** /v4/api/rcs-agent/{id} |  |



## rcsAgentCreate

> RcsAgent rcsAgentCreate(rcsAgentCreate)



Create an rcs agent.

### Example

```ts
import {
  Configuration,
  RcsAgentApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentApi(config);

  const body = {
    // RcsAgentCreate (optional)
    rcsAgentCreate: ...,
  } satisfies RcsAgentCreateRequest;

  try {
    const data = await api.rcsAgentCreate(body);
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
| **rcsAgentCreate** | [RcsAgentCreate](RcsAgentCreate.md) |  | [Optional] |

### Return type

[**RcsAgent**](RcsAgent.md)

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


## rcsAgentDelete

> rcsAgentDelete(id)



Remove an rcs agent.

### Example

```ts
import {
  Configuration,
  RcsAgentApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies RcsAgentDeleteRequest;

  try {
    const data = await api.rcsAgentDelete(body);
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


## rcsAgentGet

> RcsAgent rcsAgentGet(id)



Retrieve an rcs agent.

### Example

```ts
import {
  Configuration,
  RcsAgentApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies RcsAgentGetRequest;

  try {
    const data = await api.rcsAgentGet(body);
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

[**RcsAgent**](RcsAgent.md)

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


## rcsAgentSearch

> RcsAgentPaginationResponse rcsAgentSearch(filter, query, page, perPage, sort)



Search rcs agents.

### Example

```ts
import {
  Configuration,
  RcsAgentApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentApi(config);

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
  } satisfies RcsAgentSearchRequest;

  try {
    const data = await api.rcsAgentSearch(body);
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

[**RcsAgentPaginationResponse**](RcsAgentPaginationResponse.md)

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


## rcsAgentUpdate

> RcsAgent rcsAgentUpdate(id, rcsAgentUpdate)



Update an rcs agent.

### Example

```ts
import {
  Configuration,
  RcsAgentApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentApi(config);

  const body = {
    // string
    id: id_example,
    // RcsAgentUpdate (optional)
    rcsAgentUpdate: ...,
  } satisfies RcsAgentUpdateRequest;

  try {
    const data = await api.rcsAgentUpdate(body);
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
| **rcsAgentUpdate** | [RcsAgentUpdate](RcsAgentUpdate.md) |  | [Optional] |

### Return type

[**RcsAgent**](RcsAgent.md)

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

