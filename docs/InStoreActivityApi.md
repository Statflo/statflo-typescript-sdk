# InStoreActivityApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**inStoreActivityCreate**](InStoreActivityApi.md#instoreactivitycreate) | **POST** /v4/api/in-store-activity |  |
| [**inStoreActivityDelete**](InStoreActivityApi.md#instoreactivitydelete) | **DELETE** /v4/api/in-store-activity/{id} |  |
| [**inStoreActivityGet**](InStoreActivityApi.md#instoreactivityget) | **GET** /v4/api/in-store-activity/{id} |  |
| [**inStoreActivitySearch**](InStoreActivityApi.md#instoreactivitysearch) | **GET** /v4/api/in-store-activity |  |
| [**inStoreActivityUpdate**](InStoreActivityApi.md#instoreactivityupdate) | **PUT** /v4/api/in-store-activity/{id} |  |



## inStoreActivityCreate

> InStoreActivity inStoreActivityCreate(inStoreActivityCreate)



Create an in-store activity.

### Example

```ts
import {
  Configuration,
  InStoreActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { InStoreActivityCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InStoreActivityApi(config);

  const body = {
    // InStoreActivityCreate (optional)
    inStoreActivityCreate: ...,
  } satisfies InStoreActivityCreateRequest;

  try {
    const data = await api.inStoreActivityCreate(body);
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
| **inStoreActivityCreate** | [InStoreActivityCreate](InStoreActivityCreate.md) |  | [Optional] |

### Return type

[**InStoreActivity**](InStoreActivity.md)

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


## inStoreActivityDelete

> inStoreActivityDelete(id)



Remove an in-store activity.

### Example

```ts
import {
  Configuration,
  InStoreActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { InStoreActivityDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InStoreActivityApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies InStoreActivityDeleteRequest;

  try {
    const data = await api.inStoreActivityDelete(body);
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


## inStoreActivityGet

> InStoreActivity inStoreActivityGet(id)



Retrieve an in-store activity.

### Example

```ts
import {
  Configuration,
  InStoreActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { InStoreActivityGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InStoreActivityApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies InStoreActivityGetRequest;

  try {
    const data = await api.inStoreActivityGet(body);
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

[**InStoreActivity**](InStoreActivity.md)

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


## inStoreActivitySearch

> InStoreActivityPaginationResponse inStoreActivitySearch(filter, query, page, perPage, sort)



Search in-store activities.

### Example

```ts
import {
  Configuration,
  InStoreActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { InStoreActivitySearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InStoreActivityApi(config);

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
  } satisfies InStoreActivitySearchRequest;

  try {
    const data = await api.inStoreActivitySearch(body);
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

[**InStoreActivityPaginationResponse**](InStoreActivityPaginationResponse.md)

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


## inStoreActivityUpdate

> InStoreActivity inStoreActivityUpdate(id, inStoreActivityUpdate)



Update an in-store activity.

### Example

```ts
import {
  Configuration,
  InStoreActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { InStoreActivityUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new InStoreActivityApi(config);

  const body = {
    // string
    id: id_example,
    // InStoreActivityUpdate (optional)
    inStoreActivityUpdate: ...,
  } satisfies InStoreActivityUpdateRequest;

  try {
    const data = await api.inStoreActivityUpdate(body);
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
| **inStoreActivityUpdate** | [InStoreActivityUpdate](InStoreActivityUpdate.md) |  | [Optional] |

### Return type

[**InStoreActivity**](InStoreActivity.md)

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

