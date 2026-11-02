# RegionApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**regionCreate**](RegionApi.md#regioncreate) | **POST** /v4/api/region |  |
| [**regionDelete**](RegionApi.md#regiondelete) | **DELETE** /v4/api/region/{id} |  |
| [**regionGet**](RegionApi.md#regionget) | **GET** /v4/api/region/{id} |  |
| [**regionSearch**](RegionApi.md#regionsearch) | **GET** /v4/api/region |  |
| [**regionUpdate**](RegionApi.md#regionupdate) | **PUT** /v4/api/region/{id} |  |



## regionCreate

> Region regionCreate(regionCreate)



Create a region.

### Example

```ts
import {
  Configuration,
  RegionApi,
} from '@statflo/statflo-typescript-sdk';
import type { RegionCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RegionApi(config);

  const body = {
    // RegionCreate (optional)
    regionCreate: ...,
  } satisfies RegionCreateRequest;

  try {
    const data = await api.regionCreate(body);
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
| **regionCreate** | [RegionCreate](RegionCreate.md) |  | [Optional] |

### Return type

[**Region**](Region.md)

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


## regionDelete

> regionDelete(id)



Remove a region.

### Example

```ts
import {
  Configuration,
  RegionApi,
} from '@statflo/statflo-typescript-sdk';
import type { RegionDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RegionApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies RegionDeleteRequest;

  try {
    const data = await api.regionDelete(body);
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
| **409** | Conflict |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## regionGet

> Region regionGet(id)



Retrieve a region.

### Example

```ts
import {
  Configuration,
  RegionApi,
} from '@statflo/statflo-typescript-sdk';
import type { RegionGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RegionApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies RegionGetRequest;

  try {
    const data = await api.regionGet(body);
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

[**Region**](Region.md)

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


## regionSearch

> RegionPaginationResponse regionSearch(filter, query, page, perPage, sort)



Search regions.

### Example

```ts
import {
  Configuration,
  RegionApi,
} from '@statflo/statflo-typescript-sdk';
import type { RegionSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RegionApi(config);

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
  } satisfies RegionSearchRequest;

  try {
    const data = await api.regionSearch(body);
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

[**RegionPaginationResponse**](RegionPaginationResponse.md)

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


## regionUpdate

> Region regionUpdate(id, regionUpdate)



Update a district.

### Example

```ts
import {
  Configuration,
  RegionApi,
} from '@statflo/statflo-typescript-sdk';
import type { RegionUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RegionApi(config);

  const body = {
    // string
    id: id_example,
    // RegionUpdate (optional)
    regionUpdate: ...,
  } satisfies RegionUpdateRequest;

  try {
    const data = await api.regionUpdate(body);
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
| **regionUpdate** | [RegionUpdate](RegionUpdate.md) |  | [Optional] |

### Return type

[**Region**](Region.md)

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

