# UserExternalIdApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**userExternalIdCreate**](UserExternalIdApi.md#userexternalidcreate) | **POST** /v4/api/user-external-id |  |
| [**userExternalIdDelete**](UserExternalIdApi.md#userexternaliddelete) | **DELETE** /v4/api/user-external-id/{id} |  |
| [**userExternalIdGet**](UserExternalIdApi.md#userexternalidget) | **GET** /v4/api/user-external-id/{id} |  |
| [**userExternalIdSearch**](UserExternalIdApi.md#userexternalidsearch) | **GET** /v4/api/user-external-id |  |
| [**userExternalIdUpdate**](UserExternalIdApi.md#userexternalidupdate) | **PUT** /v4/api/user-external-id/{id} |  |



## userExternalIdCreate

> UserExternalId userExternalIdCreate(userExternalIdCreate)



Create a user external id.

### Example

```ts
import {
  Configuration,
  UserExternalIdApi,
} from '@statflo/statflo-typescript-sdk';
import type { UserExternalIdCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UserExternalIdApi(config);

  const body = {
    // UserExternalIdCreate (optional)
    userExternalIdCreate: ...,
  } satisfies UserExternalIdCreateRequest;

  try {
    const data = await api.userExternalIdCreate(body);
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
| **userExternalIdCreate** | [UserExternalIdCreate](UserExternalIdCreate.md) |  | [Optional] |

### Return type

[**UserExternalId**](UserExternalId.md)

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


## userExternalIdDelete

> userExternalIdDelete(id)



Remove a user external id.

### Example

```ts
import {
  Configuration,
  UserExternalIdApi,
} from '@statflo/statflo-typescript-sdk';
import type { UserExternalIdDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UserExternalIdApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies UserExternalIdDeleteRequest;

  try {
    const data = await api.userExternalIdDelete(body);
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


## userExternalIdGet

> UserExternalId userExternalIdGet(id)



Retrieve a user external id.

### Example

```ts
import {
  Configuration,
  UserExternalIdApi,
} from '@statflo/statflo-typescript-sdk';
import type { UserExternalIdGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UserExternalIdApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies UserExternalIdGetRequest;

  try {
    const data = await api.userExternalIdGet(body);
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

[**UserExternalId**](UserExternalId.md)

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


## userExternalIdSearch

> UserExternalIdPaginationResponse userExternalIdSearch(filter, query, page, perPage, sort)



Search user external ids.

### Example

```ts
import {
  Configuration,
  UserExternalIdApi,
} from '@statflo/statflo-typescript-sdk';
import type { UserExternalIdSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UserExternalIdApi(config);

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
  } satisfies UserExternalIdSearchRequest;

  try {
    const data = await api.userExternalIdSearch(body);
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

[**UserExternalIdPaginationResponse**](UserExternalIdPaginationResponse.md)

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


## userExternalIdUpdate

> UserExternalId userExternalIdUpdate(id, userExternalIdUpdate)



Update a user external id.

### Example

```ts
import {
  Configuration,
  UserExternalIdApi,
} from '@statflo/statflo-typescript-sdk';
import type { UserExternalIdUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UserExternalIdApi(config);

  const body = {
    // string
    id: id_example,
    // UserExternalIdUpdate (optional)
    userExternalIdUpdate: ...,
  } satisfies UserExternalIdUpdateRequest;

  try {
    const data = await api.userExternalIdUpdate(body);
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
| **userExternalIdUpdate** | [UserExternalIdUpdate](UserExternalIdUpdate.md) |  | [Optional] |

### Return type

[**UserExternalId**](UserExternalId.md)

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

