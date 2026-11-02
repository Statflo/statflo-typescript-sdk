# NotepadApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**notepadCreate**](NotepadApi.md#notepadcreate) | **POST** /v4/api/notepad |  |
| [**notepadDelete**](NotepadApi.md#notepaddelete) | **DELETE** /v4/api/notepad/{id} |  |
| [**notepadGet**](NotepadApi.md#notepadget) | **GET** /v4/api/notepad/{id} |  |
| [**notepadSearch**](NotepadApi.md#notepadsearch) | **GET** /v4/api/notepad |  |
| [**notepadUpdate**](NotepadApi.md#notepadupdate) | **PUT** /v4/api/notepad/{id} |  |



## notepadCreate

> Notepad notepadCreate(notepadCreate)



Create a notepad.

### Example

```ts
import {
  Configuration,
  NotepadApi,
} from '@statflo/statflo-typescript-sdk';
import type { NotepadCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new NotepadApi(config);

  const body = {
    // NotepadCreate (optional)
    notepadCreate: ...,
  } satisfies NotepadCreateRequest;

  try {
    const data = await api.notepadCreate(body);
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
| **notepadCreate** | [NotepadCreate](NotepadCreate.md) |  | [Optional] |

### Return type

[**Notepad**](Notepad.md)

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


## notepadDelete

> notepadDelete(id)



Remove a notepad.

### Example

```ts
import {
  Configuration,
  NotepadApi,
} from '@statflo/statflo-typescript-sdk';
import type { NotepadDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new NotepadApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies NotepadDeleteRequest;

  try {
    const data = await api.notepadDelete(body);
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


## notepadGet

> Notepad notepadGet(id)



Retrieve a notepad.

### Example

```ts
import {
  Configuration,
  NotepadApi,
} from '@statflo/statflo-typescript-sdk';
import type { NotepadGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new NotepadApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies NotepadGetRequest;

  try {
    const data = await api.notepadGet(body);
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

[**Notepad**](Notepad.md)

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


## notepadSearch

> NotepadPaginationResponse notepadSearch(filter, query, page, perPage, sort)



Search notepads.

### Example

```ts
import {
  Configuration,
  NotepadApi,
} from '@statflo/statflo-typescript-sdk';
import type { NotepadSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new NotepadApi(config);

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
  } satisfies NotepadSearchRequest;

  try {
    const data = await api.notepadSearch(body);
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

[**NotepadPaginationResponse**](NotepadPaginationResponse.md)

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


## notepadUpdate

> Notepad notepadUpdate(id, notepadUpdate)



Update a notepad.

### Example

```ts
import {
  Configuration,
  NotepadApi,
} from '@statflo/statflo-typescript-sdk';
import type { NotepadUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new NotepadApi(config);

  const body = {
    // string
    id: id_example,
    // NotepadUpdate (optional)
    notepadUpdate: ...,
  } satisfies NotepadUpdateRequest;

  try {
    const data = await api.notepadUpdate(body);
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
| **notepadUpdate** | [NotepadUpdate](NotepadUpdate.md) |  | [Optional] |

### Return type

[**Notepad**](Notepad.md)

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

