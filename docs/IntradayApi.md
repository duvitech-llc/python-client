# swagger_client.IntradayApi

All URIs are relative to *https://edgestream-egress.azurewebsites.net/curaegis/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**intraday_get_by_default**](IntradayApi.md#intraday_get_by_default) | **GET** /{id}/intraday/{resource}/date/{date} | 
[**intraday_get_by_id**](IntradayApi.md#intraday_get_by_id) | **GET** /{id}/intraday/{resource}/date/{date}/{detail}/{stime}/{etime} | 


# **intraday_get_by_default**
> object intraday_get_by_default(id, resource, _date)



Get intraday logs by user id and date

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
api_instance = swagger_client.IntradayApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | 3P7JCB
resource = 'resource_example' # str | the resource path
_date = '_date_example' # str | the date in the format yyyy-MM-dd or today

try:
    api_response = api_instance.intraday_get_by_default(id, resource, _date)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling IntradayApi->intraday_get_by_default: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| 3P7JCB | 
 **resource** | **str**| the resource path | 
 **_date** | **str**| the date in the format yyyy-MM-dd or today | 

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **intraday_get_by_id**
> object intraday_get_by_id(id, resource, _date, detail, stime, etime)



Get intraday logs by user id and date

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
api_instance = swagger_client.IntradayApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | 3P7JCB
resource = 'resource_example' # str | the resource path
_date = '_date_example' # str | the date in the format yyyy-MM-dd or today
detail = 'detail_example' # str | The range for which data will be returned. Options are 1sec(only heartrate),  1min, 15min(not valid for heart)
stime = 'stime_example' # str | The start of the period, in the format HH:mm
etime = 'etime_example' # str | The start of the period, in the format HH:mm

try:
    api_response = api_instance.intraday_get_by_id(id, resource, _date, detail, stime, etime)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling IntradayApi->intraday_get_by_id: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| 3P7JCB | 
 **resource** | **str**| the resource path | 
 **_date** | **str**| the date in the format yyyy-MM-dd or today | 
 **detail** | **str**| The range for which data will be returned. Options are 1sec(only heartrate),  1min, 15min(not valid for heart) | 
 **stime** | **str**| The start of the period, in the format HH:mm | 
 **etime** | **str**| The start of the period, in the format HH:mm | 

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

