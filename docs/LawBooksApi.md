# LawBooksApi

All URIs are relative to *https://de.openlegaldata.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**lawBooksCreate**](LawBooksApi.md#lawBooksCreate) | **POST** /law_books/ | 
[**lawBooksDelete**](LawBooksApi.md#lawBooksDelete) | **DELETE** /law_books/{id}/ | 
[**lawBooksList**](LawBooksApi.md#lawBooksList) | **GET** /law_books/ | 
[**lawBooksPartialUpdate**](LawBooksApi.md#lawBooksPartialUpdate) | **PATCH** /law_books/{id}/ | 
[**lawBooksRead**](LawBooksApi.md#lawBooksRead) | **GET** /law_books/{id}/ | 
[**lawBooksUpdate**](LawBooksApi.md#lawBooksUpdate) | **PUT** /law_books/{id}/ | 


<a name="lawBooksCreate"></a>
# **lawBooksCreate**
> LawBook lawBooksCreate(data)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.LawBooksApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

LawBooksApi apiInstance = new LawBooksApi();
LawBook data = new LawBook(); // LawBook | 
try {
    LawBook result = apiInstance.lawBooksCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LawBooksApi#lawBooksCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**LawBook**](LawBook.md)|  |

### Return type

[**LawBook**](LawBook.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="lawBooksDelete"></a>
# **lawBooksDelete**
> lawBooksDelete(id)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.LawBooksApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

LawBooksApi apiInstance = new LawBooksApi();
Integer id = 56; // Integer | A unique integer value identifying this law book.
try {
    apiInstance.lawBooksDelete(id);
} catch (ApiException e) {
    System.err.println("Exception when calling LawBooksApi#lawBooksDelete");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this law book. |

### Return type

null (empty response body)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="lawBooksList"></a>
# **lawBooksList**
> InlineResponse2008 lawBooksList(slug, code, latest, revisionDate, limit, offset)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.LawBooksApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

LawBooksApi apiInstance = new LawBooksApi();
String slug = "slug_example"; // String | 
String code = "code_example"; // String | 
String latest = "latest_example"; // String | 
String revisionDate = "revisionDate_example"; // String | 
Integer limit = 56; // Integer | Number of results to return per page.
Integer offset = 56; // Integer | The initial index from which to return the results.
try {
    InlineResponse2008 result = apiInstance.lawBooksList(slug, code, latest, revisionDate, limit, offset);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LawBooksApi#lawBooksList");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **String**|  | [optional]
 **code** | **String**|  | [optional]
 **latest** | **String**|  | [optional]
 **revisionDate** | **String**|  | [optional]
 **limit** | **Integer**| Number of results to return per page. | [optional]
 **offset** | **Integer**| The initial index from which to return the results. | [optional]

### Return type

[**InlineResponse2008**](InlineResponse2008.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="lawBooksPartialUpdate"></a>
# **lawBooksPartialUpdate**
> LawBook lawBooksPartialUpdate(id, data)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.LawBooksApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

LawBooksApi apiInstance = new LawBooksApi();
Integer id = 56; // Integer | A unique integer value identifying this law book.
LawBook data = new LawBook(); // LawBook | 
try {
    LawBook result = apiInstance.lawBooksPartialUpdate(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LawBooksApi#lawBooksPartialUpdate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this law book. |
 **data** | [**LawBook**](LawBook.md)|  |

### Return type

[**LawBook**](LawBook.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="lawBooksRead"></a>
# **lawBooksRead**
> LawBook lawBooksRead(id)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.LawBooksApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

LawBooksApi apiInstance = new LawBooksApi();
Integer id = 56; // Integer | A unique integer value identifying this law book.
try {
    LawBook result = apiInstance.lawBooksRead(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LawBooksApi#lawBooksRead");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this law book. |

### Return type

[**LawBook**](LawBook.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="lawBooksUpdate"></a>
# **lawBooksUpdate**
> LawBook lawBooksUpdate(id, data)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.LawBooksApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

LawBooksApi apiInstance = new LawBooksApi();
Integer id = 56; // Integer | A unique integer value identifying this law book.
LawBook data = new LawBook(); // LawBook | 
try {
    LawBook result = apiInstance.lawBooksUpdate(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LawBooksApi#lawBooksUpdate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this law book. |
 **data** | [**LawBook**](LawBook.md)|  |

### Return type

[**LawBook**](LawBook.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

