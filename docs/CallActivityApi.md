# CallActivityApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**callActivityCreate**](CallActivityApi.md#callactivitycreate) | **POST** /v4/api/call-activity |  |
| [**callActivityDelete**](CallActivityApi.md#callactivitydelete) | **DELETE** /v4/api/call-activity/{id} |  |
| [**callActivityGet**](CallActivityApi.md#callactivityget) | **GET** /v4/api/call-activity/{id} |  |
| [**callActivitySearch**](CallActivityApi.md#callactivitysearch) | **GET** /v4/api/call-activity |  |
| [**callActivityUpdate**](CallActivityApi.md#callactivityupdate) | **PUT** /v4/api/call-activity/{id} |  |



## callActivityCreate

> CallActivity callActivityCreate(callActivityCreate)



Create a call activity.

### Example

```ts
import {
  Configuration,
  CallActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { CallActivityCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CallActivityApi(config);

  const body = {
    // CallActivityCreate (optional)
    callActivityCreate: ...,
  } satisfies CallActivityCreateRequest;

  try {
    const data = await api.callActivityCreate(body);
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
| **callActivityCreate** | [CallActivityCreate](CallActivityCreate.md) |  | [Optional] |

### Return type

[**CallActivity**](CallActivity.md)

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


## callActivityDelete

> callActivityDelete(id)



Remove a call activity.

### Example

```ts
import {
  Configuration,
  CallActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { CallActivityDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CallActivityApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies CallActivityDeleteRequest;

  try {
    const data = await api.callActivityDelete(body);
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


## callActivityGet

> CallActivity callActivityGet(id)



Retrieve a call activity.

### Example

```ts
import {
  Configuration,
  CallActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { CallActivityGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CallActivityApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies CallActivityGetRequest;

  try {
    const data = await api.callActivityGet(body);
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

[**CallActivity**](CallActivity.md)

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


## callActivitySearch

> CallActivityPaginationResponse callActivitySearch(filter, query, page, perPage, sort)



Search call activities.

### Example

```ts
import {
  Configuration,
  CallActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { CallActivitySearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CallActivityApi(config);

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
  } satisfies CallActivitySearchRequest;

  try {
    const data = await api.callActivitySearch(body);
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

[**CallActivityPaginationResponse**](CallActivityPaginationResponse.md)

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


## callActivityUpdate

> CallActivity callActivityUpdate(id, callActivityUpdate)



Update a call activity.

### Example

```ts
import {
  Configuration,
  CallActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { CallActivityUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CallActivityApi(config);

  const body = {
    // string
    id: id_example,
    // CallActivityUpdate (optional)
    callActivityUpdate: ...,
  } satisfies CallActivityUpdateRequest;

  try {
    const data = await api.callActivityUpdate(body);
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
| **callActivityUpdate** | [CallActivityUpdate](CallActivityUpdate.md) |  | [Optional] |

### Return type

[**CallActivity**](CallActivity.md)

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

