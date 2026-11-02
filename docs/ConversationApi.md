# ConversationApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**conversationCreate**](ConversationApi.md#conversationcreate) | **POST** /v4/api/conversation |  |
| [**conversationGet**](ConversationApi.md#conversationget) | **GET** /v4/api/conversation/{id} |  |
| [**conversationSearch**](ConversationApi.md#conversationsearch) | **GET** /v4/api/conversation |  |
| [**conversationUpdate**](ConversationApi.md#conversationupdate) | **PUT** /v4/api/conversation/{id} |  |



## conversationCreate

> Conversation conversationCreate(conversationCreate)



Create a conversation.

### Example

```ts
import {
  Configuration,
  ConversationApi,
} from '@statflo/statflo-typescript-sdk';
import type { ConversationCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ConversationApi(config);

  const body = {
    // ConversationCreate (optional)
    conversationCreate: ...,
  } satisfies ConversationCreateRequest;

  try {
    const data = await api.conversationCreate(body);
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
| **conversationCreate** | [ConversationCreate](ConversationCreate.md) |  | [Optional] |

### Return type

[**Conversation**](Conversation.md)

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


## conversationGet

> Conversation conversationGet(id)



Retrieve a conversation.

### Example

```ts
import {
  Configuration,
  ConversationApi,
} from '@statflo/statflo-typescript-sdk';
import type { ConversationGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ConversationApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies ConversationGetRequest;

  try {
    const data = await api.conversationGet(body);
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

[**Conversation**](Conversation.md)

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


## conversationSearch

> ConversationPaginationResponse conversationSearch(filter, query, page, perPage, sort)



Search conversations.

### Example

```ts
import {
  Configuration,
  ConversationApi,
} from '@statflo/statflo-typescript-sdk';
import type { ConversationSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ConversationApi(config);

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
  } satisfies ConversationSearchRequest;

  try {
    const data = await api.conversationSearch(body);
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

[**ConversationPaginationResponse**](ConversationPaginationResponse.md)

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


## conversationUpdate

> Conversation conversationUpdate(id, conversationUpdate)



Update a conversation.

### Example

```ts
import {
  Configuration,
  ConversationApi,
} from '@statflo/statflo-typescript-sdk';
import type { ConversationUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ConversationApi(config);

  const body = {
    // string
    id: id_example,
    // ConversationUpdate (optional)
    conversationUpdate: ...,
  } satisfies ConversationUpdateRequest;

  try {
    const data = await api.conversationUpdate(body);
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
| **conversationUpdate** | [ConversationUpdate](ConversationUpdate.md) |  | [Optional] |

### Return type

[**Conversation**](Conversation.md)

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

