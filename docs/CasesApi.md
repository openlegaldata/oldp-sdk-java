# CasesApi

All URIs are relative to *https://de.openlegaldata.io/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**casesCreate**](CasesApi.md#casesCreate) | **POST** /cases/ | 
[**casesDelete**](CasesApi.md#casesDelete) | **DELETE** /cases/{id}/ | 
[**casesList**](CasesApi.md#casesList) | **GET** /cases/ | 
[**casesPartialUpdate**](CasesApi.md#casesPartialUpdate) | **PATCH** /cases/{id}/ | 
[**casesRead**](CasesApi.md#casesRead) | **GET** /cases/{id}/ | 
[**casesSearchList**](CasesApi.md#casesSearchList) | **GET** /cases/search/ | 
[**casesUpdate**](CasesApi.md#casesUpdate) | **PUT** /cases/{id}/ | 


<a name="casesCreate"></a>
# **casesCreate**
> ModelCase casesCreate(data)



List view for cases

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CasesApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CasesApi apiInstance = new CasesApi();
ModelCase data = new ModelCase(); // ModelCase | 
try {
    ModelCase result = apiInstance.casesCreate(data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CasesApi#casesCreate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**ModelCase**](ModelCase.md)|  |

### Return type

[**ModelCase**](ModelCase.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="casesDelete"></a>
# **casesDelete**
> casesDelete(id)



List view for cases

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CasesApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CasesApi apiInstance = new CasesApi();
Integer id = 56; // Integer | A unique integer value identifying this case.
try {
    apiInstance.casesDelete(id);
} catch (ApiException e) {
    System.err.println("Exception when calling CasesApi#casesDelete");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this case. |

### Return type

null (empty response body)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="casesList"></a>
# **casesList**
> InlineResponse2003 casesList(ordering, date, slug, fileNumber, ecli, court, courtSlug, courtJurisdiction, courtLevelOfAppeal, courtState, page, pageSize)



List view for cases

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CasesApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CasesApi apiInstance = new CasesApi();
String ordering = "ordering_example"; // String | Which field to use when ordering the results.
String date = "date_example"; // String | 
String slug = "slug_example"; // String | 
String fileNumber = "fileNumber_example"; // String | 
String ecli = "ecli_example"; // String | 
BigDecimal court = new BigDecimal(); // BigDecimal | 
String courtSlug = "courtSlug_example"; // String | 
String courtJurisdiction = "courtJurisdiction_example"; // String | 
String courtLevelOfAppeal = "courtLevelOfAppeal_example"; // String | 
String courtState = "courtState_example"; // String | 
Integer page = 56; // Integer | A page number within the paginated result set.
Integer pageSize = 56; // Integer | Number of results to return per page.
try {
    InlineResponse2003 result = apiInstance.casesList(ordering, date, slug, fileNumber, ecli, court, courtSlug, courtJurisdiction, courtLevelOfAppeal, courtState, page, pageSize);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CasesApi#casesList");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ordering** | **String**| Which field to use when ordering the results. | [optional]
 **date** | **String**|  | [optional]
 **slug** | **String**|  | [optional]
 **fileNumber** | **String**|  | [optional]
 **ecli** | **String**|  | [optional]
 **court** | **BigDecimal**|  | [optional]
 **courtSlug** | **String**|  | [optional]
 **courtJurisdiction** | **String**|  | [optional]
 **courtLevelOfAppeal** | **String**|  | [optional]
 **courtState** | **String**|  | [optional]
 **page** | **Integer**| A page number within the paginated result set. | [optional]
 **pageSize** | **Integer**| Number of results to return per page. | [optional]

### Return type

[**InlineResponse2003**](InlineResponse2003.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="casesPartialUpdate"></a>
# **casesPartialUpdate**
> ModelCase casesPartialUpdate(id, data)



List view for cases

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CasesApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CasesApi apiInstance = new CasesApi();
Integer id = 56; // Integer | A unique integer value identifying this case.
ModelCase data = new ModelCase(); // ModelCase | 
try {
    ModelCase result = apiInstance.casesPartialUpdate(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CasesApi#casesPartialUpdate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this case. |
 **data** | [**ModelCase**](ModelCase.md)|  |

### Return type

[**ModelCase**](ModelCase.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="casesRead"></a>
# **casesRead**
> ModelCase casesRead(id)



List view for cases

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CasesApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CasesApi apiInstance = new CasesApi();
Integer id = 56; // Integer | A unique integer value identifying this case.
try {
    ModelCase result = apiInstance.casesRead(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CasesApi#casesRead");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this case. |

### Return type

[**ModelCase**](ModelCase.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="casesSearchList"></a>
# **casesSearchList**
> InlineResponse2004 casesSearchList(text, facetModelName, date, courtJurisdiction, courtLevelOfAppeal, decisionType, court, page, pageSize)



Search view (list only)

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CasesApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CasesApi apiInstance = new CasesApi();
String text = "text_example"; // String | Search query on text content (Lucence syntax support).
String facetModelName = "facetModelName_example"; // String | facet_model_name
String date = "date_example"; // String | date
String courtJurisdiction = "courtJurisdiction_example"; // String | court_jurisdiction
String courtLevelOfAppeal = "courtLevelOfAppeal_example"; // String | court_level_of_appeal
String decisionType = "decisionType_example"; // String | decision_type
String court = "court_example"; // String | court
Integer page = 56; // Integer | A page number within the paginated result set.
Integer pageSize = 56; // Integer | Number of results to return per page.
try {
    InlineResponse2004 result = apiInstance.casesSearchList(text, facetModelName, date, courtJurisdiction, courtLevelOfAppeal, decisionType, court, page, pageSize);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CasesApi#casesSearchList");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **text** | **String**| Search query on text content (Lucence syntax support). |
 **facetModelName** | **String**| facet_model_name | [optional]
 **date** | **String**| date | [optional]
 **courtJurisdiction** | **String**| court_jurisdiction | [optional]
 **courtLevelOfAppeal** | **String**| court_level_of_appeal | [optional]
 **decisionType** | **String**| decision_type | [optional]
 **court** | **String**| court | [optional]
 **page** | **Integer**| A page number within the paginated result set. | [optional]
 **pageSize** | **Integer**| Number of results to return per page. | [optional]

### Return type

[**InlineResponse2004**](InlineResponse2004.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="casesUpdate"></a>
# **casesUpdate**
> ModelCase casesUpdate(id, data)



List view for cases

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.CasesApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: api_key
ApiKeyAuth api_key = (ApiKeyAuth) defaultClient.getAuthentication("api_key");
api_key.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//api_key.setApiKeyPrefix("Token");

CasesApi apiInstance = new CasesApi();
Integer id = 56; // Integer | A unique integer value identifying this case.
ModelCase data = new ModelCase(); // ModelCase | 
try {
    ModelCase result = apiInstance.casesUpdate(id, data);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CasesApi#casesUpdate");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| A unique integer value identifying this case. |
 **data** | [**ModelCase**](ModelCase.md)|  |

### Return type

[**ModelCase**](ModelCase.md)

### Authorization

[api_key](../README.md#api_key)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

