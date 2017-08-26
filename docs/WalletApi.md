# MinergateApi.WalletApi

All URIs are relative to *https://api.minergate.com/1.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getBalance**](WalletApi.md#getBalance) | **GET** /balance | Balance
[**getTransfers**](WalletApi.md#getTransfers) | **GET** /transfers/{cc} | Transfers
[**getWithdrawals**](WalletApi.md#getWithdrawals) | **GET** /withdrawals/{cc} | Withdrawals by Blockchain


<a name="getBalance"></a>
# **getBalance**
> Object getBalance()

Balance

Returns the user’s balance. **Requires authorization.** 

### Example
```javascript
var MinergateApi = require('minergate_api');
var defaultClient = MinergateApi.ApiClient.default;

// Configure API key authorization: token
var token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

var apiInstance = new MinergateApi.WalletApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.getBalance(callback);
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

<a name="getTransfers"></a>
# **getTransfers**
> getTransfers(cc)

Transfers

Returns the list of user’s transfers. **Requires authorization.** 

### Example
```javascript
var MinergateApi = require('minergate_api');
var defaultClient = MinergateApi.ApiClient.default;

// Configure API key authorization: token
var token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

var apiInstance = new MinergateApi.WalletApi();

var cc = "cc_example"; // String | Shorthand name for crypto currency. e.g. Bitcoin = btc 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.getTransfers(cc, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **cc** | **String**| Shorthand name for crypto currency. e.g. Bitcoin &#x3D; btc  | 

### Return type

null (empty response body)

### Authorization

[token](../README.md#token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getWithdrawals"></a>
# **getWithdrawals**
> getWithdrawals(cc)

Withdrawals by Blockchain

Returns the list of user’s withdrawals for  all the currencies or a specific currency  if such parameter is set.  **Requires authorization.** 

### Example
```javascript
var MinergateApi = require('minergate_api');
var defaultClient = MinergateApi.ApiClient.default;

// Configure API key authorization: token
var token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

var apiInstance = new MinergateApi.WalletApi();

var cc = "cc_example"; // String | Shorthand name for crypto currency. e.g. Bitcoin = btc 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.getWithdrawals(cc, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **cc** | **String**| Shorthand name for crypto currency. e.g. Bitcoin &#x3D; btc  | 

### Return type

null (empty response body)

### Authorization

[token](../README.md#token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

