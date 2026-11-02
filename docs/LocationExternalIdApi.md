# LocationExternalIdApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**locationExternalIdCreate**](LocationExternalIdApi.md#locationexternalidcreate) | **POST** /v4/api/location-external-id |  |
| [**locationExternalIdDelete**](LocationExternalIdApi.md#locationexternaliddelete) | **DELETE** /v4/api/location-external-id/{id} |  |
| [**locationExternalIdGet**](LocationExternalIdApi.md#locationexternalidget) | **GET** /v4/api/location-external-id/{id} |  |
| [**locationExternalIdSearch**](LocationExternalIdApi.md#locationexternalidsearch) | **GET** /v4/api/location-external-id |  |
| [**locationExternalIdUpdate**](LocationExternalIdApi.md#locationexternalidupdate) | **PUT** /v4/api/location-external-id/{id} |  |



## locationExternalIdCreate

> LocationExternalId locationExternalIdCreate(locationExternalIdCreate)



Create a location external id.

### Example

```ts
import {
  Configuration,
  LocationExternalIdApi,
} from '@statflo/statflo-typescript-sdk';
import type { LocationExternalIdCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LocationExternalIdApi(config);

  const body = {
    // LocationExternalIdCreate (optional)
    locationExternalIdCreate: ...,
  } satisfies LocationExternalIdCreateRequest;

  try {
    const data = await api.locationExternalIdCreate(body);
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
| **locationExternalIdCreate** | [LocationExternalIdCreate](LocationExternalIdCreate.md) |  | [Optional] |

### Return type

[**LocationExternalId**](LocationExternalId.md)

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


## locationExternalIdDelete

> locationExternalIdDelete(id)



Remove a location external id.

### Example

```ts
import {
  Configuration,
  LocationExternalIdApi,
} from '@statflo/statflo-typescript-sdk';
import type { LocationExternalIdDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LocationExternalIdApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies LocationExternalIdDeleteRequest;

  try {
    const data = await api.locationExternalIdDelete(body);
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


## locationExternalIdGet

> LocationExternalId locationExternalIdGet(id)



Retrieve a location external id.

### Example

```ts
import {
  Configuration,
  LocationExternalIdApi,
} from '@statflo/statflo-typescript-sdk';
import type { LocationExternalIdGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LocationExternalIdApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies LocationExternalIdGetRequest;

  try {
    const data = await api.locationExternalIdGet(body);
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

[**LocationExternalId**](LocationExternalId.md)

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


## locationExternalIdSearch

> LocationExternalIdPaginationResponse locationExternalIdSearch(filter, query, page, perPage, sort)



Search location external ids.

### Example

```ts
import {
  Configuration,
  LocationExternalIdApi,
} from '@statflo/statflo-typescript-sdk';
import type { LocationExternalIdSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LocationExternalIdApi(config);

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
  } satisfies LocationExternalIdSearchRequest;

  try {
    const data = await api.locationExternalIdSearch(body);
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

[**LocationExternalIdPaginationResponse**](LocationExternalIdPaginationResponse.md)

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


## locationExternalIdUpdate

> LocationExternalId locationExternalIdUpdate(id, locationExternalIdUpdate)



Update a location external id.

### Example

```ts
import {
  Configuration,
  LocationExternalIdApi,
} from '@statflo/statflo-typescript-sdk';
import type { LocationExternalIdUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LocationExternalIdApi(config);

  const body = {
    // string
    id: id_example,
    // LocationExternalIdUpdate (optional)
    locationExternalIdUpdate: ...,
  } satisfies LocationExternalIdUpdateRequest;

  try {
    const data = await api.locationExternalIdUpdate(body);
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
| **locationExternalIdUpdate** | [LocationExternalIdUpdate](LocationExternalIdUpdate.md) |  | [Optional] |

### Return type

[**LocationExternalId**](LocationExternalId.md)

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

