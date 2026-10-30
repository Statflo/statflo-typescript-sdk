# ContentSharingCategoryApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**contentSharingCategoryCreate**](ContentSharingCategoryApi.md#contentsharingcategorycreate) | **POST** /v4/api/content-sharing-category |  |
| [**contentSharingCategoryDelete**](ContentSharingCategoryApi.md#contentsharingcategorydelete) | **DELETE** /v4/api/content-sharing-category/{id} |  |
| [**contentSharingCategoryGet**](ContentSharingCategoryApi.md#contentsharingcategoryget) | **GET** /v4/api/content-sharing-category/{id} |  |
| [**contentSharingCategorySearch**](ContentSharingCategoryApi.md#contentsharingcategorysearch) | **GET** /v4/api/content-sharing-category |  |
| [**contentSharingCategoryUpdate**](ContentSharingCategoryApi.md#contentsharingcategoryupdate) | **PUT** /v4/api/content-sharing-category/{id} |  |



## contentSharingCategoryCreate

> ContentSharingCategory contentSharingCategoryCreate(contentSharingCategoryCreate)



Create a content sharing category.

### Example

```ts
import {
  Configuration,
  ContentSharingCategoryApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContentSharingCategoryCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContentSharingCategoryApi(config);

  const body = {
    // ContentSharingCategoryCreate (optional)
    contentSharingCategoryCreate: ...,
  } satisfies ContentSharingCategoryCreateRequest;

  try {
    const data = await api.contentSharingCategoryCreate(body);
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
| **contentSharingCategoryCreate** | [ContentSharingCategoryCreate](ContentSharingCategoryCreate.md) |  | [Optional] |

### Return type

[**ContentSharingCategory**](ContentSharingCategory.md)

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


## contentSharingCategoryDelete

> contentSharingCategoryDelete(id)



Remove a content sharing category.

### Example

```ts
import {
  Configuration,
  ContentSharingCategoryApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContentSharingCategoryDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContentSharingCategoryApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies ContentSharingCategoryDeleteRequest;

  try {
    const data = await api.contentSharingCategoryDelete(body);
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


## contentSharingCategoryGet

> ContentSharingCategory contentSharingCategoryGet(id)



Retrieve a content sharing category.

### Example

```ts
import {
  Configuration,
  ContentSharingCategoryApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContentSharingCategoryGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContentSharingCategoryApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies ContentSharingCategoryGetRequest;

  try {
    const data = await api.contentSharingCategoryGet(body);
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

[**ContentSharingCategory**](ContentSharingCategory.md)

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


## contentSharingCategorySearch

> ContentSharingCategoryPaginationResponse contentSharingCategorySearch(filter, query, page, perPage, sort)



Search content sharing categories

### Example

```ts
import {
  Configuration,
  ContentSharingCategoryApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContentSharingCategorySearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContentSharingCategoryApi(config);

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
  } satisfies ContentSharingCategorySearchRequest;

  try {
    const data = await api.contentSharingCategorySearch(body);
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

[**ContentSharingCategoryPaginationResponse**](ContentSharingCategoryPaginationResponse.md)

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


## contentSharingCategoryUpdate

> ContentSharingCategory contentSharingCategoryUpdate(id, contentSharingCategoryUpdate)



Update a content sharing category.

### Example

```ts
import {
  Configuration,
  ContentSharingCategoryApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContentSharingCategoryUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContentSharingCategoryApi(config);

  const body = {
    // string
    id: id_example,
    // ContentSharingCategoryUpdate (optional)
    contentSharingCategoryUpdate: ...,
  } satisfies ContentSharingCategoryUpdateRequest;

  try {
    const data = await api.contentSharingCategoryUpdate(body);
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
| **contentSharingCategoryUpdate** | [ContentSharingCategoryUpdate](ContentSharingCategoryUpdate.md) |  | [Optional] |

### Return type

[**ContentSharingCategory**](ContentSharingCategory.md)

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

