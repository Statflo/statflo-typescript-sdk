# EWCAcceptanceApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**ewcAcceptanceCreate**](EWCAcceptanceApi.md#ewcacceptancecreate) | **POST** /v4/api/ewc-acceptance |  |
| [**ewcAcceptanceDelete**](EWCAcceptanceApi.md#ewcacceptancedelete) | **DELETE** /v4/api/ewc-acceptance/{id} |  |
| [**ewcAcceptanceGet**](EWCAcceptanceApi.md#ewcacceptanceget) | **GET** /v4/api/ewc-acceptance/{id} |  |
| [**ewcAcceptanceSearch**](EWCAcceptanceApi.md#ewcacceptancesearch) | **GET** /v4/api/ewc-acceptance |  |
| [**ewcAcceptanceUpdate**](EWCAcceptanceApi.md#ewcacceptanceupdate) | **PUT** /v4/api/ewc-acceptance/{id} |  |



## ewcAcceptanceCreate

> EwcAcceptance ewcAcceptanceCreate(ewcAcceptanceCreate)



Create EWC acceptance

### Example

```ts
import {
  Configuration,
  EWCAcceptanceApi,
} from '@statflo/statflo-typescript-sdk';
import type { EwcAcceptanceCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EWCAcceptanceApi(config);

  const body = {
    // EwcAcceptanceCreate (optional)
    ewcAcceptanceCreate: ...,
  } satisfies EwcAcceptanceCreateRequest;

  try {
    const data = await api.ewcAcceptanceCreate(body);
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
| **ewcAcceptanceCreate** | [EwcAcceptanceCreate](EwcAcceptanceCreate.md) |  | [Optional] |

### Return type

[**EwcAcceptance**](EwcAcceptance.md)

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


## ewcAcceptanceDelete

> ewcAcceptanceDelete(id)



Remove an EWC acceptance

### Example

```ts
import {
  Configuration,
  EWCAcceptanceApi,
} from '@statflo/statflo-typescript-sdk';
import type { EwcAcceptanceDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EWCAcceptanceApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies EwcAcceptanceDeleteRequest;

  try {
    const data = await api.ewcAcceptanceDelete(body);
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


## ewcAcceptanceGet

> EwcAcceptance ewcAcceptanceGet(id)



Retrieve an EWC acceptance

### Example

```ts
import {
  Configuration,
  EWCAcceptanceApi,
} from '@statflo/statflo-typescript-sdk';
import type { EwcAcceptanceGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EWCAcceptanceApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies EwcAcceptanceGetRequest;

  try {
    const data = await api.ewcAcceptanceGet(body);
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

[**EwcAcceptance**](EwcAcceptance.md)

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


## ewcAcceptanceSearch

> EwcAcceptancePaginationResponse ewcAcceptanceSearch(filter, query, page, perPage, sort)



Search EWC acceptance

### Example

```ts
import {
  Configuration,
  EWCAcceptanceApi,
} from '@statflo/statflo-typescript-sdk';
import type { EwcAcceptanceSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EWCAcceptanceApi(config);

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
  } satisfies EwcAcceptanceSearchRequest;

  try {
    const data = await api.ewcAcceptanceSearch(body);
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

[**EwcAcceptancePaginationResponse**](EwcAcceptancePaginationResponse.md)

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


## ewcAcceptanceUpdate

> EwcAcceptance ewcAcceptanceUpdate(id, ewcAcceptanceUpdate)



Update an EWC acceptance

### Example

```ts
import {
  Configuration,
  EWCAcceptanceApi,
} from '@statflo/statflo-typescript-sdk';
import type { EwcAcceptanceUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EWCAcceptanceApi(config);

  const body = {
    // string
    id: id_example,
    // EwcAcceptanceUpdate (optional)
    ewcAcceptanceUpdate: ...,
  } satisfies EwcAcceptanceUpdateRequest;

  try {
    const data = await api.ewcAcceptanceUpdate(body);
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
| **ewcAcceptanceUpdate** | [EwcAcceptanceUpdate](EwcAcceptanceUpdate.md) |  | [Optional] |

### Return type

[**EwcAcceptance**](EwcAcceptance.md)

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

