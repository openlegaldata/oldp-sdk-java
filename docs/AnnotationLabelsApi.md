# AnnotationLabelsApi

All URIs are relative to *https://de.openlegaldata.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**annotationLabelsCreate**](AnnotationLabelsApi.md#annotationLabelsCreate) | **POST** /annotation_labels/ | 
[**annotationLabelsDelete**](AnnotationLabelsApi.md#annotationLabelsDelete) | **DELETE** /annotation_labels/{id}/ | 
[**annotationLabelsList**](AnnotationLabelsApi.md#annotationLabelsList) | **GET** /annotation_labels/ | 
[**annotationLabelsPartialUpdate**](AnnotationLabelsApi.md#annotationLabelsPartialUpdate) | **PATCH** /annotation_labels/{id}/ | 
[**annotationLabelsRead**](AnnotationLabelsApi.md#annotationLabelsRead) | **GET** /annotation_labels/{id}/ | 
[**annotationLabelsUpdate**](AnnotationLabelsApi.md#annotationLabelsUpdate) | **PUT** /annotation_labels/{id}/ | 


<a name="annotationLabelsCreate"></a>
# **annotationLabelsCreate**
> AnnotationLabel annotationLabelsCreate(data)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.AnnotationLabelsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

AnnotationLabelsApi apiInstance = new AnnotationLabelsApi();
AnnotationLabel data = new AnnotationLabel(); // AnnotationLabel | 
try {
    AnnotationLabel result = apiInstance.annotationLabelsCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AnnotationLabelsApi#annotationLabelsCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**AnnotationLabel**](AnnotationLabel.md)|  |

### Return type

[**AnnotationLabel**](AnnotationLabel.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="annotationLabelsDelete"></a>
# **annotationLabelsDelete**
> annotationLabelsDelete(id)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.AnnotationLabelsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

AnnotationLabelsApi apiInstance = new AnnotationLabelsApi();
Integer id = 56; // Integer | A unique integer value identifying this Label.
try {
    apiInstance.annotationLabelsDelete(id);
} catch (ApiException e) {
    System.err.println("Exception when calling AnnotationLabelsApi#annotationLabelsDelete");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this Label. |

### Return type

null (empty response body)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="annotationLabelsList"></a>
# **annotationLabelsList**
> InlineResponse200 annotationLabelsList(ordering, owner, slug, _private, trusted, limit, offset)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.AnnotationLabelsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

AnnotationLabelsApi apiInstance = new AnnotationLabelsApi();
String ordering = "ordering_example"; // String | Which field to use when ordering the results.
BigDecimal owner = new BigDecimal(); // BigDecimal | 
String slug = "slug_example"; // String | 
String _private = "_private_example"; // String | 
String trusted = "trusted_example"; // String | 
Integer limit = 56; // Integer | Number of results to return per page.
Integer offset = 56; // Integer | The initial index from which to return the results.
try {
    InlineResponse200 result = apiInstance.annotationLabelsList(ordering, owner, slug, _private, trusted, limit, offset);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AnnotationLabelsApi#annotationLabelsList");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ordering** | **String**| Which field to use when ordering the results. | [optional]
 **owner** | **BigDecimal**|  | [optional]
 **slug** | **String**|  | [optional]
 **_private** | **String**|  | [optional]
 **trusted** | **String**|  | [optional]
 **limit** | **Integer**| Number of results to return per page. | [optional]
 **offset** | **Integer**| The initial index from which to return the results. | [optional]

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="annotationLabelsPartialUpdate"></a>
# **annotationLabelsPartialUpdate**
> AnnotationLabel annotationLabelsPartialUpdate(id, data)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.AnnotationLabelsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

AnnotationLabelsApi apiInstance = new AnnotationLabelsApi();
Integer id = 56; // Integer | A unique integer value identifying this Label.
AnnotationLabel data = new AnnotationLabel(); // AnnotationLabel | 
try {
    AnnotationLabel result = apiInstance.annotationLabelsPartialUpdate(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AnnotationLabelsApi#annotationLabelsPartialUpdate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this Label. |
 **data** | [**AnnotationLabel**](AnnotationLabel.md)|  |

### Return type

[**AnnotationLabel**](AnnotationLabel.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="annotationLabelsRead"></a>
# **annotationLabelsRead**
> AnnotationLabel annotationLabelsRead(id)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.AnnotationLabelsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

AnnotationLabelsApi apiInstance = new AnnotationLabelsApi();
Integer id = 56; // Integer | A unique integer value identifying this Label.
try {
    AnnotationLabel result = apiInstance.annotationLabelsRead(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AnnotationLabelsApi#annotationLabelsRead");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this Label. |

### Return type

[**AnnotationLabel**](AnnotationLabel.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="annotationLabelsUpdate"></a>
# **annotationLabelsUpdate**
> AnnotationLabel annotationLabelsUpdate(id, data)





### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.AnnotationLabelsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

AnnotationLabelsApi apiInstance = new AnnotationLabelsApi();
Integer id = 56; // Integer | A unique integer value identifying this Label.
AnnotationLabel data = new AnnotationLabel(); // AnnotationLabel | 
try {
    AnnotationLabel result = apiInstance.annotationLabelsUpdate(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AnnotationLabelsApi#annotationLabelsUpdate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this Label. |
 **data** | [**AnnotationLabel**](AnnotationLabel.md)|  |

### Return type

[**AnnotationLabel**](AnnotationLabel.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

