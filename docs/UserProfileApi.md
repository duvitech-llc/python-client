# swagger_client.UserProfileApi

All URIs are relative to *https://edgestream-egress.azurewebsites.net/curaegis/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**activity_profile_get_by_id**](UserProfileApi.md#activity_profile_get_by_id) | **GET** /{id}/profile | 


# **activity_profile_get_by_id**
> object activity_profile_get_by_id(id)



Get current user profile

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
api_instance = swagger_client.UserProfileApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | 3P7JCB

try:
    api_response = api_instance.activity_profile_get_by_id(id)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling UserProfileApi->activity_profile_get_by_id: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| 3P7JCB | 

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

