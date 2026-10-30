# AccountNumberApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**accountNumberCreate**](AccountNumberApi.md#accountnumbercreate) | **POST** /v4/api/account-number |  |
| [**accountNumberGet**](AccountNumberApi.md#accountnumberget) | **GET** /v4/api/account-number/{id} |  |
| [**accountNumberSearch**](AccountNumberApi.md#accountnumbersearch) | **GET** /v4/api/account-number |  |
| [**accountNumberUpdate**](AccountNumberApi.md#accountnumberupdate) | **PUT** /v4/api/account-number/{id} |  |



## accountNumberCreate

> AccountNumber accountNumberCreate(accountNumberCreate)



Create a account number.

### Example

```ts
import {
  Configuration,
  AccountNumberApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountNumberCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountNumberApi(config);

  const body = {
    // AccountNumberCreate (optional)
    accountNumberCreate: ...,
  } satisfies AccountNumberCreateRequest;

  try {
    const data = await api.accountNumberCreate(body);
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
| **accountNumberCreate** | [AccountNumberCreate](AccountNumberCreate.md) |  | [Optional] |

### Return type

[**AccountNumber**](AccountNumber.md)

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


## accountNumberGet

> AccountNumber accountNumberGet(id)



Retrieve a message template.

### Example

```ts
import {
  Configuration,
  AccountNumberApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountNumberGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountNumberApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies AccountNumberGetRequest;

  try {
    const data = await api.accountNumberGet(body);
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

[**AccountNumber**](AccountNumber.md)

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


## accountNumberSearch

> AccountNumberPaginationResponse accountNumberSearch(filter, query, page, perPage, sort)



Search Account Number.

### Example

```ts
import {
  Configuration,
  AccountNumberApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountNumberSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountNumberApi(config);

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
  } satisfies AccountNumberSearchRequest;

  try {
    const data = await api.accountNumberSearch(body);
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

[**AccountNumberPaginationResponse**](AccountNumberPaginationResponse.md)

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


## accountNumberUpdate

> AccountNumber accountNumberUpdate(id, accountNumberUpdate)



Update a account number.

### Example

```ts
import {
  Configuration,
  AccountNumberApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountNumberUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountNumberApi(config);

  const body = {
    // string
    id: id_example,
    // AccountNumberUpdate (optional)
    accountNumberUpdate: ...,
  } satisfies AccountNumberUpdateRequest;

  try {
    const data = await api.accountNumberUpdate(body);
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
| **accountNumberUpdate** | [AccountNumberUpdate](AccountNumberUpdate.md) |  | [Optional] |

### Return type

[**AccountNumber**](AccountNumber.md)

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

