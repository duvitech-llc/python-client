# swagger_client.SummaryApi

All URIs are relative to *https://edgestream-egress.azurewebsites.net/curaegis/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**activity_summary_get_by_id**](SummaryApi.md#activity_summary_get_by_id) | **GET** /{id}/activities | 
[**activity_summary_get_by_id_date**](SummaryApi.md#activity_summary_get_by_id_date) | **GET** /{id}/activities/date/{date} | 


# **activity_summary_get_by_id**
> object activity_summary_get_by_id(id)



Get current activity summary for user

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
api_instance = swagger_client.SummaryApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | 3P7JCB

try:
    api_response = api_instance.activity_summary_get_by_id(id)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling SummaryApi->activity_summary_get_by_id: %s\n" % e)
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

# **activity_summary_get_by_id_date**
> object activity_summary_get_by_id_date(id, _date)



Get activity summary by user id and date

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
api_instance = swagger_client.SummaryApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | 3P7JCB
_date = '_date_example' # str | the date in the format yyyy-MM-dd

try:
    api_response = api_instance.activity_summary_get_by_id_date(id, _date)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling SummaryApi->activity_summary_get_by_id_date: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| 3P7JCB | 
 **_date** | **str**| the date in the format yyyy-MM-dd | 

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

