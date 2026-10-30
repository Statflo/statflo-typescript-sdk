# RcsAgentMetadataApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**rcsAgentMetadataCreate**](RcsAgentMetadataApi.md#rcsagentmetadatacreate) | **POST** /v4/api/rcs-agent-metadata |  |
| [**rcsAgentMetadataDelete**](RcsAgentMetadataApi.md#rcsagentmetadatadelete) | **DELETE** /v4/api/rcs-agent-metadata/{id} |  |
| [**rcsAgentMetadataGet**](RcsAgentMetadataApi.md#rcsagentmetadataget) | **GET** /v4/api/rcs-agent-metadata/{id} |  |
| [**rcsAgentMetadataSearch**](RcsAgentMetadataApi.md#rcsagentmetadatasearch) | **GET** /v4/api/rcs-agent-metadata |  |
| [**rcsAgentMetadataUpdate**](RcsAgentMetadataApi.md#rcsagentmetadataupdate) | **PUT** /v4/api/rcs-agent-metadata/{id} |  |



## rcsAgentMetadataCreate

> RcsAgentMetadata rcsAgentMetadataCreate(rcsAgentMetadataCreate)



Create an rcs agent metadata.

### Example

```ts
import {
  Configuration,
  RcsAgentMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentMetadataCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentMetadataApi(config);

  const body = {
    // RcsAgentMetadataCreate (optional)
    rcsAgentMetadataCreate: ...,
  } satisfies RcsAgentMetadataCreateRequest;

  try {
    const data = await api.rcsAgentMetadataCreate(body);
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
| **rcsAgentMetadataCreate** | [RcsAgentMetadataCreate](RcsAgentMetadataCreate.md) |  | [Optional] |

### Return type

[**RcsAgentMetadata**](RcsAgentMetadata.md)

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


## rcsAgentMetadataDelete

> rcsAgentMetadataDelete(id)



Remove an rcs agent metadata.

### Example

```ts
import {
  Configuration,
  RcsAgentMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentMetadataDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentMetadataApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies RcsAgentMetadataDeleteRequest;

  try {
    const data = await api.rcsAgentMetadataDelete(body);
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


## rcsAgentMetadataGet

> RcsAgentMetadata rcsAgentMetadataGet(id)



Retrieve an rcs agent metadata.

### Example

```ts
import {
  Configuration,
  RcsAgentMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentMetadataGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentMetadataApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies RcsAgentMetadataGetRequest;

  try {
    const data = await api.rcsAgentMetadataGet(body);
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

[**RcsAgentMetadata**](RcsAgentMetadata.md)

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


## rcsAgentMetadataSearch

> RcsAgentMetadataPaginationResponse rcsAgentMetadataSearch(filter, query, page, perPage, sort)



Search rcs agent metadata.

### Example

```ts
import {
  Configuration,
  RcsAgentMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentMetadataSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentMetadataApi(config);

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
  } satisfies RcsAgentMetadataSearchRequest;

  try {
    const data = await api.rcsAgentMetadataSearch(body);
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

[**RcsAgentMetadataPaginationResponse**](RcsAgentMetadataPaginationResponse.md)

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


## rcsAgentMetadataUpdate

> RcsAgentMetadata rcsAgentMetadataUpdate(id, rcsAgentMetadataUpdate)



Update an rcs agent metadata.

### Example

```ts
import {
  Configuration,
  RcsAgentMetadataApi,
} from '@statflo/statflo-typescript-sdk';
import type { RcsAgentMetadataUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new RcsAgentMetadataApi(config);

  const body = {
    // string
    id: id_example,
    // RcsAgentMetadataUpdate (optional)
    rcsAgentMetadataUpdate: ...,
  } satisfies RcsAgentMetadataUpdateRequest;

  try {
    const data = await api.rcsAgentMetadataUpdate(body);
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
| **rcsAgentMetadataUpdate** | [RcsAgentMetadataUpdate](RcsAgentMetadataUpdate.md) |  | [Optional] |

### Return type

[**RcsAgentMetadata**](RcsAgentMetadata.md)

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

