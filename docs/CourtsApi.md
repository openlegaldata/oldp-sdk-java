# CourtsApi

All URIs are relative to *https://de.openlegaldata.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**courtsList**](CourtsApi.md#courtsList) | **GET** /courts/ | 
[**courtsRead**](CourtsApi.md#courtsRead) | **GET** /courts/{id}/ | 


<a name="courtsList"></a>
# **courtsList**
> InlineResponse2007 courtsList(courtType, slug, code, stateId, cityId, limit, offset)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CourtsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CourtsApi apiInstance = new CourtsApi();
String courtType = "courtType_example"; // String | 
String slug = "slug_example"; // String | 
String code = "code_example"; // String | 
String stateId = "stateId_example"; // String | 
String cityId = "cityId_example"; // String | 
Integer limit = 56; // Integer | Number of results to return per page.
Integer offset = 56; // Integer | The initial index from which to return the results.
try {
    InlineResponse2007 result = apiInstance.courtsList(courtType, slug, code, stateId, cityId, limit, offset);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CourtsApi#courtsList");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **courtType** | **String**|  | [optional]
 **slug** | **String**|  | [optional]
 **code** | **String**|  | [optional]
 **stateId** | **String**|  | [optional]
 **cityId** | **String**|  | [optional]
 **limit** | **Integer**| Number of results to return per page. | [optional]
 **offset** | **Integer**| The initial index from which to return the results. | [optional]

### Return type

[**InlineResponse2007**](InlineResponse2007.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="courtsRead"></a>
# **courtsRead**
> Court courtsRead(id)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CourtsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CourtsApi apiInstance = new CourtsApi();
Integer id = 56; // Integer | A unique integer value identifying this court.
try {
    Court result = apiInstance.courtsRead(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CourtsApi#courtsRead");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this court. |

### Return type

[**Court**](Court.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

