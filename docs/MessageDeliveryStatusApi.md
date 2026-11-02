# MessageDeliveryStatusApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**messageDeliveryStatusCreate**](MessageDeliveryStatusApi.md#messagedeliverystatuscreate) | **POST** /v4/api/message-delivery-status |  |
| [**messageDeliveryStatusDelete**](MessageDeliveryStatusApi.md#messagedeliverystatusdelete) | **DELETE** /v4/api/message-delivery-status/{id} |  |
| [**messageDeliveryStatusGet**](MessageDeliveryStatusApi.md#messagedeliverystatusget) | **GET** /v4/api/message-delivery-status/{id} |  |
| [**messageDeliveryStatusSearch**](MessageDeliveryStatusApi.md#messagedeliverystatussearch) | **GET** /v4/api/message-delivery-status |  |
| [**messageDeliveryStatusUpdate**](MessageDeliveryStatusApi.md#messagedeliverystatusupdate) | **PUT** /v4/api/message-delivery-status/{id} |  |



## messageDeliveryStatusCreate

> MessageDeliveryStatus messageDeliveryStatusCreate(messageDeliveryStatusCreate)



Create a message delivery status.

### Example

```ts
import {
  Configuration,
  MessageDeliveryStatusApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageDeliveryStatusCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageDeliveryStatusApi(config);

  const body = {
    // MessageDeliveryStatusCreate (optional)
    messageDeliveryStatusCreate: ...,
  } satisfies MessageDeliveryStatusCreateRequest;

  try {
    const data = await api.messageDeliveryStatusCreate(body);
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
| **messageDeliveryStatusCreate** | [MessageDeliveryStatusCreate](MessageDeliveryStatusCreate.md) |  | [Optional] |

### Return type

[**MessageDeliveryStatus**](MessageDeliveryStatus.md)

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


## messageDeliveryStatusDelete

> messageDeliveryStatusDelete(id)



Remove a Message Delivery Status.

### Example

```ts
import {
  Configuration,
  MessageDeliveryStatusApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageDeliveryStatusDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageDeliveryStatusApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies MessageDeliveryStatusDeleteRequest;

  try {
    const data = await api.messageDeliveryStatusDelete(body);
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


## messageDeliveryStatusGet

> MessageDeliveryStatus messageDeliveryStatusGet(id)



Retrieve message delivery status.

### Example

```ts
import {
  Configuration,
  MessageDeliveryStatusApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageDeliveryStatusGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageDeliveryStatusApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies MessageDeliveryStatusGetRequest;

  try {
    const data = await api.messageDeliveryStatusGet(body);
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

[**MessageDeliveryStatus**](MessageDeliveryStatus.md)

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


## messageDeliveryStatusSearch

> MessageDeliveryStatusPaginationResponse messageDeliveryStatusSearch(filter, query, page, perPage, sort)



Search message delivery status.

### Example

```ts
import {
  Configuration,
  MessageDeliveryStatusApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageDeliveryStatusSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageDeliveryStatusApi(config);

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
  } satisfies MessageDeliveryStatusSearchRequest;

  try {
    const data = await api.messageDeliveryStatusSearch(body);
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

[**MessageDeliveryStatusPaginationResponse**](MessageDeliveryStatusPaginationResponse.md)

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


## messageDeliveryStatusUpdate

> MessageDeliveryStatus messageDeliveryStatusUpdate(id, messageDeliveryStatusUpdate)



Update a message delivery status.

### Example

```ts
import {
  Configuration,
  MessageDeliveryStatusApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageDeliveryStatusUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageDeliveryStatusApi(config);

  const body = {
    // string
    id: id_example,
    // MessageDeliveryStatusUpdate (optional)
    messageDeliveryStatusUpdate: ...,
  } satisfies MessageDeliveryStatusUpdateRequest;

  try {
    const data = await api.messageDeliveryStatusUpdate(body);
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
| **messageDeliveryStatusUpdate** | [MessageDeliveryStatusUpdate](MessageDeliveryStatusUpdate.md) |  | [Optional] |

### Return type

[**MessageDeliveryStatus**](MessageDeliveryStatus.md)

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

