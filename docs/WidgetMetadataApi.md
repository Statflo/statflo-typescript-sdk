# WidgetMetadataApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**widgetMetadataCreate**](WidgetMetadataApi.md#widgetmetadatacreate) | **POST** /v4/api/widget-metadata |  |
| [**widgetMetadataDelete**](WidgetMetadataApi.md#widgetmetadatadelete) | **DELETE** /v4/api/widget-metadata/{id} |  |
| [**widgetMetadataGet**](WidgetMetadataApi.md#widgetmetadataget) | **GET** /v4/api/widget-metadata/{id} |  |
| [**widgetMetadataSearch**](WidgetMetadataApi.md#widgetmetadatasearch) | **GET** /v4/api/widget-metadata |  |
| [**widgetMetadataUpdate**](WidgetMetadataApi.md#widgetmetadataupdate) | **PUT** /v4/api/widget-metadata/{id} |  |



## widgetMetadataCreate

> WidgetMetadata widgetMetadataCreate(widgetMetadataCreate)



Create a widget metadata.

### Example

```ts
import {
  Configuration,
  WidgetMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { WidgetMetadataCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WidgetMetadataApi(config);

  const body = {
    // WidgetMetadataCreate (optional)
    widgetMetadataCreate: ...,
  } satisfies WidgetMetadataCreateRequest;

  try {
    const data = await api.widgetMetadataCreate(body);
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
| **widgetMetadataCreate** | [WidgetMetadataCreate](WidgetMetadataCreate.md) |  | [Optional] |

### Return type

[**WidgetMetadata**](WidgetMetadata.md)

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


## widgetMetadataDelete

> widgetMetadataDelete(id)



Remove a widget metadata.

### Example

```ts
import {
  Configuration,
  WidgetMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { WidgetMetadataDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WidgetMetadataApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies WidgetMetadataDeleteRequest;

  try {
    const data = await api.widgetMetadataDelete(body);
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


## widgetMetadataGet

> WidgetMetadata widgetMetadataGet(id)



Retrieve a widget metadata.

### Example

```ts
import {
  Configuration,
  WidgetMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { WidgetMetadataGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WidgetMetadataApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies WidgetMetadataGetRequest;

  try {
    const data = await api.widgetMetadataGet(body);
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

[**WidgetMetadata**](WidgetMetadata.md)

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


## widgetMetadataSearch

> WidgetMetadataPaginationResponse widgetMetadataSearch(filter, query, page, perPage, sort)



Search widget metadata.

### Example

```ts
import {
  Configuration,
  WidgetMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { WidgetMetadataSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WidgetMetadataApi(config);

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
  } satisfies WidgetMetadataSearchRequest;

  try {
    const data = await api.widgetMetadataSearch(body);
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

[**WidgetMetadataPaginationResponse**](WidgetMetadataPaginationResponse.md)

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


## widgetMetadataUpdate

> WidgetMetadata widgetMetadataUpdate(id, widgetMetadataUpdate)



Update a widget metadata.

### Example

```ts
import {
  Configuration,
  WidgetMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { WidgetMetadataUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WidgetMetadataApi(config);

  const body = {
    // string
    id: id_example,
    // WidgetMetadataUpdate (optional)
    widgetMetadataUpdate: ...,
  } satisfies WidgetMetadataUpdateRequest;

  try {
    const data = await api.widgetMetadataUpdate(body);
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
| **widgetMetadataUpdate** | [WidgetMetadataUpdate](WidgetMetadataUpdate.md) |  | [Optional] |

### Return type

[**WidgetMetadata**](WidgetMetadata.md)

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

