# AppointmentLocationApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**appointmentLocationCreate**](AppointmentLocationApi.md#appointmentlocationcreate) | **POST** /v4/api/appointment-location |  |
| [**appointmentLocationDelete**](AppointmentLocationApi.md#appointmentlocationdelete) | **DELETE** /v4/api/appointment-location/{id} |  |
| [**appointmentLocationGet**](AppointmentLocationApi.md#appointmentlocationget) | **GET** /v4/api/appointment-location/{id} |  |
| [**appointmentLocationSearch**](AppointmentLocationApi.md#appointmentlocationsearch) | **GET** /v4/api/appointment-location |  |
| [**appointmentLocationUpdate**](AppointmentLocationApi.md#appointmentlocationupdate) | **PUT** /v4/api/appointment-location/{id} |  |



## appointmentLocationCreate

> AppointmentLocation appointmentLocationCreate(appointmentLocationCreate)



Create an appointment location.

### Example

```ts
import {
  Configuration,
  AppointmentLocationApi,
} from '@statflo/statflo-typescript-sdk';
import type { AppointmentLocationCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AppointmentLocationApi(config);

  const body = {
    // AppointmentLocationCreate (optional)
    appointmentLocationCreate: ...,
  } satisfies AppointmentLocationCreateRequest;

  try {
    const data = await api.appointmentLocationCreate(body);
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
| **appointmentLocationCreate** | [AppointmentLocationCreate](AppointmentLocationCreate.md) |  | [Optional] |

### Return type

[**AppointmentLocation**](AppointmentLocation.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## appointmentLocationDelete

> appointmentLocationDelete(id)



Delete an appointment location.

### Example

```ts
import {
  Configuration,
  AppointmentLocationApi,
} from '@statflo/statflo-typescript-sdk';
import type { AppointmentLocationDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AppointmentLocationApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies AppointmentLocationDeleteRequest;

  try {
    const data = await api.appointmentLocationDelete(body);
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
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **0** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## appointmentLocationGet

> AppointmentLocation appointmentLocationGet(id)



Retrieve an appointment location.

### Example

```ts
import {
  Configuration,
  AppointmentLocationApi,
} from '@statflo/statflo-typescript-sdk';
import type { AppointmentLocationGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AppointmentLocationApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies AppointmentLocationGetRequest;

  try {
    const data = await api.appointmentLocationGet(body);
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

[**AppointmentLocation**](AppointmentLocation.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## appointmentLocationSearch

> AppointmentLocationPaginationResponse appointmentLocationSearch(filter, query, page, perPage, sort)



Search appointment locations.

### Example

```ts
import {
  Configuration,
  AppointmentLocationApi,
} from '@statflo/statflo-typescript-sdk';
import type { AppointmentLocationSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AppointmentLocationApi(config);

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
  } satisfies AppointmentLocationSearchRequest;

  try {
    const data = await api.appointmentLocationSearch(body);
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

[**AppointmentLocationPaginationResponse**](AppointmentLocationPaginationResponse.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## appointmentLocationUpdate

> AppointmentLocation appointmentLocationUpdate(id, appointmentLocationUpdate)



Update an appointment location.

### Example

```ts
import {
  Configuration,
  AppointmentLocationApi,
} from '@statflo/statflo-typescript-sdk';
import type { AppointmentLocationUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AppointmentLocationApi(config);

  const body = {
    // string
    id: id_example,
    // AppointmentLocationUpdate (optional)
    appointmentLocationUpdate: ...,
  } satisfies AppointmentLocationUpdateRequest;

  try {
    const data = await api.appointmentLocationUpdate(body);
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
| **appointmentLocationUpdate** | [AppointmentLocationUpdate](AppointmentLocationUpdate.md) |  | [Optional] |

### Return type

[**AppointmentLocation**](AppointmentLocation.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

