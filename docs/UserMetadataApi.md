# UserMetadataApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**userMetadataCreate**](UserMetadataApi.md#usermetadatacreate) | **POST** /v4/api/user-metadata |  |
| [**userMetadataDelete**](UserMetadataApi.md#usermetadatadelete) | **DELETE** /v4/api/user-metadata/{id} |  |
| [**userMetadataGet**](UserMetadataApi.md#usermetadataget) | **GET** /v4/api/user-metadata/{id} |  |
| [**userMetadataSearch**](UserMetadataApi.md#usermetadatasearch) | **GET** /v4/api/user-metadata |  |
| [**userMetadataUpdate**](UserMetadataApi.md#usermetadataupdate) | **PUT** /v4/api/user-metadata/{id} |  |



## userMetadataCreate

> UserMetadata userMetadataCreate(userMetadataCreate)



Create a user metadata.

### Example

```ts
import {
  Configuration,
  UserMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { UserMetadataCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UserMetadataApi(config);

  const body = {
    // UserMetadataCreate (optional)
    userMetadataCreate: ...,
  } satisfies UserMetadataCreateRequest;

  try {
    const data = await api.userMetadataCreate(body);
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
| **userMetadataCreate** | [UserMetadataCreate](UserMetadataCreate.md) |  | [Optional] |

### Return type

[**UserMetadata**](UserMetadata.md)

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


## userMetadataDelete

> userMetadataDelete(id)



Remove a user metadata.

### Example

```ts
import {
  Configuration,
  UserMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { UserMetadataDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UserMetadataApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies UserMetadataDeleteRequest;

  try {
    const data = await api.userMetadataDelete(body);
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


## userMetadataGet

> UserMetadata userMetadataGet(id)



Retrieve a user metadata.

### Example

```ts
import {
  Configuration,
  UserMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { UserMetadataGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UserMetadataApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies UserMetadataGetRequest;

  try {
    const data = await api.userMetadataGet(body);
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

[**UserMetadata**](UserMetadata.md)

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


## userMetadataSearch

> UserMetadataPaginationResponse userMetadataSearch(filter, query, page, perPage, sort)



Search user metadata.

### Example

```ts
import {
  Configuration,
  UserMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { UserMetadataSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UserMetadataApi(config);

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
  } satisfies UserMetadataSearchRequest;

  try {
    const data = await api.userMetadataSearch(body);
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

[**UserMetadataPaginationResponse**](UserMetadataPaginationResponse.md)

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


## userMetadataUpdate

> UserMetadata userMetadataUpdate(id, userMetadataUpdate)



Update a user metadata.

### Example

```ts
import {
  Configuration,
  UserMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { UserMetadataUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UserMetadataApi(config);

  const body = {
    // string
    id: id_example,
    // UserMetadataUpdate (optional)
    userMetadataUpdate: ...,
  } satisfies UserMetadataUpdateRequest;

  try {
    const data = await api.userMetadataUpdate(body);
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
| **userMetadataUpdate** | [UserMetadataUpdate](UserMetadataUpdate.md) |  | [Optional] |

### Return type

[**UserMetadata**](UserMetadata.md)

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

