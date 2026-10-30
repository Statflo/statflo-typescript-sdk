# AccountContactMetadataApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**accountContactMetadataCreate**](AccountContactMetadataApi.md#accountcontactmetadatacreate) | **POST** /v4/api/account-contact-metadata |  |
| [**accountContactMetadataDelete**](AccountContactMetadataApi.md#accountcontactmetadatadelete) | **DELETE** /v4/api/account-contact-metadata/{id} |  |
| [**accountContactMetadataGet**](AccountContactMetadataApi.md#accountcontactmetadataget) | **GET** /v4/api/account-contact-metadata/{id} |  |
| [**accountContactMetadataSearch**](AccountContactMetadataApi.md#accountcontactmetadatasearch) | **GET** /v4/api/account-contact-metadata |  |
| [**accountContactMetadataUpdate**](AccountContactMetadataApi.md#accountcontactmetadataupdate) | **PUT** /v4/api/account-contact-metadata/{id} |  |



## accountContactMetadataCreate

> AccountContactMetadata accountContactMetadataCreate(accountContactMetadataCreate)



Create a account contact metadata.

### Example

```ts
import {
  Configuration,
  AccountContactMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountContactMetadataCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountContactMetadataApi(config);

  const body = {
    // AccountContactMetadataCreate (optional)
    accountContactMetadataCreate: ...,
  } satisfies AccountContactMetadataCreateRequest;

  try {
    const data = await api.accountContactMetadataCreate(body);
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
| **accountContactMetadataCreate** | [AccountContactMetadataCreate](AccountContactMetadataCreate.md) |  | [Optional] |

### Return type

[**AccountContactMetadata**](AccountContactMetadata.md)

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


## accountContactMetadataDelete

> accountContactMetadataDelete(id)



Remove a account contact metadata.

### Example

```ts
import {
  Configuration,
  AccountContactMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountContactMetadataDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountContactMetadataApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies AccountContactMetadataDeleteRequest;

  try {
    const data = await api.accountContactMetadataDelete(body);
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


## accountContactMetadataGet

> AccountContactMetadata accountContactMetadataGet(id)



Retrieve a account contact metadata.

### Example

```ts
import {
  Configuration,
  AccountContactMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountContactMetadataGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountContactMetadataApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies AccountContactMetadataGetRequest;

  try {
    const data = await api.accountContactMetadataGet(body);
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

[**AccountContactMetadata**](AccountContactMetadata.md)

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


## accountContactMetadataSearch

> AccountContactMetadataPaginationResponse accountContactMetadataSearch(filter, query, page, perPage, sort)



Search account contact metadata.

### Example

```ts
import {
  Configuration,
  AccountContactMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountContactMetadataSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountContactMetadataApi(config);

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
  } satisfies AccountContactMetadataSearchRequest;

  try {
    const data = await api.accountContactMetadataSearch(body);
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

[**AccountContactMetadataPaginationResponse**](AccountContactMetadataPaginationResponse.md)

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


## accountContactMetadataUpdate

> AccountContactMetadata accountContactMetadataUpdate(id, accountContactMetadataUpdate)



Update a account contact metadata.

### Example

```ts
import {
  Configuration,
  AccountContactMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountContactMetadataUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountContactMetadataApi(config);

  const body = {
    // string
    id: id_example,
    // AccountContactMetadataUpdate (optional)
    accountContactMetadataUpdate: ...,
  } satisfies AccountContactMetadataUpdateRequest;

  try {
    const data = await api.accountContactMetadataUpdate(body);
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
| **accountContactMetadataUpdate** | [AccountContactMetadataUpdate](AccountContactMetadataUpdate.md) |  | [Optional] |

### Return type

[**AccountContactMetadata**](AccountContactMetadata.md)

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

