# BulkMessageApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**bulkMessageCreate**](BulkMessageApi.md#bulkmessagecreate) | **POST** /v4/api/bulk-message |  |
| [**bulkMessageGet**](BulkMessageApi.md#bulkmessageget) | **GET** /v4/api/bulk-message/{id} |  |
| [**bulkMessageSearch**](BulkMessageApi.md#bulkmessagesearch) | **GET** /v4/api/bulk-message |  |
| [**bulkMessageUpdate**](BulkMessageApi.md#bulkmessageupdate) | **PUT** /v4/api/bulk-message/{id} |  |



## bulkMessageCreate

> BulkMessage bulkMessageCreate(bulkMessageCreate)



Create a Bulk Message.

### Example

```ts
import {
  Configuration,
  BulkMessageApi,
} from '@statflo/statflo-typescript-sdk';
import type { BulkMessageCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BulkMessageApi(config);

  const body = {
    // BulkMessageCreate (optional)
    bulkMessageCreate: ...,
  } satisfies BulkMessageCreateRequest;

  try {
    const data = await api.bulkMessageCreate(body);
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
| **bulkMessageCreate** | [BulkMessageCreate](BulkMessageCreate.md) |  | [Optional] |

### Return type

[**BulkMessage**](BulkMessage.md)

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


## bulkMessageGet

> BulkMessage bulkMessageGet(id)



Retrieve a Bulk Message.

### Example

```ts
import {
  Configuration,
  BulkMessageApi,
} from '@statflo/statflo-typescript-sdk';
import type { BulkMessageGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BulkMessageApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies BulkMessageGetRequest;

  try {
    const data = await api.bulkMessageGet(body);
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

[**BulkMessage**](BulkMessage.md)

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


## bulkMessageSearch

> BulkMessagePaginationResponse bulkMessageSearch(filter, query, page, perPage, sort)



Search bulkMessages.

### Example

```ts
import {
  Configuration,
  BulkMessageApi,
} from '@statflo/statflo-typescript-sdk';
import type { BulkMessageSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BulkMessageApi(config);

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
  } satisfies BulkMessageSearchRequest;

  try {
    const data = await api.bulkMessageSearch(body);
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

[**BulkMessagePaginationResponse**](BulkMessagePaginationResponse.md)

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


## bulkMessageUpdate

> BulkMessage bulkMessageUpdate(id, bulkMessageUpdate)



Update a Bulk Message.

### Example

```ts
import {
  Configuration,
  BulkMessageApi,
} from '@statflo/statflo-typescript-sdk';
import type { BulkMessageUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BulkMessageApi(config);

  const body = {
    // string
    id: id_example,
    // BulkMessageUpdate (optional)
    bulkMessageUpdate: ...,
  } satisfies BulkMessageUpdateRequest;

  try {
    const data = await api.bulkMessageUpdate(body);
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
| **bulkMessageUpdate** | [BulkMessageUpdate](BulkMessageUpdate.md) |  | [Optional] |

### Return type

[**BulkMessage**](BulkMessage.md)

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

