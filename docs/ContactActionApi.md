# ContactActionApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**contactActionCreate**](ContactActionApi.md#contactactioncreate) | **POST** /v4/api/contact-action |  |
| [**contactActionDelete**](ContactActionApi.md#contactactiondelete) | **DELETE** /v4/api/contact-action/{id} |  |
| [**contactActionGet**](ContactActionApi.md#contactactionget) | **GET** /v4/api/contact-action/{id} |  |
| [**contactActionSearch**](ContactActionApi.md#contactactionsearch) | **GET** /v4/api/contact-action |  |
| [**contactActionUpdate**](ContactActionApi.md#contactactionupdate) | **PUT** /v4/api/contact-action/{id} |  |



## contactActionCreate

> ContactAction contactActionCreate(contactActionCreate)



Create a contact action.

### Example

```ts
import {
  Configuration,
  ContactActionApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContactActionCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContactActionApi(config);

  const body = {
    // ContactActionCreate (optional)
    contactActionCreate: ...,
  } satisfies ContactActionCreateRequest;

  try {
    const data = await api.contactActionCreate(body);
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
| **contactActionCreate** | [ContactActionCreate](ContactActionCreate.md) |  | [Optional] |

### Return type

[**ContactAction**](ContactAction.md)

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


## contactActionDelete

> contactActionDelete(id)



Remove a contact action.

### Example

```ts
import {
  Configuration,
  ContactActionApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContactActionDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContactActionApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies ContactActionDeleteRequest;

  try {
    const data = await api.contactActionDelete(body);
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


## contactActionGet

> ContactAction contactActionGet(id)



Retrieve a contact action.

### Example

```ts
import {
  Configuration,
  ContactActionApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContactActionGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContactActionApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies ContactActionGetRequest;

  try {
    const data = await api.contactActionGet(body);
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

[**ContactAction**](ContactAction.md)

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


## contactActionSearch

> ContactActionPaginationResponse contactActionSearch(filter, query, page, perPage, sort)



Search contact actions.

### Example

```ts
import {
  Configuration,
  ContactActionApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContactActionSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContactActionApi(config);

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
  } satisfies ContactActionSearchRequest;

  try {
    const data = await api.contactActionSearch(body);
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

[**ContactActionPaginationResponse**](ContactActionPaginationResponse.md)

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


## contactActionUpdate

> ContactAction contactActionUpdate(id, contactActionUpdate)



Update a contact action.

### Example

```ts
import {
  Configuration,
  ContactActionApi,
} from '@statflo/statflo-typescript-sdk';
import type { ContactActionUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new ContactActionApi(config);

  const body = {
    // string
    id: id_example,
    // ContactActionUpdate (optional)
    contactActionUpdate: ...,
  } satisfies ContactActionUpdateRequest;

  try {
    const data = await api.contactActionUpdate(body);
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
| **contactActionUpdate** | [ContactActionUpdate](ContactActionUpdate.md) |  | [Optional] |

### Return type

[**ContactAction**](ContactAction.md)

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

