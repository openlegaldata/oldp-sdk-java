# CaseMarkersApi

All URIs are relative to *https://de.openlegaldata.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**caseMarkersCreate**](CaseMarkersApi.md#caseMarkersCreate) | **POST** /case_markers/ | 
[**caseMarkersDelete**](CaseMarkersApi.md#caseMarkersDelete) | **DELETE** /case_markers/{id}/ | 
[**caseMarkersList**](CaseMarkersApi.md#caseMarkersList) | **GET** /case_markers/ | 
[**caseMarkersPartialUpdate**](CaseMarkersApi.md#caseMarkersPartialUpdate) | **PATCH** /case_markers/{id}/ | 
[**caseMarkersRead**](CaseMarkersApi.md#caseMarkersRead) | **GET** /case_markers/{id}/ | 
[**caseMarkersUpdate**](CaseMarkersApi.md#caseMarkersUpdate) | **PUT** /case_markers/{id}/ | 


<a name="caseMarkersCreate"></a>
# **caseMarkersCreate**
> CaseMarker caseMarkersCreate(data)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CaseMarkersApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CaseMarkersApi apiInstance = new CaseMarkersApi();
CaseMarker data = new CaseMarker(); // CaseMarker | 
try {
    CaseMarker result = apiInstance.caseMarkersCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CaseMarkersApi#caseMarkersCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**CaseMarker**](CaseMarker.md)|  |

### Return type

[**CaseMarker**](CaseMarker.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="caseMarkersDelete"></a>
# **caseMarkersDelete**
> caseMarkersDelete(id)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CaseMarkersApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CaseMarkersApi apiInstance = new CaseMarkersApi();
Integer id = 56; // Integer | A unique integer value identifying this case marker.
try {
    apiInstance.caseMarkersDelete(id);
} catch (ApiException e) {
    System.err.println("Exception when calling CaseMarkersApi#caseMarkersDelete");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this case marker. |

### Return type

null (empty response body)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="caseMarkersList"></a>
# **caseMarkersList**
> InlineResponse2002 caseMarkersList(belongsTo, label, limit, offset)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CaseMarkersApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CaseMarkersApi apiInstance = new CaseMarkersApi();
BigDecimal belongsTo = new BigDecimal(); // BigDecimal | 
BigDecimal label = new BigDecimal(); // BigDecimal | 
Integer limit = 56; // Integer | Number of results to return per page.
Integer offset = 56; // Integer | The initial index from which to return the results.
try {
    InlineResponse2002 result = apiInstance.caseMarkersList(belongsTo, label, limit, offset);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CaseMarkersApi#caseMarkersList");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **belongsTo** | **BigDecimal**|  | [optional]
 **label** | **BigDecimal**|  | [optional]
 **limit** | **Integer**| Number of results to return per page. | [optional]
 **offset** | **Integer**| The initial index from which to return the results. | [optional]

### Return type

[**InlineResponse2002**](InlineResponse2002.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="caseMarkersPartialUpdate"></a>
# **caseMarkersPartialUpdate**
> CaseMarker caseMarkersPartialUpdate(id, data)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CaseMarkersApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CaseMarkersApi apiInstance = new CaseMarkersApi();
Integer id = 56; // Integer | A unique integer value identifying this case marker.
CaseMarker data = new CaseMarker(); // CaseMarker | 
try {
    CaseMarker result = apiInstance.caseMarkersPartialUpdate(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CaseMarkersApi#caseMarkersPartialUpdate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this case marker. |
 **data** | [**CaseMarker**](CaseMarker.md)|  |

### Return type

[**CaseMarker**](CaseMarker.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="caseMarkersRead"></a>
# **caseMarkersRead**
> CaseMarker caseMarkersRead(id)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CaseMarkersApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CaseMarkersApi apiInstance = new CaseMarkersApi();
Integer id = 56; // Integer | A unique integer value identifying this case marker.
try {
    CaseMarker result = apiInstance.caseMarkersRead(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CaseMarkersApi#caseMarkersRead");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this case marker. |

### Return type

[**CaseMarker**](CaseMarker.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="caseMarkersUpdate"></a>
# **caseMarkersUpdate**
> CaseMarker caseMarkersUpdate(id, data)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CaseMarkersApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CaseMarkersApi apiInstance = new CaseMarkersApi();
Integer id = 56; // Integer | A unique integer value identifying this case marker.
CaseMarker data = new CaseMarker(); // CaseMarker | 
try {
    CaseMarker result = apiInstance.caseMarkersUpdate(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CaseMarkersApi#caseMarkersUpdate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this case marker. |
 **data** | [**CaseMarker**](CaseMarker.md)|  |

### Return type

[**CaseMarker**](CaseMarker.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

