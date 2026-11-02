# EmailActivityApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**emailActivityCreate**](EmailActivityApi.md#emailactivitycreate) | **POST** /v4/api/email-activity |  |
| [**emailActivityDelete**](EmailActivityApi.md#emailactivitydelete) | **DELETE** /v4/api/email-activity/{id} |  |
| [**emailActivityGet**](EmailActivityApi.md#emailactivityget) | **GET** /v4/api/email-activity/{id} |  |
| [**emailActivitySearch**](EmailActivityApi.md#emailactivitysearch) | **GET** /v4/api/email-activity |  |
| [**emailActivityUpdate**](EmailActivityApi.md#emailactivityupdate) | **PUT** /v4/api/email-activity/{id} |  |



## emailActivityCreate

> EmailActivity emailActivityCreate(emailActivityCreate)



Create email activity

### Example

```ts
import {
  Configuration,
  EmailActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { EmailActivityCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmailActivityApi(config);

  const body = {
    // EmailActivityCreate (optional)
    emailActivityCreate: ...,
  } satisfies EmailActivityCreateRequest;

  try {
    const data = await api.emailActivityCreate(body);
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
| **emailActivityCreate** | [EmailActivityCreate](EmailActivityCreate.md) |  | [Optional] |

### Return type

[**EmailActivity**](EmailActivity.md)

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


## emailActivityDelete

> emailActivityDelete(id)



Remove an email activity

### Example

```ts
import {
  Configuration,
  EmailActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { EmailActivityDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmailActivityApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies EmailActivityDeleteRequest;

  try {
    const data = await api.emailActivityDelete(body);
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


## emailActivityGet

> EmailActivity emailActivityGet(id)



Retrieve an email activity

### Example

```ts
import {
  Configuration,
  EmailActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { EmailActivityGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmailActivityApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies EmailActivityGetRequest;

  try {
    const data = await api.emailActivityGet(body);
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

[**EmailActivity**](EmailActivity.md)

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


## emailActivitySearch

> EmailActivityPaginationResponse emailActivitySearch(filter, query, page, perPage, sort)



Search email activity

### Example

```ts
import {
  Configuration,
  EmailActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { EmailActivitySearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmailActivityApi(config);

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
  } satisfies EmailActivitySearchRequest;

  try {
    const data = await api.emailActivitySearch(body);
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

[**EmailActivityPaginationResponse**](EmailActivityPaginationResponse.md)

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


## emailActivityUpdate

> EmailActivity emailActivityUpdate(id, emailActivityUpdate)



Update an email activity

### Example

```ts
import {
  Configuration,
  EmailActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { EmailActivityUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EmailActivityApi(config);

  const body = {
    // string
    id: id_example,
    // EmailActivityUpdate (optional)
    emailActivityUpdate: ...,
  } satisfies EmailActivityUpdateRequest;

  try {
    const data = await api.emailActivityUpdate(body);
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
| **emailActivityUpdate** | [EmailActivityUpdate](EmailActivityUpdate.md) |  | [Optional] |

### Return type

[**EmailActivity**](EmailActivity.md)

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

