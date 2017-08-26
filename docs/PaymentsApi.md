# MinergateApi.PaymentsApi

All URIs are relative to *https://api.minergate.com/1.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getInvoiceById**](PaymentsApi.md#getInvoiceById) | **GET** /invoices/{INVOICE_ID} | Invoices by Id
[**getInvoices**](PaymentsApi.md#getInvoices) | **GET** /invoices | Invoices


<a name="getInvoiceById"></a>
# **getInvoiceById**
> getInvoiceById(INVOICE_ID)

Invoices by Id

Returns the specified invoice. **Requires authorization.** 

### Example
```javascript
var MinergateApi = require('minergate_api');
var defaultClient = MinergateApi.ApiClient.default;

// Configure API key authorization: token
var token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

var apiInstance = new MinergateApi.PaymentsApi();

var INVOICE_ID = "INVOICE_ID_example"; // String | Id of Invoice


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.getInvoiceById(INVOICE_ID, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **INVOICE_ID** | **String**| Id of Invoice | 

### Return type

null (empty response body)

### Authorization

[token](../README.md#token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getInvoices"></a>
# **getInvoices**
> getInvoices()

Invoices

Returns the list of user&#39;s invoices. **Requires authorization.** 

### Example
```javascript
var MinergateApi = require('minergate_api');
var defaultClient = MinergateApi.ApiClient.default;

// Configure API key authorization: token
var token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

var apiInstance = new MinergateApi.PaymentsApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.getInvoices(callback);
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

[token](../README.md#token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

