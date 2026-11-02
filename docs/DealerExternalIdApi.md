# DealerExternalIdApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**dealerExternalIdCreate**](DealerExternalIdApi.md#dealerexternalidcreate) | **POST** /v4/api/dealer-external-id |  |
| [**dealerExternalIdDelete**](DealerExternalIdApi.md#dealerexternaliddelete) | **DELETE** /v4/api/dealer-external-id/{id} |  |
| [**dealerExternalIdGet**](DealerExternalIdApi.md#dealerexternalidget) | **GET** /v4/api/dealer-external-id/{id} |  |
| [**dealerExternalIdSearch**](DealerExternalIdApi.md#dealerexternalidsearch) | **GET** /v4/api/dealer-external-id |  |
| [**dealerExternalIdUpdate**](DealerExternalIdApi.md#dealerexternalidupdate) | **PUT** /v4/api/dealer-external-id/{id} |  |



## dealerExternalIdCreate

> DealerExternalId dealerExternalIdCreate(dealerExternalIdCreate)



Create a Dealer External id.

### Example

```ts
import {
  Configuration,
  DealerExternalIdApi,
} from '@statflo/statflo-typescript-sdk';
import type { DealerExternalIdCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DealerExternalIdApi(config);

  const body = {
    // DealerExternalIdCreate (optional)
    dealerExternalIdCreate: ...,
  } satisfies DealerExternalIdCreateRequest;

  try {
    const data = await api.dealerExternalIdCreate(body);
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
| **dealerExternalIdCreate** | [DealerExternalIdCreate](DealerExternalIdCreate.md) |  | [Optional] |

### Return type

[**DealerExternalId**](DealerExternalId.md)

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


## dealerExternalIdDelete

> dealerExternalIdDelete(id)



Remove a Dealer External id.

### Example

```ts
import {
  Configuration,
  DealerExternalIdApi,
} from '@statflo/statflo-typescript-sdk';
import type { DealerExternalIdDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DealerExternalIdApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies DealerExternalIdDeleteRequest;

  try {
    const data = await api.dealerExternalIdDelete(body);
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


## dealerExternalIdGet

> DealerExternalId dealerExternalIdGet(id)



Retrieve a Dealer External id.

### Example

```ts
import {
  Configuration,
  DealerExternalIdApi,
} from '@statflo/statflo-typescript-sdk';
import type { DealerExternalIdGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DealerExternalIdApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies DealerExternalIdGetRequest;

  try {
    const data = await api.dealerExternalIdGet(body);
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

[**DealerExternalId**](DealerExternalId.md)

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


## dealerExternalIdSearch

> DealerExternalIdPaginationResponse dealerExternalIdSearch(filter, query, page, perPage, sort)



Search Dealer External ids.

### Example

```ts
import {
  Configuration,
  DealerExternalIdApi,
} from '@statflo/statflo-typescript-sdk';
import type { DealerExternalIdSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DealerExternalIdApi(config);

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
  } satisfies DealerExternalIdSearchRequest;

  try {
    const data = await api.dealerExternalIdSearch(body);
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

[**DealerExternalIdPaginationResponse**](DealerExternalIdPaginationResponse.md)

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


## dealerExternalIdUpdate

> DealerExternalId dealerExternalIdUpdate(id, dealerExternalIdUpdate)



Update a Dealer External id.

### Example

```ts
import {
  Configuration,
  DealerExternalIdApi,
} from '@statflo/statflo-typescript-sdk';
import type { DealerExternalIdUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DealerExternalIdApi(config);

  const body = {
    // string
    id: id_example,
    // DealerExternalIdUpdate (optional)
    dealerExternalIdUpdate: ...,
  } satisfies DealerExternalIdUpdateRequest;

  try {
    const data = await api.dealerExternalIdUpdate(body);
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
| **dealerExternalIdUpdate** | [DealerExternalIdUpdate](DealerExternalIdUpdate.md) |  | [Optional] |

### Return type

[**DealerExternalId**](DealerExternalId.md)

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

