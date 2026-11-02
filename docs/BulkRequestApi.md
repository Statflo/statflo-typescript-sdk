# BulkRequestApi

All URIs are relative to *https://app.statflo.com*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**bulkRequest**](BulkRequestApi.md#bulkrequest) | **POST** /v4/api/bulk |  |



## bulkRequest

> Array&lt;object&gt; bulkRequest(bulkSubRequest)



Submit multiple requests in bulk.

### Example

```ts
import {
  Configuration,
  BulkRequestApi,
} from '@statflo/statflo-typescript-sdk';
import type { BulkRequestRequest } from '@statflo/statflo-typescript-sdk';

async function example() {
  console.log("🚀 Testing @statflo/statflo-typescript-sdk SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: Bearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new BulkRequestApi(config);

  const body = {
    // Array<BulkSubRequest>
    bulkSubRequest: ...,
  } satisfies BulkRequestRequest;

  try {
    const data = await api.bulkRequest(body);
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
| **bulkSubRequest** | `Array<BulkSubRequest>` |  | |

### Return type

**Array<object>**

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

