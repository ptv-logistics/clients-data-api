# APIChangesApi

All URIs are relative to *https://api.myptv.com/data/v1*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getApiChanges**](APIChangesApi.md#getapichanges) | **GET** /api-changes |  |



## getApiChanges

> ApiChanges getApiChanges()



Get all API changes for PTV Developer.

### Example

```ts
import {
  Configuration,
  APIChangesApi,
} from '';
import type { GetApiChangesRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new APIChangesApi(config);

  try {
    const data = await api.getApiChanges();
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

[**ApiChanges**](ApiChanges.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Response on success. |  -  |
| **0** | Response on failure. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

