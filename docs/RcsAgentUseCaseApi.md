# RcsAgentUseCaseApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**rcsAgentUseCaseCreate**](RcsAgentUseCaseApi.md#rcsagentusecasecreate) | **POST** /v4/api/rcs-agent-use-case |  |
| [**rcsAgentUseCaseDelete**](RcsAgentUseCaseApi.md#rcsagentusecasedelete) | **DELETE** /v4/api/rcs-agent-use-case/{id} |  |
| [**rcsAgentUseCaseGet**](RcsAgentUseCaseApi.md#rcsagentusecaseget) | **GET** /v4/api/rcs-agent-use-case/{id} |  |
| [**rcsAgentUseCaseSearch**](RcsAgentUseCaseApi.md#rcsagentusecasesearch) | **GET** /v4/api/rcs-agent-use-case |  |
| [**rcsAgentUseCaseUpdate**](RcsAgentUseCaseApi.md#rcsagentusecaseupdate) | **PUT** /v4/api/rcs-agent-use-case/{id} |  |



## rcsAgentUseCaseCreate

> RcsAgentUseCase rcsAgentUseCaseCreate(rcsAgentUseCaseCreate)



Create an rcs agent use case.

### Example

```ts
import {
  Configuration,
  RcsAgentUseCaseApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentUseCaseCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentUseCaseApi(config);

  const body = {
    // RcsAgentUseCaseCreate (optional)
    rcsAgentUseCaseCreate: ...,
  } satisfies RcsAgentUseCaseCreateRequest;

  try {
    const data = await api.rcsAgentUseCaseCreate(body);
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
| **rcsAgentUseCaseCreate** | [RcsAgentUseCaseCreate](RcsAgentUseCaseCreate.md) |  | [Optional] |

### Return type

[**RcsAgentUseCase**](RcsAgentUseCase.md)

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


## rcsAgentUseCaseDelete

> rcsAgentUseCaseDelete(id)



Remove an rcs agent use case.

### Example

```ts
import {
  Configuration,
  RcsAgentUseCaseApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentUseCaseDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentUseCaseApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies RcsAgentUseCaseDeleteRequest;

  try {
    const data = await api.rcsAgentUseCaseDelete(body);
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


## rcsAgentUseCaseGet

> RcsAgentUseCase rcsAgentUseCaseGet(id)



Retrieve an rcs agent use case.

### Example

```ts
import {
  Configuration,
  RcsAgentUseCaseApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentUseCaseGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentUseCaseApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies RcsAgentUseCaseGetRequest;

  try {
    const data = await api.rcsAgentUseCaseGet(body);
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

[**RcsAgentUseCase**](RcsAgentUseCase.md)

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


## rcsAgentUseCaseSearch

> RcsAgentUseCasePaginationResponse rcsAgentUseCaseSearch(filter, query, page, perPage, sort)



Search rcs agent use cases.

### Example

```ts
import {
  Configuration,
  RcsAgentUseCaseApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentUseCaseSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentUseCaseApi(config);

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
  } satisfies RcsAgentUseCaseSearchRequest;

  try {
    const data = await api.rcsAgentUseCaseSearch(body);
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

[**RcsAgentUseCasePaginationResponse**](RcsAgentUseCasePaginationResponse.md)

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


## rcsAgentUseCaseUpdate

> RcsAgentUseCase rcsAgentUseCaseUpdate(id, rcsAgentUseCaseUpdate)



Update an rcs agent use case.

### Example

```ts
import {
  Configuration,
  RcsAgentUseCaseApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentUseCaseUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentUseCaseApi(config);

  const body = {
    // string
    id: id_example,
    // RcsAgentUseCaseUpdate (optional)
    rcsAgentUseCaseUpdate: ...,
  } satisfies RcsAgentUseCaseUpdateRequest;

  try {
    const data = await api.rcsAgentUseCaseUpdate(body);
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
| **rcsAgentUseCaseUpdate** | [RcsAgentUseCaseUpdate](RcsAgentUseCaseUpdate.md) |  | [Optional] |

### Return type

[**RcsAgentUseCase**](RcsAgentUseCase.md)

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

