# swagger_client.ManagerApi

All URIs are relative to *https://edgestream-egress.azurewebsites.net/curaegis/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_cura_by_users**](ManagerApi.md#get_cura_by_users) | **POST** /dispatchedusers | 


# **get_cura_by_users**
> list[InlineResponse2002] get_cura_by_users(body)



Get Dispatched Users Cura score

### Example
```python
from __future__ import print_function
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: ApiKeyAuth
configuration = swagger_client.Configuration()
configuration.api_key['X-API-KEY'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['X-API-KEY'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.ManagerApi(swagger_client.ApiClient(configuration))
body = [swagger_client.Body()] # list[Body] | TenantID UserID list

try:
    api_response = api_instance.get_cura_by_users(body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling ManagerApi->get_cura_by_users: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**list[Body]**](Body.md)| TenantID UserID list | 

### Return type

[**list[InlineResponse2002]**](InlineResponse2002.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

