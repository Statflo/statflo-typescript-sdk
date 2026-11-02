# AuthenticationApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**authMe**](AuthenticationApi.md#authme) | **GET** /v4/api/auth/me |  |
| [**login**](AuthenticationApi.md#loginoperation) | **POST** /v4/api/auth/login |  |
| [**logout**](AuthenticationApi.md#logout) | **GET** /v4/api/auth/logout |  |
| [**switchDealer**](AuthenticationApi.md#switchdealer) | **GET** /v4/api/auth/switch |  |
| [**switchDealerPost**](AuthenticationApi.md#switchdealerpostoperation) | **POST** /v4/api/auth/switch |  |



## authMe

> User authMe()



Get currently logged in user.

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@statflo/statflo-typescript-sdk';
import type { AuthMeRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  try {
    const data = await api.authMe();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**User**](User.md)

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


## login

> Login200Response login(loginRequest)



Log in.

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@statflo/statflo-typescript-sdk';
import type { LoginOperationRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // LoginRequest (optional)
    loginRequest: ...,
  } satisfies LoginOperationRequest;

  try {
    const data = await api.login(body);
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
| **loginRequest** | [LoginRequest](LoginRequest.md) |  | [Optional] |

### Return type

[**Login200Response**](Login200Response.md)

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


## logout

> logout()



Log out.

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@statflo/statflo-typescript-sdk';
import type { LogoutRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  try {
    const data = await api.logout();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

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
| **200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## switchDealer

> switchDealer(dealerId, roleId)



Switch active dealer.

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@statflo/statflo-typescript-sdk';
import type { SwitchDealerRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // number (optional)
    dealerId: 56,
    // number (optional)
    roleId: 56,
  } satisfies SwitchDealerRequest;

  try {
    const data = await api.switchDealer(body);
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
| **dealerId** | `number` |  | [Optional] [Defaults to `undefined`] |
| **roleId** | `number` |  | [Optional] [Defaults to `undefined`] |

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
| **302** | Success |  -  |
| **400** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## switchDealerPost

> User switchDealerPost(switchDealerPostRequest)



Switch active dealer.

### Example

```ts
import {
  Configuration,
  AuthenticationApi,
} from '@statflo/statflo-typescript-sdk';
import type { SwitchDealerPostOperationRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new AuthenticationApi(config);

  const body = {
    // SwitchDealerPostRequest (optional)
    switchDealerPostRequest: ...,
  } satisfies SwitchDealerPostOperationRequest;

  try {
    const data = await api.switchDealerPost(body);
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
| **switchDealerPostRequest** | [SwitchDealerPostRequest](SwitchDealerPostRequest.md) |  | [Optional] |

### Return type

[**User**](User.md)

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

