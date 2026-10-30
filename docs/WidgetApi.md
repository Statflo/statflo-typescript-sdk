# WidgetApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getV4ApiWidgetsCampaigns**](WidgetApi.md#getv4apiwidgetscampaigns) | **GET** /v4/api/widgets/campaigns/{accountId} |  |
| [**widgetCreate**](WidgetApi.md#widgetcreate) | **POST** /v4/api/widget |  |
| [**widgetDelete**](WidgetApi.md#widgetdelete) | **DELETE** /v4/api/widget/{id} |  |
| [**widgetGet**](WidgetApi.md#widgetget) | **GET** /v4/api/widget/{id} |  |
| [**widgetSearch**](WidgetApi.md#widgetsearch) | **GET** /v4/api/widget |  |
| [**widgetUpdate**](WidgetApi.md#widgetupdate) | **PUT** /v4/api/widget/{id} |  |



## getV4ApiWidgetsCampaigns

> getV4ApiWidgetsCampaigns(accountId)



### Example

```ts
import {
  Configuration,
  WidgetApi,
} from '@statflo/statflo-typescript-sdk';
import type { GetV4ApiWidgetsCampaignsRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WidgetApi(config);

  const body = {
    // string
    accountId: accountId_example,
  } satisfies GetV4ApiWidgetsCampaignsRequest;

  try {
    const data = await api.getV4ApiWidgetsCampaigns(body);
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
| **accountId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## widgetCreate

> Widget widgetCreate(widgetCreate)



Create a widget.

### Example

```ts
import {
  Configuration,
  WidgetApi,
} from '@statflo/statflo-typescript-sdk';
import type { WidgetCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WidgetApi(config);

  const body = {
    // WidgetCreate (optional)
    widgetCreate: ...,
  } satisfies WidgetCreateRequest;

  try {
    const data = await api.widgetCreate(body);
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
| **widgetCreate** | [WidgetCreate](WidgetCreate.md) |  | [Optional] |

### Return type

[**Widget**](Widget.md)

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


## widgetDelete

> widgetDelete(id)



Remove a widget.

### Example

```ts
import {
  Configuration,
  WidgetApi,
} from '@statflo/statflo-typescript-sdk';
import type { WidgetDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WidgetApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies WidgetDeleteRequest;

  try {
    const data = await api.widgetDelete(body);
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


## widgetGet

> Widget widgetGet(id)



Retrieve a widget.

### Example

```ts
import {
  Configuration,
  WidgetApi,
} from '@statflo/statflo-typescript-sdk';
import type { WidgetGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WidgetApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies WidgetGetRequest;

  try {
    const data = await api.widgetGet(body);
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

[**Widget**](Widget.md)

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


## widgetSearch

> WidgetPaginationResponse widgetSearch(filter, query, page, perPage, sort)



Search widgets.

### Example

```ts
import {
  Configuration,
  WidgetApi,
} from '@statflo/statflo-typescript-sdk';
import type { WidgetSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WidgetApi(config);

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
  } satisfies WidgetSearchRequest;

  try {
    const data = await api.widgetSearch(body);
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

[**WidgetPaginationResponse**](WidgetPaginationResponse.md)

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


## widgetUpdate

> Widget widgetUpdate(id, widgetUpdate)



Update a widget.

### Example

```ts
import {
  Configuration,
  WidgetApi,
} from '@statflo/statflo-typescript-sdk';
import type { WidgetUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new WidgetApi(config);

  const body = {
    // string
    id: id_example,
    // WidgetUpdate (optional)
    widgetUpdate: ...,
  } satisfies WidgetUpdateRequest;

  try {
    const data = await api.widgetUpdate(body);
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
| **widgetUpdate** | [WidgetUpdate](WidgetUpdate.md) |  | [Optional] |

### Return type

[**Widget**](Widget.md)

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

