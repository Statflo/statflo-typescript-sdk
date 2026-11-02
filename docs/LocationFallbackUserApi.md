# LocationFallbackUserApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**locationFallbackUserCreate**](LocationFallbackUserApi.md#locationfallbackusercreate) | **POST** /v4/api/location-fallback-user |  |
| [**locationFallbackUserDelete**](LocationFallbackUserApi.md#locationfallbackuserdelete) | **DELETE** /v4/api/location-fallback-user/{id} |  |
| [**locationFallbackUserGet**](LocationFallbackUserApi.md#locationfallbackuserget) | **GET** /v4/api/location-fallback-user/{id} |  |
| [**locationFallbackUserSearch**](LocationFallbackUserApi.md#locationfallbackusersearch) | **GET** /v4/api/location-fallback-user |  |
| [**locationFallbackUserUpdate**](LocationFallbackUserApi.md#locationfallbackuserupdate) | **PUT** /v4/api/location-fallback-user/{id} |  |



## locationFallbackUserCreate

> LocationFallbackUser locationFallbackUserCreate(locationFallbackUserCreate)



Create a location fallback user.

### Example

```ts
import {
  Configuration,
  LocationFallbackUserApi,
} from '@statflo/statflo-typescript-sdk';
import type { LocationFallbackUserCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LocationFallbackUserApi(config);

  const body = {
    // LocationFallbackUserCreate (optional)
    locationFallbackUserCreate: ...,
  } satisfies LocationFallbackUserCreateRequest;

  try {
    const data = await api.locationFallbackUserCreate(body);
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
| **locationFallbackUserCreate** | [LocationFallbackUserCreate](LocationFallbackUserCreate.md) |  | [Optional] |

### Return type

[**LocationFallbackUser**](LocationFallbackUser.md)

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


## locationFallbackUserDelete

> locationFallbackUserDelete(id)



Remove a location fallback user.

### Example

```ts
import {
  Configuration,
  LocationFallbackUserApi,
} from '@statflo/statflo-typescript-sdk';
import type { LocationFallbackUserDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LocationFallbackUserApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies LocationFallbackUserDeleteRequest;

  try {
    const data = await api.locationFallbackUserDelete(body);
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


## locationFallbackUserGet

> LocationFallbackUser locationFallbackUserGet(id)



Retrieve a location fallback user.

### Example

```ts
import {
  Configuration,
  LocationFallbackUserApi,
} from '@statflo/statflo-typescript-sdk';
import type { LocationFallbackUserGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LocationFallbackUserApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies LocationFallbackUserGetRequest;

  try {
    const data = await api.locationFallbackUserGet(body);
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

[**LocationFallbackUser**](LocationFallbackUser.md)

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


## locationFallbackUserSearch

> LocationFallbackUserPaginationResponse locationFallbackUserSearch(filter, query, page, perPage, sort)



Search location fallback users.

### Example

```ts
import {
  Configuration,
  LocationFallbackUserApi,
} from '@statflo/statflo-typescript-sdk';
import type { LocationFallbackUserSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LocationFallbackUserApi(config);

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
  } satisfies LocationFallbackUserSearchRequest;

  try {
    const data = await api.locationFallbackUserSearch(body);
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

[**LocationFallbackUserPaginationResponse**](LocationFallbackUserPaginationResponse.md)

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


## locationFallbackUserUpdate

> LocationFallbackUser locationFallbackUserUpdate(id, locationFallbackUserUpdate)



Update a location fallback user.

### Example

```ts
import {
  Configuration,
  LocationFallbackUserApi,
} from '@statflo/statflo-typescript-sdk';
import type { LocationFallbackUserUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new LocationFallbackUserApi(config);

  const body = {
    // string
    id: id_example,
    // LocationFallbackUserUpdate (optional)
    locationFallbackUserUpdate: ...,
  } satisfies LocationFallbackUserUpdateRequest;

  try {
    const data = await api.locationFallbackUserUpdate(body);
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
| **locationFallbackUserUpdate** | [LocationFallbackUserUpdate](LocationFallbackUserUpdate.md) |  | [Optional] |

### Return type

[**LocationFallbackUser**](LocationFallbackUser.md)

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

