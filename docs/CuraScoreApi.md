# swagger_client.CuraScoreApi

All URIs are relative to *https://edgestream-egress.azurewebsites.net/curaegis/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_cura_by_id**](CuraScoreApi.md#get_cura_by_id) | **GET** /curascore | 
[**get_cura_ex_by_id**](CuraScoreApi.md#get_cura_ex_by_id) | **GET** /curascoreex | 


# **get_cura_by_id**
> object get_cura_by_id(id=id)



Get Individuals Cura score

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
api_instance = swagger_client.CuraScoreApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | id to filter by (optional)

try:
    api_response = api_instance.get_cura_by_id(id=id)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling CuraScoreApi->get_cura_by_id: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| id to filter by | [optional] 

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_cura_ex_by_id**
> object get_cura_ex_by_id(id=id)



Get Individuals Cura Different return format score

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
api_instance = swagger_client.CuraScoreApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | id to filter by (optional)

try:
    api_response = api_instance.get_cura_ex_by_id(id=id)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling CuraScoreApi->get_cura_ex_by_id: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| id to filter by | [optional] 

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

