# SmsActivityApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**smsActivityCreate**](SmsActivityApi.md#smsactivitycreate) | **POST** /v4/api/sms-activity |  |
| [**smsActivityDelete**](SmsActivityApi.md#smsactivitydelete) | **DELETE** /v4/api/sms-activity/{id} |  |
| [**smsActivityGet**](SmsActivityApi.md#smsactivityget) | **GET** /v4/api/sms-activity/{id} |  |
| [**smsActivitySearch**](SmsActivityApi.md#smsactivitysearch) | **GET** /v4/api/sms-activity |  |
| [**smsActivityUpdate**](SmsActivityApi.md#smsactivityupdate) | **PUT** /v4/api/sms-activity/{id} |  |



## smsActivityCreate

> SmsActivity smsActivityCreate(smsActivityCreate)



Create sms activity

### Example

```ts
import {
  Configuration,
  SmsActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { SmsActivityCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SmsActivityApi(config);

  const body = {
    // SmsActivityCreate (optional)
    smsActivityCreate: ...,
  } satisfies SmsActivityCreateRequest;

  try {
    const data = await api.smsActivityCreate(body);
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
| **smsActivityCreate** | [SmsActivityCreate](SmsActivityCreate.md) |  | [Optional] |

### Return type

[**SmsActivity**](SmsActivity.md)

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


## smsActivityDelete

> smsActivityDelete(id)



Remove an sms activity

### Example

```ts
import {
  Configuration,
  SmsActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { SmsActivityDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SmsActivityApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies SmsActivityDeleteRequest;

  try {
    const data = await api.smsActivityDelete(body);
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


## smsActivityGet

> SmsActivity smsActivityGet(id)



Retrieve an sms activity

### Example

```ts
import {
  Configuration,
  SmsActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { SmsActivityGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SmsActivityApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies SmsActivityGetRequest;

  try {
    const data = await api.smsActivityGet(body);
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

[**SmsActivity**](SmsActivity.md)

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


## smsActivitySearch

> SmsActivityPaginationResponse smsActivitySearch(filter, query, page, perPage, sort)



Search sms activity

### Example

```ts
import {
  Configuration,
  SmsActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { SmsActivitySearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SmsActivityApi(config);

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
  } satisfies SmsActivitySearchRequest;

  try {
    const data = await api.smsActivitySearch(body);
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

[**SmsActivityPaginationResponse**](SmsActivityPaginationResponse.md)

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


## smsActivityUpdate

> SmsActivity smsActivityUpdate(id, smsActivityUpdate)



Update an sms activity

### Example

```ts
import {
  Configuration,
  SmsActivityApi,
} from '@statflo/statflo-typescript-sdk';
import type { SmsActivityUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new SmsActivityApi(config);

  const body = {
    // string
    id: id_example,
    // SmsActivityUpdate (optional)
    smsActivityUpdate: ...,
  } satisfies SmsActivityUpdateRequest;

  try {
    const data = await api.smsActivityUpdate(body);
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
| **smsActivityUpdate** | [SmsActivityUpdate](SmsActivityUpdate.md) |  | [Optional] |

### Return type

[**SmsActivity**](SmsActivity.md)

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

