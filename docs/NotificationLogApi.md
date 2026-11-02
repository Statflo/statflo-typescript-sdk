# NotificationLogApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**notificationLogCreate**](NotificationLogApi.md#notificationlogcreate) | **POST** /v4/api/notification-log |  |
| [**notificationLogDelete**](NotificationLogApi.md#notificationlogdelete) | **DELETE** /v4/api/notification-log/{id} |  |
| [**notificationLogGet**](NotificationLogApi.md#notificationlogget) | **GET** /v4/api/notification-log/{id} |  |
| [**notificationLogSearch**](NotificationLogApi.md#notificationlogsearch) | **GET** /v4/api/notification-log |  |



## notificationLogCreate

> NotificationLog notificationLogCreate(notificationLogCreate)



Create notification log.

### Example

```ts
import {
  Configuration,
  NotificationLogApi,
} from '@statflo/statflo-typescript-sdk';
import type { NotificationLogCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new NotificationLogApi(config);

  const body = {
    // NotificationLogCreate (optional)
    notificationLogCreate: ...,
  } satisfies NotificationLogCreateRequest;

  try {
    const data = await api.notificationLogCreate(body);
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
| **notificationLogCreate** | [NotificationLogCreate](NotificationLogCreate.md) |  | [Optional] |

### Return type

[**NotificationLog**](NotificationLog.md)

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


## notificationLogDelete

> notificationLogDelete(id)



Remove notification log.

### Example

```ts
import {
  Configuration,
  NotificationLogApi,
} from '@statflo/statflo-typescript-sdk';
import type { NotificationLogDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new NotificationLogApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies NotificationLogDeleteRequest;

  try {
    const data = await api.notificationLogDelete(body);
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


## notificationLogGet

> NotificationLog notificationLogGet(id)



Retrieve notification log.

### Example

```ts
import {
  Configuration,
  NotificationLogApi,
} from '@statflo/statflo-typescript-sdk';
import type { NotificationLogGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new NotificationLogApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies NotificationLogGetRequest;

  try {
    const data = await api.notificationLogGet(body);
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

[**NotificationLog**](NotificationLog.md)

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


## notificationLogSearch

> NotificationLogPaginationResponse notificationLogSearch(filter, query, page, perPage, sort)



Search notificationLogs.

### Example

```ts
import {
  Configuration,
  NotificationLogApi,
} from '@statflo/statflo-typescript-sdk';
import type { NotificationLogSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new NotificationLogApi(config);

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
  } satisfies NotificationLogSearchRequest;

  try {
    const data = await api.notificationLogSearch(body);
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

[**NotificationLogPaginationResponse**](NotificationLogPaginationResponse.md)

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

