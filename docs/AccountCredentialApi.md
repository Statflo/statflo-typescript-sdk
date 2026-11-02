# AccountCredentialApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**accountCredentialCreate**](AccountCredentialApi.md#accountcredentialcreate) | **POST** /v4/api/account-credential |  |
| [**accountCredentialGet**](AccountCredentialApi.md#accountcredentialget) | **GET** /v4/api/account-credential/{id} |  |
| [**accountCredentialSearch**](AccountCredentialApi.md#accountcredentialsearch) | **GET** /v4/api/account-credential |  |
| [**accountCredentialUpdate**](AccountCredentialApi.md#accountcredentialupdate) | **PUT** /v4/api/account-credential/{id} |  |



## accountCredentialCreate

> AccountCredential accountCredentialCreate(accountCredentialCreate)



Create a account credential.

### Example

```ts
import {
  Configuration,
  AccountCredentialApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountCredentialCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountCredentialApi(config);

  const body = {
    // AccountCredentialCreate (optional)
    accountCredentialCreate: ...,
  } satisfies AccountCredentialCreateRequest;

  try {
    const data = await api.accountCredentialCreate(body);
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
| **accountCredentialCreate** | [AccountCredentialCreate](AccountCredentialCreate.md) |  | [Optional] |

### Return type

[**AccountCredential**](AccountCredential.md)

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


## accountCredentialGet

> AccountCredential accountCredentialGet(id)



Retrieve a account credential.

### Example

```ts
import {
  Configuration,
  AccountCredentialApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountCredentialGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountCredentialApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies AccountCredentialGetRequest;

  try {
    const data = await api.accountCredentialGet(body);
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

[**AccountCredential**](AccountCredential.md)

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


## accountCredentialSearch

> AccountCredentialPaginationResponse accountCredentialSearch(filter, query, page, perPage, sort)



Search account credentials.

### Example

```ts
import {
  Configuration,
  AccountCredentialApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountCredentialSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountCredentialApi(config);

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
  } satisfies AccountCredentialSearchRequest;

  try {
    const data = await api.accountCredentialSearch(body);
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

[**AccountCredentialPaginationResponse**](AccountCredentialPaginationResponse.md)

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


## accountCredentialUpdate

> AccountCredential accountCredentialUpdate(id, accountCredentialUpdate)



Update a account credential.

### Example

```ts
import {
  Configuration,
  AccountCredentialApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountCredentialUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountCredentialApi(config);

  const body = {
    // string
    id: id_example,
    // AccountCredentialUpdate (optional)
    accountCredentialUpdate: ...,
  } satisfies AccountCredentialUpdateRequest;

  try {
    const data = await api.accountCredentialUpdate(body);
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
| **accountCredentialUpdate** | [AccountCredentialUpdate](AccountCredentialUpdate.md) |  | [Optional] |

### Return type

[**AccountCredential**](AccountCredential.md)

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

