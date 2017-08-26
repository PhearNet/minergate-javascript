# MinergateApi.ProfileApi

All URIs are relative to *https://api.minergate.com/1.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getProfileNickname**](ProfileApi.md#getProfileNickname) | **GET** /profile/nickname | Profile Nickname


<a name="getProfileNickname"></a>
# **getProfileNickname**
> getProfileNickname()

Profile Nickname

Returns the user’s nickname. **Requires authorization.** 

### Example
```javascript
var MinergateApi = require('minergate_api');
var defaultClient = MinergateApi.ApiClient.default;

// Configure API key authorization: token
var token = defaultClient.authentications['token'];
token.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//token.apiKeyPrefix = 'Token';

var apiInstance = new MinergateApi.ProfileApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.getProfileNickname(callback);
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

