# MinergateApi.PublicApi

All URIs are relative to *https://api.minergate.com/1.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getBlockchainStatus**](PublicApi.md#getBlockchainStatus) | **GET** /{cc}/status | Blockchain Status
[**getPoolProfitRating**](PublicApi.md#getPoolProfitRating) | **GET** /pool/profit-rating | Pool Profit-Rating
[**getPoolTopHashrate**](PublicApi.md#getPoolTopHashrate) | **GET** /pool/top/hashrate | Pool Top Hashrate


<a name="getBlockchainStatus"></a>
# **getBlockchainStatus**
> Object getBlockchainStatus(cc)

Blockchain Status

Returns the blockchain data of the specified currency. Returned values are as follows: chain height, last block timestamp, network difficulty, network hashrate, base reward. 

### Example
```javascript
var MinergateApi = require('minergate_api');

var apiInstance = new MinergateApi.PublicApi();

var cc = "cc_example"; // String | Shorthand name for crypto currency. e.g. Bitcoin = btc 


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.getBlockchainStatus(cc, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **cc** | **String**| Shorthand name for crypto currency. e.g. Bitcoin &#x3D; btc  | 

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getPoolProfitRating"></a>
# **getPoolProfitRating**
> [&#39;String&#39;] getPoolProfitRating()

Pool Profit-Rating

Returns the list of all currencies sorted by profitability. 

### Example
```javascript
var MinergateApi = require('minergate_api');

var apiInstance = new MinergateApi.PublicApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.getPoolProfitRating(callback);
```

### Parameters
This endpoint does not need any parameter.

### Return type

**[&#39;String&#39;]**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getPoolTopHashrate"></a>
# **getPoolTopHashrate**
> Object getPoolTopHashrate()

Pool Top Hashrate

Returns the lists of top 10 miners for each currency. 

### Example
```javascript
var MinergateApi = require('minergate_api');

var apiInstance = new MinergateApi.PublicApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.getPoolTopHashrate(callback);
```

### Parameters
This endpoint does not need any parameter.

### Return type

**Object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

