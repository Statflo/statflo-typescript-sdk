# UserTeamApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**userTeamCreate**](UserTeamApi.md#userteamcreate) | **POST** /v4/api/user-team |  |
| [**userTeamDelete**](UserTeamApi.md#userteamdelete) | **DELETE** /v4/api/user-team/{team}/{user} |  |



## userTeamCreate

> UserTeam userTeamCreate(userTeamCreate)



Assign user to a team.

### Example

```ts
import {
  Configuration,
  UserTeamApi,
} from '@statflo/statflo-typescript-sdk';
import type { UserTeamCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UserTeamApi(config);

  const body = {
    // UserTeamCreate (optional)
    userTeamCreate: ...,
  } satisfies UserTeamCreateRequest;

  try {
    const data = await api.userTeamCreate(body);
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
| **userTeamCreate** | [UserTeamCreate](UserTeamCreate.md) |  | [Optional] |

### Return type

[**UserTeam**](UserTeam.md)

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


## userTeamDelete

> userTeamDelete(team, user)



Remove user from team.

### Example

```ts
import {
  Configuration,
  UserTeamApi,
} from '@statflo/statflo-typescript-sdk';
import type { UserTeamDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new UserTeamApi(config);

  const body = {
    // string
    team: team_example,
    // string
    user: user_example,
  } satisfies UserTeamDeleteRequest;

  try {
    const data = await api.userTeamDelete(body);
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
| **team** | `string` |  | [Defaults to `undefined`] |
| **user** | `string` |  | [Defaults to `undefined`] |

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

