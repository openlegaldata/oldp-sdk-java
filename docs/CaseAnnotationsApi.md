# CaseAnnotationsApi

All URIs are relative to *https://de.openlegaldata.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**caseAnnotationsCreate**](CaseAnnotationsApi.md#caseAnnotationsCreate) | **POST** /case_annotations/ | 
[**caseAnnotationsDelete**](CaseAnnotationsApi.md#caseAnnotationsDelete) | **DELETE** /case_annotations/{id}/ | 
[**caseAnnotationsList**](CaseAnnotationsApi.md#caseAnnotationsList) | **GET** /case_annotations/ | 
[**caseAnnotationsPartialUpdate**](CaseAnnotationsApi.md#caseAnnotationsPartialUpdate) | **PATCH** /case_annotations/{id}/ | 
[**caseAnnotationsRead**](CaseAnnotationsApi.md#caseAnnotationsRead) | **GET** /case_annotations/{id}/ | 
[**caseAnnotationsUpdate**](CaseAnnotationsApi.md#caseAnnotationsUpdate) | **PUT** /case_annotations/{id}/ | 


<a name="caseAnnotationsCreate"></a>
# **caseAnnotationsCreate**
> CaseAnnotation caseAnnotationsCreate(data)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CaseAnnotationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CaseAnnotationsApi apiInstance = new CaseAnnotationsApi();
CaseAnnotation data = new CaseAnnotation(); // CaseAnnotation | 
try {
    CaseAnnotation result = apiInstance.caseAnnotationsCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CaseAnnotationsApi#caseAnnotationsCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**CaseAnnotation**](CaseAnnotation.md)|  |

### Return type

[**CaseAnnotation**](CaseAnnotation.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="caseAnnotationsDelete"></a>
# **caseAnnotationsDelete**
> caseAnnotationsDelete(id)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CaseAnnotationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CaseAnnotationsApi apiInstance = new CaseAnnotationsApi();
Integer id = 56; // Integer | A unique integer value identifying this case annotation.
try {
    apiInstance.caseAnnotationsDelete(id);
} catch (ApiException e) {
    System.err.println("Exception when calling CaseAnnotationsApi#caseAnnotationsDelete");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this case annotation. |

### Return type

null (empty response body)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="caseAnnotationsList"></a>
# **caseAnnotationsList**
> InlineResponse2001 caseAnnotationsList(belongsTo, label, limit, offset)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CaseAnnotationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CaseAnnotationsApi apiInstance = new CaseAnnotationsApi();
BigDecimal belongsTo = new BigDecimal(); // BigDecimal | 
BigDecimal label = new BigDecimal(); // BigDecimal | 
Integer limit = 56; // Integer | Number of results to return per page.
Integer offset = 56; // Integer | The initial index from which to return the results.
try {
    InlineResponse2001 result = apiInstance.caseAnnotationsList(belongsTo, label, limit, offset);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CaseAnnotationsApi#caseAnnotationsList");
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

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="caseAnnotationsPartialUpdate"></a>
# **caseAnnotationsPartialUpdate**
> CaseAnnotation caseAnnotationsPartialUpdate(id, data)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CaseAnnotationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CaseAnnotationsApi apiInstance = new CaseAnnotationsApi();
Integer id = 56; // Integer | A unique integer value identifying this case annotation.
CaseAnnotation data = new CaseAnnotation(); // CaseAnnotation | 
try {
    CaseAnnotation result = apiInstance.caseAnnotationsPartialUpdate(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CaseAnnotationsApi#caseAnnotationsPartialUpdate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this case annotation. |
 **data** | [**CaseAnnotation**](CaseAnnotation.md)|  |

### Return type

[**CaseAnnotation**](CaseAnnotation.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="caseAnnotationsRead"></a>
# **caseAnnotationsRead**
> CaseAnnotation caseAnnotationsRead(id)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CaseAnnotationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CaseAnnotationsApi apiInstance = new CaseAnnotationsApi();
Integer id = 56; // Integer | A unique integer value identifying this case annotation.
try {
    CaseAnnotation result = apiInstance.caseAnnotationsRead(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CaseAnnotationsApi#caseAnnotationsRead");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this case annotation. |

### Return type

[**CaseAnnotation**](CaseAnnotation.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="caseAnnotationsUpdate"></a>
# **caseAnnotationsUpdate**
> CaseAnnotation caseAnnotationsUpdate(id, data)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CaseAnnotationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CaseAnnotationsApi apiInstance = new CaseAnnotationsApi();
Integer id = 56; // Integer | A unique integer value identifying this case annotation.
CaseAnnotation data = new CaseAnnotation(); // CaseAnnotation | 
try {
    CaseAnnotation result = apiInstance.caseAnnotationsUpdate(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CaseAnnotationsApi#caseAnnotationsUpdate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this case annotation. |
 **data** | [**CaseAnnotation**](CaseAnnotation.md)|  |

### Return type

[**CaseAnnotation**](CaseAnnotation.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

