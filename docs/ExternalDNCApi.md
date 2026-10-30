# ExternalDNCApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**externalDncCreate**](ExternalDNCApi.md#externaldnccreate) | **POST** /v4/api/external-dnc |  |
| [**externalDncDelete**](ExternalDNCApi.md#externaldncdelete) | **DELETE** /v4/api/external-dnc/{id} |  |
| [**externalDncGet**](ExternalDNCApi.md#externaldncget) | **GET** /v4/api/external-dnc/{id} |  |
| [**externalDncSearch**](ExternalDNCApi.md#externaldncsearch) | **GET** /v4/api/external-dnc |  |
| [**externalDncUpdate**](ExternalDNCApi.md#externaldncupdate) | **PUT** /v4/api/external-dnc/{id} |  |



## externalDncCreate

> ExternalDnc externalDncCreate(externalDncCreate)



Create an external DNC.

### Example

```ts
import {
  Configuration,
  ExternalDNCApi,
} from '@statflo/statflo-typescript-sdk';
import type { ExternalDncCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ExternalDNCApi(config);

  const body = {
    // ExternalDncCreate (optional)
    externalDncCreate: ...,
  } satisfies ExternalDncCreateRequest;

  try {
    const data = await api.externalDncCreate(body);
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
| **externalDncCreate** | [ExternalDncCreate](ExternalDncCreate.md) |  | [Optional] |

### Return type

[**ExternalDnc**](ExternalDnc.md)

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


## externalDncDelete

> externalDncDelete(id)



Remove an external DNC entry.

### Example

```ts
import {
  Configuration,
  ExternalDNCApi,
} from '@statflo/statflo-typescript-sdk';
import type { ExternalDncDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ExternalDNCApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies ExternalDncDeleteRequest;

  try {
    const data = await api.externalDncDelete(body);
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


## externalDncGet

> ExternalDnc externalDncGet(id)



Retrieve an external DNC.

### Example

```ts
import {
  Configuration,
  ExternalDNCApi,
} from '@statflo/statflo-typescript-sdk';
import type { ExternalDncGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ExternalDNCApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies ExternalDncGetRequest;

  try {
    const data = await api.externalDncGet(body);
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

[**ExternalDnc**](ExternalDnc.md)

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


## externalDncSearch

> ExternalDncPaginationResponse externalDncSearch(filter, query, page, perPage, sort)



Search external DNC.

### Example

```ts
import {
  Configuration,
  ExternalDNCApi,
} from '@statflo/statflo-typescript-sdk';
import type { ExternalDncSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ExternalDNCApi(config);

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
  } satisfies ExternalDncSearchRequest;

  try {
    const data = await api.externalDncSearch(body);
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

[**ExternalDncPaginationResponse**](ExternalDncPaginationResponse.md)

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


## externalDncUpdate

> ExternalDnc externalDncUpdate(id, externalDncUpdate)



Update an external DNC.

### Example

```ts
import {
  Configuration,
  ExternalDNCApi,
} from '@statflo/statflo-typescript-sdk';
import type { ExternalDncUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ExternalDNCApi(config);

  const body = {
    // string
    id: id_example,
    // ExternalDncUpdate (optional)
    externalDncUpdate: ...,
  } satisfies ExternalDncUpdateRequest;

  try {
    const data = await api.externalDncUpdate(body);
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
| **externalDncUpdate** | [ExternalDncUpdate](ExternalDncUpdate.md) |  | [Optional] |

### Return type

[**ExternalDnc**](ExternalDnc.md)

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

