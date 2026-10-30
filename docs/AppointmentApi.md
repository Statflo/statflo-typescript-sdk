# AppointmentApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**appointmentCreate**](AppointmentApi.md#appointmentcreate) | **POST** /v4/api/appointment |  |
| [**appointmentDelete**](AppointmentApi.md#appointmentdelete) | **DELETE** /v4/api/appointment/{id} |  |
| [**appointmentGet**](AppointmentApi.md#appointmentget) | **GET** /v4/api/appointment/{id} |  |
| [**appointmentSearch**](AppointmentApi.md#appointmentsearch) | **GET** /v4/api/appointment |  |
| [**appointmentUpdate**](AppointmentApi.md#appointmentupdate) | **PUT** /v4/api/appointment/{id} |  |



## appointmentCreate

> Appointment appointmentCreate(appointmentCreate)



Create an appointment.

### Example

```ts
import {
  Configuration,
  AppointmentApi,
} from '@statflo/statflo-typescript-sdk';
import type { AppointmentCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AppointmentApi(config);

  const body = {
    // AppointmentCreate (optional)
    appointmentCreate: ...,
  } satisfies AppointmentCreateRequest;

  try {
    const data = await api.appointmentCreate(body);
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
| **appointmentCreate** | [AppointmentCreate](AppointmentCreate.md) |  | [Optional] |

### Return type

[**Appointment**](Appointment.md)

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


## appointmentDelete

> appointmentDelete(id)



Delete an appointment.

### Example

```ts
import {
  Configuration,
  AppointmentApi,
} from '@statflo/statflo-typescript-sdk';
import type { AppointmentDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AppointmentApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies AppointmentDeleteRequest;

  try {
    const data = await api.appointmentDelete(body);
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


## appointmentGet

> Appointment appointmentGet(id)



Retrieve an appointment.

### Example

```ts
import {
  Configuration,
  AppointmentApi,
} from '@statflo/statflo-typescript-sdk';
import type { AppointmentGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AppointmentApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies AppointmentGetRequest;

  try {
    const data = await api.appointmentGet(body);
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

[**Appointment**](Appointment.md)

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


## appointmentSearch

> AppointmentPaginationResponse appointmentSearch(filter, query, page, perPage, sort)



Search appointments.

### Example

```ts
import {
  Configuration,
  AppointmentApi,
} from '@statflo/statflo-typescript-sdk';
import type { AppointmentSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AppointmentApi(config);

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
  } satisfies AppointmentSearchRequest;

  try {
    const data = await api.appointmentSearch(body);
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

[**AppointmentPaginationResponse**](AppointmentPaginationResponse.md)

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


## appointmentUpdate

> Appointment appointmentUpdate(id, appointmentUpdate)



Update an appointment.

### Example

```ts
import {
  Configuration,
  AppointmentApi,
} from '@statflo/statflo-typescript-sdk';
import type { AppointmentUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AppointmentApi(config);

  const body = {
    // string
    id: id_example,
    // AppointmentUpdate (optional)
    appointmentUpdate: ...,
  } satisfies AppointmentUpdateRequest;

  try {
    const data = await api.appointmentUpdate(body);
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
| **appointmentUpdate** | [AppointmentUpdate](AppointmentUpdate.md) |  | [Optional] |

### Return type

[**Appointment**](Appointment.md)

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

