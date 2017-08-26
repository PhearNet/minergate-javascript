# MinergateApi.AffiliatesApi

All URIs are relative to *https://api.minergate.com/1.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getAffiliateChildren**](AffiliatesApi.md#getAffiliateChildren) | **GET** /affiliate/childrens | Affiliate Childrens
[**getAffiliateLinks**](AffiliatesApi.md#getAffiliateLinks) | **GET** /affiliate/links | Affiliate Links
[**getAffiliateProfit**](AffiliatesApi.md#getAffiliateProfit) | **GET** /affiliate/profit | Affiliate Profit


<a name="getAffiliateChildren"></a>
# **getAffiliateChildren**
> Object getAffiliateChildren()

Affiliate Childrens

Returns the list of user’s affiliates. **Requires authorization.** 

### Example
```javascript
var MinergateApi = require('minergate_api');
var defaultClient = MinergateApi.ApiClient.default;

// Configure API key authorization: token
var token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

var apiInstance = new MinergateApi.AffiliatesApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.getAffiliateChildren(callback);
```

### Parameters
This endpoint does not need any parameter.

### Return type

**Object**

### Authorization

[token](../README.md#token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAffiliateLinks"></a>
# **getAffiliateLinks**
> Object getAffiliateLinks()

Affiliate Links

Returns the list of user’s affiliate links. **Requires authorization.** 

### Example
```javascript
var MinergateApi = require('minergate_api');
var defaultClient = MinergateApi.ApiClient.default;

// Configure API key authorization: token
var token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

var apiInstance = new MinergateApi.AffiliatesApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.getAffiliateLinks(callback);
```

### Parameters
This endpoint does not need any parameter.

### Return type

**Object**

### Authorization

[token](../README.md#token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAffiliateProfit"></a>
# **getAffiliateProfit**
> Object getAffiliateProfit()

Affiliate Profit

Returns the user’s income from affiliates. **Requires authorization.** 

### Example
```javascript
var MinergateApi = require('minergate_api');
var defaultClient = MinergateApi.ApiClient.default;

// Configure API key authorization: token
var token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

var apiInstance = new MinergateApi.AffiliatesApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.getAffiliateProfit(callback);
```

### Parameters
This endpoint does not need any parameter.

### Return type

**Object**

### Authorization

[token](../README.md#token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

