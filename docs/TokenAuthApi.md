# TokenAuthApi

All URIs are relative to *https://de.openlegaldata.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**tokenAuthCreate**](TokenAuthApi.md#tokenAuthCreate) | **POST** /token-auth/ | 


<a name="tokenAuthCreate"></a>
# **tokenAuthCreate**
> tokenAuthCreate()





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.TokenAuthApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

TokenAuthApi apiInstance = new TokenAuthApi();
try {
    apiInstance.tokenAuthCreate();
} catch (ApiException e) {
    System.err.println("Exception when calling TokenAuthApi#tokenAuthCreate");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

