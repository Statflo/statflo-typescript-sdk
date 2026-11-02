# LocationMetadataApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**locationMetadataCreate**](LocationMetadataApi.md#locationmetadatacreate) | **POST** /v4/api/location-metadata |  |
| [**locationMetadataDelete**](LocationMetadataApi.md#locationmetadatadelete) | **DELETE** /v4/api/location-metadata/{id} |  |
| [**locationMetadataGet**](LocationMetadataApi.md#locationmetadataget) | **GET** /v4/api/location-metadata/{id} |  |
| [**locationMetadataSearch**](LocationMetadataApi.md#locationmetadatasearch) | **GET** /v4/api/location-metadata |  |
| [**locationMetadataUpdate**](LocationMetadataApi.md#locationmetadataupdate) | **PUT** /v4/api/location-metadata/{id} |  |



## locationMetadataCreate

> LocationMetadata locationMetadataCreate(locationMetadataCreate)



Create location metadata.

### Example

```ts
import {
  Configuration,
  LocationMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { LocationMetadataCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LocationMetadataApi(config);

  const body = {
    // LocationMetadataCreate (optional)
    locationMetadataCreate: ...,
  } satisfies LocationMetadataCreateRequest;

  try {
    const data = await api.locationMetadataCreate(body);
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
| **locationMetadataCreate** | [LocationMetadataCreate](LocationMetadataCreate.md) |  | [Optional] |

### Return type

[**LocationMetadata**](LocationMetadata.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
| **422** | Validation error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## locationMetadataDelete

> locationMetadataDelete(id)



Remove location metadata.

### Example

```ts
import {
  Configuration,
  LocationMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { LocationMetadataDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LocationMetadataApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies LocationMetadataDeleteRequest;

  try {
    const data = await api.locationMetadataDelete(body);
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
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## locationMetadataGet

> LocationMetadata locationMetadataGet(id)



Retrieve location metadata.

### Example

```ts
import {
  Configuration,
  LocationMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { LocationMetadataGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LocationMetadataApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies LocationMetadataGetRequest;

  try {
    const data = await api.locationMetadataGet(body);
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

[**LocationMetadata**](LocationMetadata.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
| **404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## locationMetadataSearch

> LocationMetadataPaginationResponse locationMetadataSearch(filter, query, page, perPage, sort)



Search location metadata.

### Example

```ts
import {
  Configuration,
  LocationMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { LocationMetadataSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LocationMetadataApi(config);

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
  } satisfies LocationMetadataSearchRequest;

  try {
    const data = await api.locationMetadataSearch(body);
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

[**LocationMetadataPaginationResponse**](LocationMetadataPaginationResponse.md)

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


## locationMetadataUpdate

> LocationMetadata locationMetadataUpdate(id, locationMetadataUpdate)



Update location metadata.

### Example

```ts
import {
  Configuration,
  LocationMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { LocationMetadataUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LocationMetadataApi(config);

  const body = {
    // string
    id: id_example,
    // LocationMetadataUpdate (optional)
    locationMetadataUpdate: ...,
  } satisfies LocationMetadataUpdateRequest;

  try {
    const data = await api.locationMetadataUpdate(body);
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
| **locationMetadataUpdate** | [LocationMetadataUpdate](LocationMetadataUpdate.md) |  | [Optional] |

### Return type

[**LocationMetadata**](LocationMetadata.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |
| **422** | Validation error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

