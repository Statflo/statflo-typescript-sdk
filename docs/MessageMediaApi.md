# MessageMediaApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**messageMediaCreate**](MessageMediaApi.md#messagemediacreate) | **POST** /v4/api/message-media |  |
| [**messageMediaDelete**](MessageMediaApi.md#messagemediadelete) | **DELETE** /v4/api/message-media/{id} |  |
| [**messageMediaGet**](MessageMediaApi.md#messagemediaget) | **GET** /v4/api/message-media/{id} |  |
| [**messageMediaSearch**](MessageMediaApi.md#messagemediasearch) | **GET** /v4/api/message-media |  |
| [**messageMediaUpdate**](MessageMediaApi.md#messagemediaupdate) | **PUT** /v4/api/message-media/{id} |  |



## messageMediaCreate

> MessageMedia messageMediaCreate(messageMediaCreate)



Create a message media.

### Example

```ts
import {
  Configuration,
  MessageMediaApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageMediaCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageMediaApi(config);

  const body = {
    // MessageMediaCreate (optional)
    messageMediaCreate: ...,
  } satisfies MessageMediaCreateRequest;

  try {
    const data = await api.messageMediaCreate(body);
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
| **messageMediaCreate** | [MessageMediaCreate](MessageMediaCreate.md) |  | [Optional] |

### Return type

[**MessageMedia**](MessageMedia.md)

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


## messageMediaDelete

> messageMediaDelete(id)



Remove a Message Media.

### Example

```ts
import {
  Configuration,
  MessageMediaApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageMediaDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageMediaApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies MessageMediaDeleteRequest;

  try {
    const data = await api.messageMediaDelete(body);
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


## messageMediaGet

> MessageMedia messageMediaGet(id)



Retrieve message media.

### Example

```ts
import {
  Configuration,
  MessageMediaApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageMediaGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageMediaApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies MessageMediaGetRequest;

  try {
    const data = await api.messageMediaGet(body);
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

[**MessageMedia**](MessageMedia.md)

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


## messageMediaSearch

> MessageMediaPaginationResponse messageMediaSearch(filter, query, page, perPage, sort)



Search message media.

### Example

```ts
import {
  Configuration,
  MessageMediaApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageMediaSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageMediaApi(config);

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
  } satisfies MessageMediaSearchRequest;

  try {
    const data = await api.messageMediaSearch(body);
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

[**MessageMediaPaginationResponse**](MessageMediaPaginationResponse.md)

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


## messageMediaUpdate

> MessageMedia messageMediaUpdate(id, messageMediaUpdate)



Update a message media.

### Example

```ts
import {
  Configuration,
  MessageMediaApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageMediaUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageMediaApi(config);

  const body = {
    // string
    id: id_example,
    // MessageMediaUpdate (optional)
    messageMediaUpdate: ...,
  } satisfies MessageMediaUpdateRequest;

  try {
    const data = await api.messageMediaUpdate(body);
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
| **messageMediaUpdate** | [MessageMediaUpdate](MessageMediaUpdate.md) |  | [Optional] |

### Return type

[**MessageMedia**](MessageMedia.md)

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

