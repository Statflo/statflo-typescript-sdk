# ContactConsentLogApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**contactConsentLogCreate**](ContactConsentLogApi.md#contactconsentlogcreate) | **POST** /v4/api/contact-consent-log |  |
| [**contactConsentLogDelete**](ContactConsentLogApi.md#contactconsentlogdelete) | **DELETE** /v4/api/contact-consent-log/{id} |  |
| [**contactConsentLogGet**](ContactConsentLogApi.md#contactconsentlogget) | **GET** /v4/api/contact-consent-log/{id} |  |
| [**contactConsentLogSearch**](ContactConsentLogApi.md#contactconsentlogsearch) | **GET** /v4/api/contact-consent-log |  |
| [**contactConsentLogUpdate**](ContactConsentLogApi.md#contactconsentlogupdate) | **PUT** /v4/api/contact-consent-log/{id} |  |



## contactConsentLogCreate

> ContactConsentLog contactConsentLogCreate(contactConsentLogCreate)



Create contact consent log.

### Example

```ts
import {
  Configuration,
  ContactConsentLogApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContactConsentLogCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContactConsentLogApi(config);

  const body = {
    // ContactConsentLogCreate (optional)
    contactConsentLogCreate: ...,
  } satisfies ContactConsentLogCreateRequest;

  try {
    const data = await api.contactConsentLogCreate(body);
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
| **contactConsentLogCreate** | [ContactConsentLogCreate](ContactConsentLogCreate.md) |  | [Optional] |

### Return type

[**ContactConsentLog**](ContactConsentLog.md)

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


## contactConsentLogDelete

> contactConsentLogDelete(id)



Remove contact consent log.

### Example

```ts
import {
  Configuration,
  ContactConsentLogApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContactConsentLogDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContactConsentLogApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies ContactConsentLogDeleteRequest;

  try {
    const data = await api.contactConsentLogDelete(body);
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


## contactConsentLogGet

> ContactConsentLog contactConsentLogGet(id)



Retrieve contact consent log.

### Example

```ts
import {
  Configuration,
  ContactConsentLogApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContactConsentLogGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContactConsentLogApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies ContactConsentLogGetRequest;

  try {
    const data = await api.contactConsentLogGet(body);
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

[**ContactConsentLog**](ContactConsentLog.md)

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


## contactConsentLogSearch

> ContactConsentLogPaginationResponse contactConsentLogSearch(filter, query, page, perPage, sort)



Search contact consent logs.

### Example

```ts
import {
  Configuration,
  ContactConsentLogApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContactConsentLogSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContactConsentLogApi(config);

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
  } satisfies ContactConsentLogSearchRequest;

  try {
    const data = await api.contactConsentLogSearch(body);
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

[**ContactConsentLogPaginationResponse**](ContactConsentLogPaginationResponse.md)

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


## contactConsentLogUpdate

> ContactConsentLog contactConsentLogUpdate(id, contactConsentLogUpdate)



Update contact consent log.

### Example

```ts
import {
  Configuration,
  ContactConsentLogApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContactConsentLogUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContactConsentLogApi(config);

  const body = {
    // string
    id: id_example,
    // ContactConsentLogUpdate (optional)
    contactConsentLogUpdate: ...,
  } satisfies ContactConsentLogUpdateRequest;

  try {
    const data = await api.contactConsentLogUpdate(body);
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
| **contactConsentLogUpdate** | [ContactConsentLogUpdate](ContactConsentLogUpdate.md) |  | [Optional] |

### Return type

[**ContactConsentLog**](ContactConsentLog.md)

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

