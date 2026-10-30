# AccountMemberApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**accountMemberCreate**](AccountMemberApi.md#accountmembercreate) | **POST** /v4/api/account-member |  |
| [**accountMemberDelete**](AccountMemberApi.md#accountmemberdelete) | **DELETE** /v4/api/account-member/{id} |  |
| [**accountMemberGet**](AccountMemberApi.md#accountmemberget) | **GET** /v4/api/account-member/{id} |  |
| [**accountMemberSearch**](AccountMemberApi.md#accountmembersearch) | **GET** /v4/api/account-member |  |
| [**accountMemberUpdate**](AccountMemberApi.md#accountmemberupdate) | **PUT** /v4/api/account-member/{id} |  |



## accountMemberCreate

> AccountMember accountMemberCreate(accountMemberCreate)



Create an account.

### Example

```ts
import {
  Configuration,
  AccountMemberApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountMemberCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountMemberApi(config);

  const body = {
    // AccountMemberCreate (optional)
    accountMemberCreate: ...,
  } satisfies AccountMemberCreateRequest;

  try {
    const data = await api.accountMemberCreate(body);
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
| **accountMemberCreate** | [AccountMemberCreate](AccountMemberCreate.md) |  | [Optional] |

### Return type

[**AccountMember**](AccountMember.md)

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


## accountMemberDelete

> accountMemberDelete(id)



Remove an account member.

### Example

```ts
import {
  Configuration,
  AccountMemberApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountMemberDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountMemberApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies AccountMemberDeleteRequest;

  try {
    const data = await api.accountMemberDelete(body);
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


## accountMemberGet

> AccountMember accountMemberGet(id)



Retrieve an account member.

### Example

```ts
import {
  Configuration,
  AccountMemberApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountMemberGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountMemberApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies AccountMemberGetRequest;

  try {
    const data = await api.accountMemberGet(body);
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

[**AccountMember**](AccountMember.md)

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


## accountMemberSearch

> AccountMemberPaginationResponse accountMemberSearch(filter, query, page, perPage, sort)



Search account members.

### Example

```ts
import {
  Configuration,
  AccountMemberApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountMemberSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountMemberApi(config);

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
  } satisfies AccountMemberSearchRequest;

  try {
    const data = await api.accountMemberSearch(body);
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

[**AccountMemberPaginationResponse**](AccountMemberPaginationResponse.md)

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


## accountMemberUpdate

> AccountMember accountMemberUpdate(id, accountMemberUpdate)



Update an account member.

### Example

```ts
import {
  Configuration,
  AccountMemberApi,
} from '@statflo/statflo-typescript-sdk';
import type { AccountMemberUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AccountMemberApi(config);

  const body = {
    // string
    id: id_example,
    // AccountMemberUpdate (optional)
    accountMemberUpdate: ...,
  } satisfies AccountMemberUpdateRequest;

  try {
    const data = await api.accountMemberUpdate(body);
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
| **accountMemberUpdate** | [AccountMemberUpdate](AccountMemberUpdate.md) |  | [Optional] |

### Return type

[**AccountMember**](AccountMember.md)

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

