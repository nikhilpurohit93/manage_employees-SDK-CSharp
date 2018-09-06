# IO.Swagger.Api.AuthenticationApi

All URIs are relative to *https://mg-eval-test.apigee.net/demo/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**OauthTokenPost**](AuthenticationApi.md#oauthtokenpost) | **POST** /oauth/token | Get Access Token


<a name="oauthtokenpost"></a>
# **OauthTokenPost**
> AccessToken OauthTokenPost (string grantType = null, string clientId = null, string clientSecret = null)

Get Access Token

Verify client credentials and returns a bearer token.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class OauthTokenPostExample
    {
        public void main()
        {
            var apiInstance = new AuthenticationApi();
            var grantType = grantType_example;  // string | The grant type for OAuth2.0 (optional)  (default to client_credentials)
            var clientId = clientId_example;  // string | Client ID (optional) 
            var clientSecret = clientSecret_example;  // string | Client Secret (optional) 

            try
            {
                // Get Access Token
                AccessToken result = apiInstance.OauthTokenPost(grantType, clientId, clientSecret);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling AuthenticationApi.OauthTokenPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **grantType** | **string**| The grant type for OAuth2.0 | [optional] [default to client_credentials]
 **clientId** | **string**| Client ID | [optional] 
 **clientSecret** | **string**| Client Secret | [optional] 

### Return type

[**AccessToken**](AccessToken.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

