# MessageTemplateApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**messageTemplateCreate**](MessageTemplateApi.md#messagetemplatecreate) | **POST** /v4/api/message-template |  |
| [**messageTemplateDelete**](MessageTemplateApi.md#messagetemplatedelete) | **DELETE** /v4/api/message-template/{id} |  |
| [**messageTemplateGet**](MessageTemplateApi.md#messagetemplateget) | **GET** /v4/api/message-template/{id} |  |
| [**messageTemplateSearch**](MessageTemplateApi.md#messagetemplatesearch) | **GET** /v4/api/message-template |  |
| [**messageTemplateUpdate**](MessageTemplateApi.md#messagetemplateupdate) | **PUT** /v4/api/message-template/{id} |  |



## messageTemplateCreate

> MessageTemplate messageTemplateCreate(messageTemplateCreate)



Create an message template.

### Example

```ts
import {
  Configuration,
  MessageTemplateApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageTemplateCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageTemplateApi(config);

  const body = {
    // MessageTemplateCreate (optional)
    messageTemplateCreate: ...,
  } satisfies MessageTemplateCreateRequest;

  try {
    const data = await api.messageTemplateCreate(body);
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
| **messageTemplateCreate** | [MessageTemplateCreate](MessageTemplateCreate.md) |  | [Optional] |

### Return type

[**MessageTemplate**](MessageTemplate.md)

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


## messageTemplateDelete

> messageTemplateDelete(id)



Remove an message template.

### Example

```ts
import {
  Configuration,
  MessageTemplateApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageTemplateDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageTemplateApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies MessageTemplateDeleteRequest;

  try {
    const data = await api.messageTemplateDelete(body);
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


## messageTemplateGet

> MessageTemplate messageTemplateGet(id)



Retrieve an message template.

### Example

```ts
import {
  Configuration,
  MessageTemplateApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageTemplateGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageTemplateApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies MessageTemplateGetRequest;

  try {
    const data = await api.messageTemplateGet(body);
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

[**MessageTemplate**](MessageTemplate.md)

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


## messageTemplateSearch

> MessageTemplatePaginationResponse messageTemplateSearch(filter, query, page, perPage, sort)



Search message templates.

### Example

```ts
import {
  Configuration,
  MessageTemplateApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageTemplateSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageTemplateApi(config);

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
  } satisfies MessageTemplateSearchRequest;

  try {
    const data = await api.messageTemplateSearch(body);
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

[**MessageTemplatePaginationResponse**](MessageTemplatePaginationResponse.md)

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


## messageTemplateUpdate

> MessageTemplate messageTemplateUpdate(id, messageTemplateUpdate)



Update an message template.

### Example

```ts
import {
  Configuration,
  MessageTemplateApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageTemplateUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageTemplateApi(config);

  const body = {
    // string
    id: id_example,
    // MessageTemplateUpdate (optional)
    messageTemplateUpdate: ...,
  } satisfies MessageTemplateUpdateRequest;

  try {
    const data = await api.messageTemplateUpdate(body);
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
| **messageTemplateUpdate** | [MessageTemplateUpdate](MessageTemplateUpdate.md) |  | [Optional] |

### Return type

[**MessageTemplate**](MessageTemplate.md)

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

