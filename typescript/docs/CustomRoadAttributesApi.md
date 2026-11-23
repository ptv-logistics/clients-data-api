# CustomRoadAttributesApi

All URIs are relative to *https://api.myptv.com/data/v1*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createCustomRoadAttributeScenario**](CustomRoadAttributesApi.md#createcustomroadattributescenario) | **POST** /road-attributes |  |
| [**deleteCustomRoadAttributeScenario**](CustomRoadAttributesApi.md#deletecustomroadattributescenario) | **DELETE** /road-attributes/{scenarioId} |  |
| [**getAllCustomRoadAttributeScenarios**](CustomRoadAttributesApi.md#getallcustomroadattributescenarios) | **GET** /road-attributes |  |
| [**getCustomRoadAttributeScenario**](CustomRoadAttributesApi.md#getcustomroadattributescenario) | **GET** /road-attributes/{scenarioId} |  |
| [**getRoads**](CustomRoadAttributesApi.md#getroads) | **GET** /roads |  |
| [**updateCustomRoadAttributeScenario**](CustomRoadAttributesApi.md#updatecustomroadattributescenario) | **PUT** /road-attributes/{scenarioId} |  |



## createCustomRoadAttributeScenario

> CustomRoadAttributeScenario createCustomRoadAttributeScenario(customRoadAttributeScenario, results, polylineFormat, polylineMapType)



Create a custom road attribute scenario.

### Example

```ts
import {
  Configuration,
  CustomRoadAttributesApi,
} from '';
import type { CreateCustomRoadAttributeScenarioRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new CustomRoadAttributesApi(config);

  const body = {
    // CustomRoadAttributeScenario | The roads to be attributed.
    customRoadAttributeScenario: ...,
    // Array<RoadAttributesResults> | Defines which results will be returned. (optional)
    results: ...,
    // PolylineFormat (optional)
    polylineFormat: ...,
    // PolylineMapType | Defines whether polylines should match the Raster Maps API or the Vector Maps API.  This parameter affects the polylines returned in the response of this request and all subsequent requests referring to this scenario, if polylines are to be returned. Once created or updated, it is not possible to request the polyline for this scenario matching a different map. (optional)
    polylineMapType: ...,
  } satisfies CreateCustomRoadAttributeScenarioRequest;

  try {
    const data = await api.createCustomRoadAttributeScenario(body);
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
| **customRoadAttributeScenario** | [CustomRoadAttributeScenario](CustomRoadAttributeScenario.md) | The roads to be attributed. | |
| **results** | `Array<RoadAttributesResults>` | Defines which results will be returned. | [Optional] |
| **polylineFormat** | `PolylineFormat` |  | [Optional] [Defaults to `undefined`] [Enum: GEO_JSON, GOOGLE_ENCODED_POLYLINE] |
| **polylineMapType** | `PolylineMapType` | Defines whether polylines should match the Raster Maps API or the Vector Maps API.  This parameter affects the polylines returned in the response of this request and all subsequent requests referring to this scenario, if polylines are to be returned. Once created or updated, it is not possible to request the polyline for this scenario matching a different map. | [Optional] [Defaults to `undefined`] [Enum: RASTER, VECTOR] |

### Return type

[**CustomRoadAttributeScenario**](CustomRoadAttributeScenario.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Response on success. |  -  |
| **0** | Response on failure. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteCustomRoadAttributeScenario

> deleteCustomRoadAttributeScenario(scenarioId)



Delete a custom road attribute scenario.

### Example

```ts
import {
  Configuration,
  CustomRoadAttributesApi,
} from '';
import type { DeleteCustomRoadAttributeScenarioRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new CustomRoadAttributesApi(config);

  const body = {
    // string | The ID of the custom road attribute scenario.
    scenarioId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteCustomRoadAttributeScenarioRequest;

  try {
    const data = await api.deleteCustomRoadAttributeScenario(body);
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
| **scenarioId** | `string` | The ID of the custom road attribute scenario. | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Response on success. |  -  |
| **0** | Response on failure. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getAllCustomRoadAttributeScenarios

> CustomRoadAttributeScenarioList getAllCustomRoadAttributeScenarios(results, polylineFormat)



Get a list of all custom road attribute scenarios of the current user.

### Example

```ts
import {
  Configuration,
  CustomRoadAttributesApi,
} from '';
import type { GetAllCustomRoadAttributeScenariosRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new CustomRoadAttributesApi(config);

  const body = {
    // Array<RoadAttributesResults> | Defines which results will be returned. (optional)
    results: ...,
    // PolylineFormat (optional)
    polylineFormat: ...,
  } satisfies GetAllCustomRoadAttributeScenariosRequest;

  try {
    const data = await api.getAllCustomRoadAttributeScenarios(body);
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
| **results** | `Array<RoadAttributesResults>` | Defines which results will be returned. | [Optional] |
| **polylineFormat** | `PolylineFormat` |  | [Optional] [Defaults to `undefined`] [Enum: GEO_JSON, GOOGLE_ENCODED_POLYLINE] |

### Return type

[**CustomRoadAttributeScenarioList**](CustomRoadAttributeScenarioList.md)

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


## getCustomRoadAttributeScenario

> CustomRoadAttributeScenario getCustomRoadAttributeScenario(scenarioId, results, polylineFormat)



Get a custom road attribute scenario by its ID.

### Example

```ts
import {
  Configuration,
  CustomRoadAttributesApi,
} from '';
import type { GetCustomRoadAttributeScenarioRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new CustomRoadAttributesApi(config);

  const body = {
    // string | The ID of the custom road attribute scenario.
    scenarioId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // Array<RoadAttributesResults> | Defines which results will be returned. (optional)
    results: ...,
    // PolylineFormat (optional)
    polylineFormat: ...,
  } satisfies GetCustomRoadAttributeScenarioRequest;

  try {
    const data = await api.getCustomRoadAttributeScenario(body);
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
| **scenarioId** | `string` | The ID of the custom road attribute scenario. | [Defaults to `undefined`] |
| **results** | `Array<RoadAttributesResults>` | Defines which results will be returned. | [Optional] |
| **polylineFormat** | `PolylineFormat` |  | [Optional] [Defaults to `undefined`] [Enum: GEO_JSON, GOOGLE_ENCODED_POLYLINE] |

### Return type

[**CustomRoadAttributeScenario**](CustomRoadAttributeScenario.md)

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


## getRoads

> RoadsResponse getRoads(points, polylineFormat, polylineMapType)



Get roads from (click) points on a map.

### Example

```ts
import {
  Configuration,
  CustomRoadAttributesApi,
} from '';
import type { GetRoadsRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new CustomRoadAttributesApi(config);

  const body = {
    // string | A point, a polyline or a polygon to select roads. Combined transports will not be selected.  * For a single point the road(s) closest to this point will be returned.  Usually, a single road will be returned, but if there are multiple roads at the same distance from the point, all of them will be returned. This is most likely to happen on road crossings. * Several points where the first and last point are different will be considered a polyline and  all roads intersected by this polyline will be returned. * If the polyline is closed, i.e. the first and the last point are the same, the polyline defines  a polygon and all roads whose complete polyline is within the polygon will be returned. A polygon must be  valid according to [OGC](https://www.ogc.org/standard/sfa/). Holes within polygons are not supported.  Format: `<point1_lat>,<point1_lon>,...,<pointN_lat>,<pointN_lon>`.  A request will be rejected if it * does not contain an even number of coordinates, * contains a closed polyline defining an invalid polygon according to OGC, * contains invalid coordinates or * covers more than 5000 roads.
    points: 49.0133618,8.4277972,
    // PolylineFormat (optional)
    polylineFormat: ...,
    // PolylineMapType | Defines whether polylines should match the Raster Maps API or the Vector Maps API.  The polylines are used for the selection, hence the selected roads can differ when using different values. (optional)
    polylineMapType: ...,
  } satisfies GetRoadsRequest;

  try {
    const data = await api.getRoads(body);
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
| **points** | `string` | A point, a polyline or a polygon to select roads. Combined transports will not be selected.  * For a single point the road(s) closest to this point will be returned.  Usually, a single road will be returned, but if there are multiple roads at the same distance from the point, all of them will be returned. This is most likely to happen on road crossings. * Several points where the first and last point are different will be considered a polyline and  all roads intersected by this polyline will be returned. * If the polyline is closed, i.e. the first and the last point are the same, the polyline defines  a polygon and all roads whose complete polyline is within the polygon will be returned. A polygon must be  valid according to [OGC](https://www.ogc.org/standard/sfa/). Holes within polygons are not supported.  Format: &#x60;&lt;point1_lat&gt;,&lt;point1_lon&gt;,...,&lt;pointN_lat&gt;,&lt;pointN_lon&gt;&#x60;.  A request will be rejected if it * does not contain an even number of coordinates, * contains a closed polyline defining an invalid polygon according to OGC, * contains invalid coordinates or * covers more than 5000 roads. | [Defaults to `undefined`] |
| **polylineFormat** | `PolylineFormat` |  | [Optional] [Defaults to `undefined`] [Enum: GEO_JSON, GOOGLE_ENCODED_POLYLINE] |
| **polylineMapType** | `PolylineMapType` | Defines whether polylines should match the Raster Maps API or the Vector Maps API.  The polylines are used for the selection, hence the selected roads can differ when using different values. | [Optional] [Defaults to `undefined`] [Enum: RASTER, VECTOR] |

### Return type

[**RoadsResponse**](RoadsResponse.md)

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


## updateCustomRoadAttributeScenario

> CustomRoadAttributeScenario updateCustomRoadAttributeScenario(scenarioId, customRoadAttributeScenario, results, polylineFormat, polylineMapType)



Perform a full update of an existing custom road attribute scenario.

### Example

```ts
import {
  Configuration,
  CustomRoadAttributesApi,
} from '';
import type { UpdateCustomRoadAttributeScenarioRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // To configure API key authorization: apiKeyAuth
    apiKey: "YOUR API KEY",
  });
  const api = new CustomRoadAttributesApi(config);

  const body = {
    // string | The ID of the custom road attribute scenario.
    scenarioId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
    // CustomRoadAttributeScenario | The custom road attribute scenario to be updated.
    customRoadAttributeScenario: ...,
    // Array<RoadAttributesResults> | Defines which results will be returned. (optional)
    results: ...,
    // PolylineFormat (optional)
    polylineFormat: ...,
    // PolylineMapType | Defines whether polylines should match the Raster Maps API or the Vector Maps API.  This parameter affects the polylines returned in the response of this request and all subsequent requests referring to this scenario, if polylines are to be returned. Once created or updated, it is not possible to request the polyline for this scenario matching a different map. (optional)
    polylineMapType: ...,
  } satisfies UpdateCustomRoadAttributeScenarioRequest;

  try {
    const data = await api.updateCustomRoadAttributeScenario(body);
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
| **scenarioId** | `string` | The ID of the custom road attribute scenario. | [Defaults to `undefined`] |
| **customRoadAttributeScenario** | [CustomRoadAttributeScenario](CustomRoadAttributeScenario.md) | The custom road attribute scenario to be updated. | |
| **results** | `Array<RoadAttributesResults>` | Defines which results will be returned. | [Optional] |
| **polylineFormat** | `PolylineFormat` |  | [Optional] [Defaults to `undefined`] [Enum: GEO_JSON, GOOGLE_ENCODED_POLYLINE] |
| **polylineMapType** | `PolylineMapType` | Defines whether polylines should match the Raster Maps API or the Vector Maps API.  This parameter affects the polylines returned in the response of this request and all subsequent requests referring to this scenario, if polylines are to be returned. Once created or updated, it is not possible to request the polyline for this scenario matching a different map. | [Optional] [Defaults to `undefined`] [Enum: RASTER, VECTOR] |

### Return type

[**CustomRoadAttributeScenario**](CustomRoadAttributeScenario.md)

### Authorization

[apiKeyAuth](../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Response on success. |  -  |
| **0** | Response on failure. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

