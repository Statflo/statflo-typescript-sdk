# CampaignMemberApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**campaignMemberCreate**](CampaignMemberApi.md#campaignmembercreate) | **POST** /v4/api/campaign-member |  |
| [**campaignMemberDelete**](CampaignMemberApi.md#campaignmemberdelete) | **DELETE** /v4/api/campaign-member/{id} |  |
| [**campaignMemberGet**](CampaignMemberApi.md#campaignmemberget) | **GET** /v4/api/campaign-member/{id} |  |
| [**campaignMemberSearch**](CampaignMemberApi.md#campaignmembersearch) | **GET** /v4/api/campaign-member |  |
| [**campaignMemberUpdate**](CampaignMemberApi.md#campaignmemberupdate) | **PUT** /v4/api/campaign-member/{id} |  |



## campaignMemberCreate

> CampaignMember campaignMemberCreate(campaignMemberCreate)



Create a campaign member.

### Example

```ts
import {
  Configuration,
  CampaignMemberApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignMemberCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignMemberApi(config);

  const body = {
    // CampaignMemberCreate (optional)
    campaignMemberCreate: ...,
  } satisfies CampaignMemberCreateRequest;

  try {
    const data = await api.campaignMemberCreate(body);
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
| **campaignMemberCreate** | [CampaignMemberCreate](CampaignMemberCreate.md) |  | [Optional] |

### Return type

[**CampaignMember**](CampaignMember.md)

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


## campaignMemberDelete

> campaignMemberDelete(id)



Remove a campaign member.

### Example

```ts
import {
  Configuration,
  CampaignMemberApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignMemberDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignMemberApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies CampaignMemberDeleteRequest;

  try {
    const data = await api.campaignMemberDelete(body);
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


## campaignMemberGet

> CampaignMember campaignMemberGet(id)



Retrieve a campaign member.

### Example

```ts
import {
  Configuration,
  CampaignMemberApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignMemberGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignMemberApi(config);

  const body = {
    // string
    id: id_example,
  } satisfies CampaignMemberGetRequest;

  try {
    const data = await api.campaignMemberGet(body);
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

[**CampaignMember**](CampaignMember.md)

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


## campaignMemberSearch

> CampaignMemberPaginationResponse campaignMemberSearch(filter, query, page, perPage, sort)



Search campaign member.

### Example

```ts
import {
  Configuration,
  CampaignMemberApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignMemberSearchRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignMemberApi(config);

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
  } satisfies CampaignMemberSearchRequest;

  try {
    const data = await api.campaignMemberSearch(body);
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

[**CampaignMemberPaginationResponse**](CampaignMemberPaginationResponse.md)

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


## campaignMemberUpdate

> CampaignMember campaignMemberUpdate(id, campaignMemberUpdate)



Update a campaign member.

### Example

```ts
import {
  Configuration,
  CampaignMemberApi,
} from '@statflo/statflo-typescript-sdk';
import type { CampaignMemberUpdateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new CampaignMemberApi(config);

  const body = {
    // string
    id: id_example,
    // CampaignMemberUpdate (optional)
    campaignMemberUpdate: ...,
  } satisfies CampaignMemberUpdateRequest;

  try {
    const data = await api.campaignMemberUpdate(body);
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
| **campaignMemberUpdate** | [CampaignMemberUpdate](CampaignMemberUpdate.md) |  | [Optional] |

### Return type

[**CampaignMember**](CampaignMember.md)

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

