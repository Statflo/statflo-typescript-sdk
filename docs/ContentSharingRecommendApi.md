# ContentSharingRecommendApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**contentSharingRecommendedCreate**](ContentSharingRecommendApi.md#contentsharingrecommendedcreate) | **POST** /v4/api/content-sharing-recommend |  |
| [**contentSharingRecommendedDelete**](ContentSharingRecommendApi.md#contentsharingrecommendeddelete) | **DELETE** /v4/api/content-sharing-recommend/{id} |  |
| [**contentSharingRecommendedGet**](ContentSharingRecommendApi.md#contentsharingrecommendedget) | **GET** /v4/api/content-sharing-recommend/{id} |  |
| [**contentSharingRecommendedSearch**](ContentSharingRecommendApi.md#contentsharingrecommendedsearch) | **GET** /v4/api/content-sharing-recommend |  |
| [**contentSharingRecommendedUpdate**](ContentSharingRecommendApi.md#contentsharingrecommendedupdate) | **PUT** /v4/api/content-sharing-recommend/{id} |  |



## contentSharingRecommendedCreate

> ContentSharingRecommended contentSharingRecommendedCreate(contentSharingRecommendedCreate)



Create a content sharing recommendation.

### Example

```ts
import {
  Configuration,
  ContentSharingRecommendApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContentSharingRecommendedCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContentSharingRecommendApi(config);

  const body = {
    // ContentSharingRecommendedCreate (optional)
    contentSharingRecommendedCreate: ...,
  } satisfies ContentSharingRecommendedCreateRequest;

  try {
    const data = await api.contentSharingRecommendedCreate(body);
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
| **contentSharingRecommendedCreate** | [ContentSharingRecommendedCreate](ContentSharingRecommendedCreate.md) |  | [Optional] |

### Return type

[**ContentSharingRecommended**](ContentSharingRecommended.md)

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


## contentSharingRecommendedDelete

> contentSharingRecommendedDelete(id)



Remove a content sharing recommendation.

### Example

```ts
import {
  Configuration,
  ContentSharingRecommendApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContentSharingRecommendedDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContentSharingRecommendApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies ContentSharingRecommendedDeleteRequest;

  try {
    const data = await api.contentSharingRecommendedDelete(body);
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


## contentSharingRecommendedGet

> ContentSharingRecommended contentSharingRecommendedGet(id)



Retrieve a content sharing recommendation.

### Example

```ts
import {
  Configuration,
  ContentSharingRecommendApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContentSharingRecommendedGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContentSharingRecommendApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies ContentSharingRecommendedGetRequest;

  try {
    const data = await api.contentSharingRecommendedGet(body);
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

[**ContentSharingRecommended**](ContentSharingRecommended.md)

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


## contentSharingRecommendedSearch

> ContentSharingRecommendPaginationResponse contentSharingRecommendedSearch(filter, query, page, perPage, sort)



Get a list of all recommendations

### Example

```ts
import {
  Configuration,
  ContentSharingRecommendApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContentSharingRecommendedSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContentSharingRecommendApi(config);

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
  } satisfies ContentSharingRecommendedSearchRequest;

  try {
    const data = await api.contentSharingRecommendedSearch(body);
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

[**ContentSharingRecommendPaginationResponse**](ContentSharingRecommendPaginationResponse.md)

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


## contentSharingRecommendedUpdate

> ContentSharingRecommended contentSharingRecommendedUpdate(id, contentSharingRecommendedUpdate)



Update a content sharing recommendation.

### Example

```ts
import {
  Configuration,
  ContentSharingRecommendApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContentSharingRecommendedUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContentSharingRecommendApi(config);

  const body = {
    // string
    id: id_example,
    // ContentSharingRecommendedUpdate (optional)
    contentSharingRecommendedUpdate: ...,
  } satisfies ContentSharingRecommendedUpdateRequest;

  try {
    const data = await api.contentSharingRecommendedUpdate(body);
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
| **contentSharingRecommendedUpdate** | [ContentSharingRecommendedUpdate](ContentSharingRecommendedUpdate.md) |  | [Optional] |

### Return type

[**ContentSharingRecommended**](ContentSharingRecommended.md)

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

