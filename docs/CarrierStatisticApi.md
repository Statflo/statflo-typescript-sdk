# CarrierStatisticApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**carrierStatisticCreate**](CarrierStatisticApi.md#carrierstatisticcreate) | **POST** /v4/api/carrier-statistic |  |
| [**carrierStatisticDelete**](CarrierStatisticApi.md#carrierstatisticdelete) | **DELETE** /v4/api/carrier-statistic/{id} |  |
| [**carrierStatisticGet**](CarrierStatisticApi.md#carrierstatisticget) | **GET** /v4/api/carrier-statistic/{id} |  |
| [**carrierStatisticSearch**](CarrierStatisticApi.md#carrierstatisticsearch) | **GET** /v4/api/carrier-statistic |  |
| [**carrierStatisticUpdate**](CarrierStatisticApi.md#carrierstatisticupdate) | **PUT** /v4/api/carrier-statistic/{id} |  |



## carrierStatisticCreate

> CarrierStatistic carrierStatisticCreate(carrierStatisticCreate)



Create carrier statistic.

### Example

```ts
import {
  Configuration,
  CarrierStatisticApi,
} from '@statflo/statflo-typescript-sdk';
import type { CarrierStatisticCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CarrierStatisticApi(config);

  const body = {
    // CarrierStatisticCreate (optional)
    carrierStatisticCreate: ...,
  } satisfies CarrierStatisticCreateRequest;

  try {
    const data = await api.carrierStatisticCreate(body);
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
| **carrierStatisticCreate** | [CarrierStatisticCreate](CarrierStatisticCreate.md) |  | [Optional] |

### Return type

[**CarrierStatistic**](CarrierStatistic.md)

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


## carrierStatisticDelete

> carrierStatisticDelete(id)



Remove carrier statistic.

### Example

```ts
import {
  Configuration,
  CarrierStatisticApi,
} from '@statflo/statflo-typescript-sdk';
import type { CarrierStatisticDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CarrierStatisticApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies CarrierStatisticDeleteRequest;

  try {
    const data = await api.carrierStatisticDelete(body);
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


## carrierStatisticGet

> CarrierStatistic carrierStatisticGet(id)



Retrieve carrier statistic.

### Example

```ts
import {
  Configuration,
  CarrierStatisticApi,
} from '@statflo/statflo-typescript-sdk';
import type { CarrierStatisticGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CarrierStatisticApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies CarrierStatisticGetRequest;

  try {
    const data = await api.carrierStatisticGet(body);
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

[**CarrierStatistic**](CarrierStatistic.md)

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


## carrierStatisticSearch

> CarrierStatisticPaginationResponse carrierStatisticSearch(filter, query, page, perPage, sort)



Search carrier statistic.

### Example

```ts
import {
  Configuration,
  CarrierStatisticApi,
} from '@statflo/statflo-typescript-sdk';
import type { CarrierStatisticSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CarrierStatisticApi(config);

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
  } satisfies CarrierStatisticSearchRequest;

  try {
    const data = await api.carrierStatisticSearch(body);
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

[**CarrierStatisticPaginationResponse**](CarrierStatisticPaginationResponse.md)

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


## carrierStatisticUpdate

> CarrierStatistic carrierStatisticUpdate(id, carrierStatisticUpdate)



Update carrier statistic.

### Example

```ts
import {
  Configuration,
  CarrierStatisticApi,
} from '@statflo/statflo-typescript-sdk';
import type { CarrierStatisticUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CarrierStatisticApi(config);

  const body = {
    // string
    id: id_example,
    // CarrierStatisticUpdate (optional)
    carrierStatisticUpdate: ...,
  } satisfies CarrierStatisticUpdateRequest;

  try {
    const data = await api.carrierStatisticUpdate(body);
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
| **carrierStatisticUpdate** | [CarrierStatisticUpdate](CarrierStatisticUpdate.md) |  | [Optional] |

### Return type

[**CarrierStatistic**](CarrierStatistic.md)

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

