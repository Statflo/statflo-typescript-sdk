# ContentSharingLinkApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**contentSharingLinkCreate**](ContentSharingLinkApi.md#contentsharinglinkcreate) | **POST** /v4/api/content-sharing-link |  |
| [**contentSharingLinkDelete**](ContentSharingLinkApi.md#contentsharinglinkdelete) | **DELETE** /v4/api/content-sharing-link/{id} |  |
| [**contentSharingLinkGet**](ContentSharingLinkApi.md#contentsharinglinkget) | **GET** /v4/api/content-sharing-link/{id} |  |
| [**contentSharingLinkSearch**](ContentSharingLinkApi.md#contentsharinglinksearch) | **GET** /v4/api/content-sharing-link |  |
| [**contentSharingLinkUpdate**](ContentSharingLinkApi.md#contentsharinglinkupdate) | **PUT** /v4/api/content-sharing-link/{id} |  |



## contentSharingLinkCreate

> ContentSharingLink contentSharingLinkCreate(contentSharingLinkCreate)



Create a content sharing link.

### Example

```ts
import {
  Configuration,
  ContentSharingLinkApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContentSharingLinkCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContentSharingLinkApi(config);

  const body = {
    // ContentSharingLinkCreate (optional)
    contentSharingLinkCreate: ...,
  } satisfies ContentSharingLinkCreateRequest;

  try {
    const data = await api.contentSharingLinkCreate(body);
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
| **contentSharingLinkCreate** | [ContentSharingLinkCreate](ContentSharingLinkCreate.md) |  | [Optional] |

### Return type

[**ContentSharingLink**](ContentSharingLink.md)

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


## contentSharingLinkDelete

> contentSharingLinkDelete(id)



Remove a content sharing link.

### Example

```ts
import {
  Configuration,
  ContentSharingLinkApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContentSharingLinkDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContentSharingLinkApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies ContentSharingLinkDeleteRequest;

  try {
    const data = await api.contentSharingLinkDelete(body);
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


## contentSharingLinkGet

> ContentSharingLink contentSharingLinkGet(id)



Retrieve a content sharing category.

### Example

```ts
import {
  Configuration,
  ContentSharingLinkApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContentSharingLinkGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContentSharingLinkApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies ContentSharingLinkGetRequest;

  try {
    const data = await api.contentSharingLinkGet(body);
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

[**ContentSharingLink**](ContentSharingLink.md)

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


## contentSharingLinkSearch

> ContentSharingLinkPaginationResponse contentSharingLinkSearch(filter, query, page, perPage, sort)



Get a list of all links

### Example

```ts
import {
  Configuration,
  ContentSharingLinkApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContentSharingLinkSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContentSharingLinkApi(config);

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
  } satisfies ContentSharingLinkSearchRequest;

  try {
    const data = await api.contentSharingLinkSearch(body);
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

[**ContentSharingLinkPaginationResponse**](ContentSharingLinkPaginationResponse.md)

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


## contentSharingLinkUpdate

> ContentSharingLink contentSharingLinkUpdate(id, contentSharingLinkUpdate)



Update a content sharing link.

### Example

```ts
import {
  Configuration,
  ContentSharingLinkApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContentSharingLinkUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContentSharingLinkApi(config);

  const body = {
    // string
    id: id_example,
    // ContentSharingLinkUpdate (optional)
    contentSharingLinkUpdate: ...,
  } satisfies ContentSharingLinkUpdateRequest;

  try {
    const data = await api.contentSharingLinkUpdate(body);
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
| **contentSharingLinkUpdate** | [ContentSharingLinkUpdate](ContentSharingLinkUpdate.md) |  | [Optional] |

### Return type

[**ContentSharingLink**](ContentSharingLink.md)

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

