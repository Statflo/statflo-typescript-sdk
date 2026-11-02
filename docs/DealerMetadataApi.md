# DealerMetadataApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**dealerMetadataCreate**](DealerMetadataApi.md#dealermetadatacreate) | **POST** /v4/api/dealer-metadata |  |
| [**dealerMetadataDelete**](DealerMetadataApi.md#dealermetadatadelete) | **DELETE** /v4/api/dealer-metadata/{id} |  |
| [**dealerMetadataGet**](DealerMetadataApi.md#dealermetadataget) | **GET** /v4/api/dealer-metadata/{id} |  |
| [**dealerMetadataSearch**](DealerMetadataApi.md#dealermetadatasearch) | **GET** /v4/api/dealer-metadata |  |
| [**dealerMetadataUpdate**](DealerMetadataApi.md#dealermetadataupdate) | **PUT** /v4/api/dealer-metadata/{id} |  |



## dealerMetadataCreate

> DealerMetadata dealerMetadataCreate(dealerMetadataCreate)



Create a dealer metadata.

### Example

```ts
import {
  Configuration,
  DealerMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { DealerMetadataCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DealerMetadataApi(config);

  const body = {
    // DealerMetadataCreate (optional)
    dealerMetadataCreate: ...,
  } satisfies DealerMetadataCreateRequest;

  try {
    const data = await api.dealerMetadataCreate(body);
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
| **dealerMetadataCreate** | [DealerMetadataCreate](DealerMetadataCreate.md) |  | [Optional] |

### Return type

[**DealerMetadata**](DealerMetadata.md)

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


## dealerMetadataDelete

> dealerMetadataDelete(id)



Remove a dealer metadata.

### Example

```ts
import {
  Configuration,
  DealerMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { DealerMetadataDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DealerMetadataApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies DealerMetadataDeleteRequest;

  try {
    const data = await api.dealerMetadataDelete(body);
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


## dealerMetadataGet

> DealerMetadata dealerMetadataGet(id)



Retrieve a dealer metadata.

### Example

```ts
import {
  Configuration,
  DealerMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { DealerMetadataGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DealerMetadataApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies DealerMetadataGetRequest;

  try {
    const data = await api.dealerMetadataGet(body);
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

[**DealerMetadata**](DealerMetadata.md)

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


## dealerMetadataSearch

> DealerMetadataPaginationResponse dealerMetadataSearch(filter, query, page, perPage, sort)



Search dealer metadata.

### Example

```ts
import {
  Configuration,
  DealerMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { DealerMetadataSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DealerMetadataApi(config);

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
  } satisfies DealerMetadataSearchRequest;

  try {
    const data = await api.dealerMetadataSearch(body);
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

[**DealerMetadataPaginationResponse**](DealerMetadataPaginationResponse.md)

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


## dealerMetadataUpdate

> DealerMetadata dealerMetadataUpdate(id, dealerMetadataUpdate)



Update a dealer metadata.

### Example

```ts
import {
  Configuration,
  DealerMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { DealerMetadataUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DealerMetadataApi(config);

  const body = {
    // string
    id: id_example,
    // DealerMetadataUpdate (optional)
    dealerMetadataUpdate: ...,
  } satisfies DealerMetadataUpdateRequest;

  try {
    const data = await api.dealerMetadataUpdate(body);
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
| **dealerMetadataUpdate** | [DealerMetadataUpdate](DealerMetadataUpdate.md) |  | [Optional] |

### Return type

[**DealerMetadata**](DealerMetadata.md)

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

