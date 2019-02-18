# LawsApi

All URIs are relative to *https://de.openlegaldata.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**lawsCreate**](LawsApi.md#lawsCreate) | **POST** /laws/ | 
[**lawsDelete**](LawsApi.md#lawsDelete) | **DELETE** /laws/{id}/ | 
[**lawsList**](LawsApi.md#lawsList) | **GET** /laws/ | 
[**lawsPartialUpdate**](LawsApi.md#lawsPartialUpdate) | **PATCH** /laws/{id}/ | 
[**lawsRead**](LawsApi.md#lawsRead) | **GET** /laws/{id}/ | 
[**lawsSearchList**](LawsApi.md#lawsSearchList) | **GET** /laws/search/ | 
[**lawsUpdate**](LawsApi.md#lawsUpdate) | **PUT** /laws/{id}/ | 


<a name="lawsCreate"></a>
# **lawsCreate**
> Law lawsCreate(data)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.LawsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

LawsApi apiInstance = new LawsApi();
Law data = new Law(); // Law | 
try {
    Law result = apiInstance.lawsCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LawsApi#lawsCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Law**](Law.md)|  |

### Return type

[**Law**](Law.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="lawsDelete"></a>
# **lawsDelete**
> lawsDelete(id)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.LawsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

LawsApi apiInstance = new LawsApi();
Integer id = 56; // Integer | A unique integer value identifying this law.
try {
    apiInstance.lawsDelete(id);
} catch (ApiException e) {
    System.err.println("Exception when calling LawsApi#lawsDelete");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this law. |

### Return type

null (empty response body)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="lawsList"></a>
# **lawsList**
> InlineResponse2009 lawsList(bookId, bookLatest, bookRevisionDate, limit, offset)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.LawsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

LawsApi apiInstance = new LawsApi();
String bookId = "bookId_example"; // String | 
String bookLatest = "bookLatest_example"; // String | 
String bookRevisionDate = "bookRevisionDate_example"; // String | 
Integer limit = 56; // Integer | Number of results to return per page.
Integer offset = 56; // Integer | The initial index from which to return the results.
try {
    InlineResponse2009 result = apiInstance.lawsList(bookId, bookLatest, bookRevisionDate, limit, offset);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LawsApi#lawsList");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bookId** | **String**|  | [optional]
 **bookLatest** | **String**|  | [optional]
 **bookRevisionDate** | **String**|  | [optional]
 **limit** | **Integer**| Number of results to return per page. | [optional]
 **offset** | **Integer**| The initial index from which to return the results. | [optional]

### Return type

[**InlineResponse2009**](InlineResponse2009.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="lawsPartialUpdate"></a>
# **lawsPartialUpdate**
> Law lawsPartialUpdate(id, data)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.LawsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

LawsApi apiInstance = new LawsApi();
Integer id = 56; // Integer | A unique integer value identifying this law.
Law data = new Law(); // Law | 
try {
    Law result = apiInstance.lawsPartialUpdate(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LawsApi#lawsPartialUpdate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this law. |
 **data** | [**Law**](Law.md)|  |

### Return type

[**Law**](Law.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="lawsRead"></a>
# **lawsRead**
> Law lawsRead(id)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.LawsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

LawsApi apiInstance = new LawsApi();
Integer id = 56; // Integer | A unique integer value identifying this law.
try {
    Law result = apiInstance.lawsRead(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LawsApi#lawsRead");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this law. |

### Return type

[**Law**](Law.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="lawsSearchList"></a>
# **lawsSearchList**
> InlineResponse20010 lawsSearchList(text, facetModelName, bookCode, page, pageSize)



Search view

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.LawsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

LawsApi apiInstance = new LawsApi();
String text = "text_example"; // String | Search query on text content (Lucence syntax support).
String facetModelName = "facetModelName_example"; // String | facet_model_name
String bookCode = "bookCode_example"; // String | book_code
Integer page = 56; // Integer | A page number within the paginated result set.
Integer pageSize = 56; // Integer | Number of results to return per page.
try {
    InlineResponse20010 result = apiInstance.lawsSearchList(text, facetModelName, bookCode, page, pageSize);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LawsApi#lawsSearchList");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **text** | **String**| Search query on text content (Lucence syntax support). |
 **facetModelName** | **String**| facet_model_name | [optional]
 **bookCode** | **String**| book_code | [optional]
 **page** | **Integer**| A page number within the paginated result set. | [optional]
 **pageSize** | **Integer**| Number of results to return per page. | [optional]

### Return type

[**InlineResponse20010**](InlineResponse20010.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="lawsUpdate"></a>
# **lawsUpdate**
> Law lawsUpdate(id, data)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.LawsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

LawsApi apiInstance = new LawsApi();
Integer id = 56; // Integer | A unique integer value identifying this law.
Law data = new Law(); // Law | 
try {
    Law result = apiInstance.lawsUpdate(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LawsApi#lawsUpdate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this law. |
 **data** | [**Law**](Law.md)|  |

### Return type

[**Law**](Law.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

