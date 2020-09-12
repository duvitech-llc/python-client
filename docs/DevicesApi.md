# swagger_client.DevicesApi

All URIs are relative to *https://edgestream-egress.azurewebsites.net/curaegis/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_device_by_id**](DevicesApi.md#add_device_by_id) | **POST** /register | 
[**add_profile_by_id**](DevicesApi.md#add_profile_by_id) | **POST** /profile | 
[**get_device_list**](DevicesApi.md#get_device_list) | **GET** /devices | 
[**get_profile_by_id**](DevicesApi.md#get_profile_by_id) | **GET** /profile | 


# **add_device_by_id**
> Registration add_device_by_id(registration)



Register device with platform

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
api_instance = swagger_client.DevicesApi(swagger_client.ApiClient(configuration))
registration = swagger_client.Registration() # Registration | device to add to the platform

try:
    api_response = api_instance.add_device_by_id(registration)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DevicesApi->add_device_by_id: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registration** | [**Registration**](Registration.md)| device to add to the platform | 

### Return type

[**Registration**](Registration.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **add_profile_by_id**
> Profile add_profile_by_id(profile)



Register profile data with platform

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
api_instance = swagger_client.DevicesApi(swagger_client.ApiClient(configuration))
profile = swagger_client.Profile() # Profile | profile data to add to the platform

try:
    api_response = api_instance.add_profile_by_id(profile)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DevicesApi->add_profile_by_id: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile** | [**Profile**](Profile.md)| profile data to add to the platform | 

### Return type

[**Profile**](Profile.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_device_list**
> list[InlineResponse200] get_device_list(id=id)



Get registered device list

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
api_instance = swagger_client.DevicesApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | id to filter by (optional)

try:
    api_response = api_instance.get_device_list(id=id)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DevicesApi->get_device_list: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| id to filter by | [optional] 

### Return type

[**list[InlineResponse200]**](InlineResponse200.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_profile_by_id**
> InlineResponse2001 get_profile_by_id(tenantid, userid)



Register profile data with platform

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
api_instance = swagger_client.DevicesApi(swagger_client.ApiClient(configuration))
tenantid = 8.14 # float | Tenant ID
userid = 8.14 # float | User ID

try:
    api_response = api_instance.get_profile_by_id(tenantid, userid)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling DevicesApi->get_profile_by_id: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **tenantid** | **float**| Tenant ID | 
 **userid** | **float**| User ID | 

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

