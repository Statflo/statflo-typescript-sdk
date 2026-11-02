# TimelineApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**timelineCreate**](TimelineApi.md#timelinecreate) | **POST** /v4/api/timeline |  |
| [**timelineDelete**](TimelineApi.md#timelinedelete) | **DELETE** /v4/api/timeline/{id} |  |
| [**timelineGet**](TimelineApi.md#timelineget) | **GET** /v4/api/timeline/{id} |  |
| [**timelineSearch**](TimelineApi.md#timelinesearch) | **GET** /v4/api/timeline |  |
| [**timelineUpdate**](TimelineApi.md#timelineupdate) | **PUT** /v4/api/timeline/{id} |  |



## timelineCreate

> Timeline timelineCreate(timelineCreate)



Create an timeline.

### Example

```ts
import {
  Configuration,
  TimelineApi,
} from '@statflo/statflo-typescript-sdk';
import type { TimelineCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TimelineApi(config);

  const body = {
    // TimelineCreate (optional)
    timelineCreate: ...,
  } satisfies TimelineCreateRequest;

  try {
    const data = await api.timelineCreate(body);
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
| **timelineCreate** | [TimelineCreate](TimelineCreate.md) |  | [Optional] |

### Return type

[**Timeline**](Timeline.md)

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


## timelineDelete

> timelineDelete(id)



Remove an timeline.

### Example

```ts
import {
  Configuration,
  TimelineApi,
} from '@statflo/statflo-typescript-sdk';
import type { TimelineDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TimelineApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies TimelineDeleteRequest;

  try {
    const data = await api.timelineDelete(body);
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


## timelineGet

> Timeline timelineGet(id)



Retrieve an timeline.

### Example

```ts
import {
  Configuration,
  TimelineApi,
} from '@statflo/statflo-typescript-sdk';
import type { TimelineGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TimelineApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies TimelineGetRequest;

  try {
    const data = await api.timelineGet(body);
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

[**Timeline**](Timeline.md)

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


## timelineSearch

> TimelinePaginationResponse timelineSearch(filter, query, page, perPage, sort)



Search timelines.

### Example

```ts
import {
  Configuration,
  TimelineApi,
} from '@statflo/statflo-typescript-sdk';
import type { TimelineSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TimelineApi(config);

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
  } satisfies TimelineSearchRequest;

  try {
    const data = await api.timelineSearch(body);
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

[**TimelinePaginationResponse**](TimelinePaginationResponse.md)

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


## timelineUpdate

> Timeline timelineUpdate(id, timelineUpdate)



Update an timeline.

### Example

```ts
import {
  Configuration,
  TimelineApi,
} from '@statflo/statflo-typescript-sdk';
import type { TimelineUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TimelineApi(config);

  const body = {
    // string
    id: id_example,
    // TimelineUpdate (optional)
    timelineUpdate: ...,
  } satisfies TimelineUpdateRequest;

  try {
    const data = await api.timelineUpdate(body);
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
| **timelineUpdate** | [TimelineUpdate](TimelineUpdate.md) |  | [Optional] |

### Return type

[**Timeline**](Timeline.md)

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

