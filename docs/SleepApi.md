# swagger_client.SleepApi

All URIs are relative to *https://edgestream-egress.azurewebsites.net/curaegis/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sleep_log_get_by_id**](SleepApi.md#sleep_log_get_by_id) | **GET** /{id}/sleep/{date} | 
[**sleep_log_get_range**](SleepApi.md#sleep_log_get_range) | **GET** /{id}/sleep/{resource}/{date}/{period} | 
[**sleep_log_get_timeseries**](SleepApi.md#sleep_log_get_timeseries) | **GET** /{id}/sleep/{resource}/range/{basedate}/{enddate} | 


# **sleep_log_get_by_id**
> object sleep_log_get_by_id(id, _date)



Get sleep log by user id and date

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
api_instance = swagger_client.SleepApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | 3P7JCB
_date = '_date_example' # str | the date of records to be returned. In the format yyyy-MM-dd

try:
    api_response = api_instance.sleep_log_get_by_id(id, _date)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling SleepApi->sleep_log_get_by_id: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| 3P7JCB | 
 **_date** | **str**| the date of records to be returned. In the format yyyy-MM-dd | 

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sleep_log_get_range**
> object sleep_log_get_range(id, resource, _date, period)



Get sleep timeseries log by user id and date

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
api_instance = swagger_client.SleepApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | 3P7JCB
resource = 'resource_example' # str | the resource path
_date = '_date_example' # str | the date of records to be returned. In the format yyyy-MM-dd
period = 'period_example' # str | the range for which data will be returned. Options are 1d, 7d, 30d, 1w, 1m, 3m, 6m, 1y, or max

try:
    api_response = api_instance.sleep_log_get_range(id, resource, _date, period)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling SleepApi->sleep_log_get_range: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| 3P7JCB | 
 **resource** | **str**| the resource path | 
 **_date** | **str**| the date of records to be returned. In the format yyyy-MM-dd | 
 **period** | **str**| the range for which data will be returned. Options are 1d, 7d, 30d, 1w, 1m, 3m, 6m, 1y, or max | 

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sleep_log_get_timeseries**
> object sleep_log_get_timeseries(id, resource, basedate, enddate)



Get sleep timeseries log by user id and date range

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
api_instance = swagger_client.SleepApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | 3P7JCB
resource = 'resource_example' # str | the resource path
basedate = 'basedate_example' # str | the range start date, in the format yyyy-MM-dd or today
enddate = 'enddate_example' # str | the end date of the range

try:
    api_response = api_instance.sleep_log_get_timeseries(id, resource, basedate, enddate)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling SleepApi->sleep_log_get_timeseries: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| 3P7JCB | 
 **resource** | **str**| the resource path | 
 **basedate** | **str**| the range start date, in the format yyyy-MM-dd or today | 
 **enddate** | **str**| the end date of the range | 

### Return type

**object**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

