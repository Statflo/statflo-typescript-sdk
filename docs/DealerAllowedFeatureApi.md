# DealerAllowedFeatureApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**dealerAllowedFeatureCreate**](DealerAllowedFeatureApi.md#dealerallowedfeaturecreate) | **POST** /v4/api/dealer-allowed-feature |  |
| [**dealerAllowedFeatureDelete**](DealerAllowedFeatureApi.md#dealerallowedfeaturedelete) | **DELETE** /v4/api/dealer-allowed-feature/{dealer}/{feature} |  |
| [**dealerAllowedFeatureGet**](DealerAllowedFeatureApi.md#dealerallowedfeatureget) | **GET** /v4/api/dealer-allowed-feature/{dealer}/{feature} |  |



## dealerAllowedFeatureCreate

> DealerAllowedFeature dealerAllowedFeatureCreate(dealerAllowedFeatureCreate)



Create a dealer allowed feature.

### Example

```ts
import {
  Configuration,
  DealerAllowedFeatureApi,
} from '@statflo/statflo-typescript-sdk';
import type { DealerAllowedFeatureCreateRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DealerAllowedFeatureApi(config);

  const body = {
    // DealerAllowedFeatureCreate (optional)
    dealerAllowedFeatureCreate: ...,
  } satisfies DealerAllowedFeatureCreateRequest;

  try {
    const data = await api.dealerAllowedFeatureCreate(body);
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
| **dealerAllowedFeatureCreate** | [DealerAllowedFeatureCreate](DealerAllowedFeatureCreate.md) |  | [Optional] |

### Return type

[**DealerAllowedFeature**](DealerAllowedFeature.md)

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


## dealerAllowedFeatureDelete

> dealerAllowedFeatureDelete(dealer, feature)



Remove a dealer allowed feature.

### Example

```ts
import {
  Configuration,
  DealerAllowedFeatureApi,
} from '@statflo/statflo-typescript-sdk';
import type { DealerAllowedFeatureDeleteRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DealerAllowedFeatureApi(config);

  const body = {
    // string
    dealer: dealer_example,
    // string
    feature: feature_example,
  } satisfies DealerAllowedFeatureDeleteRequest;

  try {
    const data = await api.dealerAllowedFeatureDelete(body);
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
| **dealer** | `string` |  | [Defaults to `undefined`] |
| **feature** | `string` |  | [Defaults to `undefined`] |

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


## dealerAllowedFeatureGet

> DealerAllowedFeature dealerAllowedFeatureGet(dealer, feature)



Retrieve a dealer allowed feature.

### Example

```ts
import {
  Configuration,
  DealerAllowedFeatureApi,
} from '@statflo/statflo-typescript-sdk';
import type { DealerAllowedFeatureGetRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new DealerAllowedFeatureApi(config);

  const body = {
    // string
    dealer: dealer_example,
    // string
    feature: feature_example,
  } satisfies DealerAllowedFeatureGetRequest;

  try {
    const data = await api.dealerAllowedFeatureGet(body);
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
| **dealer** | `string` |  | [Defaults to `undefined`] |
| **feature** | `string` |  | [Defaults to `undefined`] |

### Return type

[**DealerAllowedFeature**](DealerAllowedFeature.md)

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

