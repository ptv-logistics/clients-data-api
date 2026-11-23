# MapInformationApi

All URIs are relative to *https://api.myptv.com/data/v1*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getCombinedTransports**](MapInformationApi.md#getcombinedtransports) | **GET** /combined-transports |  |
| [**getMapInformation**](MapInformationApi.md#getmapinformation) | **GET** /map-information |  |



## getCombinedTransports

> CombinedTransportsResponse getCombinedTransports(position, text, polylineFormat)



Get combined transports from a (click) point on a map or matching a given text input.  A request will be rejected if  * it covers more than 5000 combined transports or * if neither the parameter **position** nor the parameter **text** is specified.

### Example

```ts
import {
  Configuration,
  MapInformationApi,
} from '';
import type { GetCombinedTransportsRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new MapInformationApi(config);

  const body = {
    // CombinedTransportByPosition (optional)
    position: ...,
    // CombinedTransportByText (optional)
    text: ...,
    // PolylineFormat (optional)
    polylineFormat: ...,
  } satisfies GetCombinedTransportsRequest;

  try {
    const data = await api.getCombinedTransports(body);
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
| **position** | [](.md) |  | [Optional] [Defaults to `undefined`] |
| **text** | [](.md) |  | [Optional] [Defaults to `undefined`] |
| **polylineFormat** | `PolylineFormat` |  | [Optional] [Defaults to `undefined`] [Enum: GEO_JSON, GOOGLE_ENCODED_POLYLINE] |

### Return type

[**CombinedTransportsResponse**](CombinedTransportsResponse.md)

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


## getMapInformation

> MapInformationResponse getMapInformation()



Gets information about the map. See [here](./concepts/map-information) for more information.

### Example

```ts
import {
  Configuration,
  MapInformationApi,
} from '';
import type { GetMapInformationRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new MapInformationApi(config);

  try {
    const data = await api.getMapInformation();
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

[**MapInformationResponse**](MapInformationResponse.md)

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

