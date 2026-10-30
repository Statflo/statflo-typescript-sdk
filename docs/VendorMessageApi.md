# VendorMessageApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**vendorMessageCreate**](VendorMessageApi.md#vendormessagecreate) | **POST** /v4/api/vendor-message |  |
| [**vendorMessageGet**](VendorMessageApi.md#vendormessageget) | **GET** /v4/api/vendor-message/{id} |  |
| [**vendorMessageSearch**](VendorMessageApi.md#vendormessagesearch) | **GET** /v4/api/vendor-message |  |



## vendorMessageCreate

> VendorMessage vendorMessageCreate(vendorMessageCreate)



Create a message template.

### Example

```ts
import {
  Configuration,
  VendorMessageApi,
} from '@statflo/statflo-typescript-sdk';
import type { VendorMessageCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VendorMessageApi(config);

  const body = {
    // VendorMessageCreate (optional)
    vendorMessageCreate: ...,
  } satisfies VendorMessageCreateRequest;

  try {
    const data = await api.vendorMessageCreate(body);
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
| **vendorMessageCreate** | [VendorMessageCreate](VendorMessageCreate.md) |  | [Optional] |

### Return type

[**VendorMessage**](VendorMessage.md)

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


## vendorMessageGet

> VendorMessage vendorMessageGet(id)



Retrieve a message template.

### Example

```ts
import {
  Configuration,
  VendorMessageApi,
} from '@statflo/statflo-typescript-sdk';
import type { VendorMessageGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VendorMessageApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies VendorMessageGetRequest;

  try {
    const data = await api.vendorMessageGet(body);
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

[**VendorMessage**](VendorMessage.md)

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


## vendorMessageSearch

> VendorMessagePaginationResponse vendorMessageSearch(filter, query, page, perPage, sort)



Search vendor messages.

### Example

```ts
import {
  Configuration,
  VendorMessageApi,
} from '@statflo/statflo-typescript-sdk';
import type { VendorMessageSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new VendorMessageApi(config);

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
  } satisfies VendorMessageSearchRequest;

  try {
    const data = await api.vendorMessageSearch(body);
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

[**VendorMessagePaginationResponse**](VendorMessagePaginationResponse.md)

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

