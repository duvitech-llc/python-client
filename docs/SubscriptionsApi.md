# swagger_client.SubscriptionsApi

All URIs are relative to *https://edgestream-egress.azurewebsites.net/curaegis/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_subscription_by_id**](SubscriptionsApi.md#add_subscription_by_id) | **POST** /{id}/subscription/{resource} | 
[**delete_subscription_by_id**](SubscriptionsApi.md#delete_subscription_by_id) | **DELETE** /{id}/subscription/{resource} | 
[**get_subscribed_by_id**](SubscriptionsApi.md#get_subscribed_by_id) | **GET** /{id}/subscription/{resource} | 


# **add_subscription_by_id**
> add_subscription_by_id(id, resource)



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
api_instance = swagger_client.SubscriptionsApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | 3P7JCB
resource = 'resource_example' # str | the resource path

try:
    api_instance.add_subscription_by_id(id, resource)
except ApiException as e:
    print("Exception when calling SubscriptionsApi->add_subscription_by_id: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| 3P7JCB | 
 **resource** | **str**| the resource path | 

### Return type

void (empty response body)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_subscription_by_id**
> delete_subscription_by_id(id, resource)



Delete activity subscriptions

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
api_instance = swagger_client.SubscriptionsApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | 3P7JCB
resource = 'resource_example' # str | the resource path

try:
    api_instance.delete_subscription_by_id(id, resource)
except ApiException as e:
    print("Exception when calling SubscriptionsApi->delete_subscription_by_id: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| 3P7JCB | 
 **resource** | **str**| the resource path | 

### Return type

void (empty response body)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_subscribed_by_id**
> get_subscribed_by_id(id, resource)



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
api_instance = swagger_client.SubscriptionsApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | 3P7JCB
resource = 'resource_example' # str | the resource path

try:
    api_instance.get_subscribed_by_id(id, resource)
except ApiException as e:
    print("Exception when calling SubscriptionsApi->get_subscribed_by_id: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| 3P7JCB | 
 **resource** | **str**| the resource path | 

### Return type

void (empty response body)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

