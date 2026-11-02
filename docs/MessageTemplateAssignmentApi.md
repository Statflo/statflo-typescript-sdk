# MessageTemplateAssignmentApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**messageTemplateAssignmentCreate**](MessageTemplateAssignmentApi.md#messagetemplateassignmentcreate) | **POST** /v4/api/message-template-assignment |  |
| [**messageTemplateAssignmentDelete**](MessageTemplateAssignmentApi.md#messagetemplateassignmentdelete) | **DELETE** /v4/api/message-template-assignment/{id} |  |
| [**messageTemplateAssignmentGet**](MessageTemplateAssignmentApi.md#messagetemplateassignmentget) | **GET** /v4/api/message-template-assignment/{id} |  |
| [**messageTemplateAssignmentSearch**](MessageTemplateAssignmentApi.md#messagetemplateassignmentsearch) | **GET** /v4/api/message-template-assignment |  |
| [**messageTemplateAssignmentUpdate**](MessageTemplateAssignmentApi.md#messagetemplateassignmentupdate) | **PUT** /v4/api/message-template-assignment/{id} |  |



## messageTemplateAssignmentCreate

> MessageTemplateAssignment messageTemplateAssignmentCreate(messageTemplateAssignmentCreate)



Create a message template assignment.

### Example

```ts
import {
  Configuration,
  MessageTemplateAssignmentApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageTemplateAssignmentCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageTemplateAssignmentApi(config);

  const body = {
    // MessageTemplateAssignmentCreate (optional)
    messageTemplateAssignmentCreate: ...,
  } satisfies MessageTemplateAssignmentCreateRequest;

  try {
    const data = await api.messageTemplateAssignmentCreate(body);
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
| **messageTemplateAssignmentCreate** | [MessageTemplateAssignmentCreate](MessageTemplateAssignmentCreate.md) |  | [Optional] |

### Return type

[**MessageTemplateAssignment**](MessageTemplateAssignment.md)

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


## messageTemplateAssignmentDelete

> messageTemplateAssignmentDelete(id)



Remove a message template assignment.

### Example

```ts
import {
  Configuration,
  MessageTemplateAssignmentApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageTemplateAssignmentDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageTemplateAssignmentApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies MessageTemplateAssignmentDeleteRequest;

  try {
    const data = await api.messageTemplateAssignmentDelete(body);
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


## messageTemplateAssignmentGet

> MessageTemplateAssignment messageTemplateAssignmentGet(id)



Retrieve a message template assignment.

### Example

```ts
import {
  Configuration,
  MessageTemplateAssignmentApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageTemplateAssignmentGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageTemplateAssignmentApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies MessageTemplateAssignmentGetRequest;

  try {
    const data = await api.messageTemplateAssignmentGet(body);
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

[**MessageTemplateAssignment**](MessageTemplateAssignment.md)

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


## messageTemplateAssignmentSearch

> MessageTemplateAssignmentPaginationResponse messageTemplateAssignmentSearch(filter, query, page, perPage, sort)



Search message template assignments.

### Example

```ts
import {
  Configuration,
  MessageTemplateAssignmentApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageTemplateAssignmentSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageTemplateAssignmentApi(config);

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
  } satisfies MessageTemplateAssignmentSearchRequest;

  try {
    const data = await api.messageTemplateAssignmentSearch(body);
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

[**MessageTemplateAssignmentPaginationResponse**](MessageTemplateAssignmentPaginationResponse.md)

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


## messageTemplateAssignmentUpdate

> MessageTemplateAssignment messageTemplateAssignmentUpdate(id, messageTemplateAssignmentUpdate)



Update a message template Assignment.

### Example

```ts
import {
  Configuration,
  MessageTemplateAssignmentApi,
} from '@statflo/statflo-typescript-sdk';
import type { MessageTemplateAssignmentUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MessageTemplateAssignmentApi(config);

  const body = {
    // string
    id: id_example,
    // MessageTemplateAssignmentUpdate (optional)
    messageTemplateAssignmentUpdate: ...,
  } satisfies MessageTemplateAssignmentUpdateRequest;

  try {
    const data = await api.messageTemplateAssignmentUpdate(body);
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
| **messageTemplateAssignmentUpdate** | [MessageTemplateAssignmentUpdate](MessageTemplateAssignmentUpdate.md) |  | [Optional] |

### Return type

[**MessageTemplateAssignment**](MessageTemplateAssignment.md)

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

