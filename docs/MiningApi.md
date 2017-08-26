# MinergateApi.MiningApi

All URIs are relative to *https://api.minergate.com/1.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getWorkers**](MiningApi.md#getWorkers) | **GET** /workers | Workers
[**miningStats**](MiningApi.md#miningStats) | **GET** /mining/stats | Mining Stats


<a name="getWorkers"></a>
# **getWorkers**
> getWorkers()

Workers

Returns the number of user’s active workers. **Requires authorization.** 

### Example
```javascript
var MinergateApi = require('minergate_api');
var defaultClient = MinergateApi.ApiClient.default;

// Configure API key authorization: token
var token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

var apiInstance = new MinergateApi.MiningApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.getWorkers(callback);
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

<a name="miningStats"></a>
# **miningStats**
> miningStats()

Mining Stats

Returns the user’s mining statistics. **Requires authorization.** 

### Example
```javascript
var MinergateApi = require('minergate_api');
var defaultClient = MinergateApi.ApiClient.default;

// Configure API key authorization: token
var token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

var apiInstance = new MinergateApi.MiningApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.miningStats(callback);
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

