# VehicleModelsApi

All URIs are relative to *https://api.myptv.com/data/v1*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getVehicleModels**](VehicleModelsApi.md#getvehiclemodels) | **GET** /vehicle-models |  |



## getVehicleModels

> VehicleModels getVehicleModels(identification, vehicleTypes)



A list of **VehicleModel** objects. Only vehicle models matching all filters are returned. In case that no vehicle model is found an empty list is returned. In case no filters are applied, all available vehicle models are returned.  This method is in a preview state, the API is stable, feature changes could be introduced in future.

### Example

```ts
import {
  Configuration,
  VehicleModelsApi,
} from '';
import type { GetVehicleModelsRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new VehicleModelsApi(config);

  const body = {
    // string | String which must be contained in the vehicle model or the vehicle variant. See **commercial** in the response. (optional)
    identification: identification_example,
    // Array<string> | A comma-separated list of vehicle types. See **vehicleType** in the response. The following vehicle types are supported.  Tractor-like vehicle types: * `TRUCK` - Truck. Total permitted weight > 7.5t. * `LCV` - Light Commercial Vehicle. Total permitted weight < 7.5t. * `SCV` - Small Commercial Vehicle. Total permitted weight < 3.5t.  Trailer-like vehicle types: * `TRAILER` - Trailer * `SEMI_TRAILER` - Semi-trailer * `BODY` - Body  This list can be extended at any time. (optional)
    vehicleTypes: ["TRUCK","LCV","SCV"],
  } satisfies GetVehicleModelsRequest;

  try {
    const data = await api.getVehicleModels(body);
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
| **identification** | `string` | String which must be contained in the vehicle model or the vehicle variant. See **commercial** in the response. | [Optional] [Defaults to `undefined`] |
| **vehicleTypes** | `Array<string>` | A comma-separated list of vehicle types. See **vehicleType** in the response. The following vehicle types are supported.  Tractor-like vehicle types: * &#x60;TRUCK&#x60; - Truck. Total permitted weight &gt; 7.5t. * &#x60;LCV&#x60; - Light Commercial Vehicle. Total permitted weight &lt; 7.5t. * &#x60;SCV&#x60; - Small Commercial Vehicle. Total permitted weight &lt; 3.5t.  Trailer-like vehicle types: * &#x60;TRAILER&#x60; - Trailer * &#x60;SEMI_TRAILER&#x60; - Semi-trailer * &#x60;BODY&#x60; - Body  This list can be extended at any time. | [Optional] |

### Return type

[**VehicleModels**](VehicleModels.md)

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

