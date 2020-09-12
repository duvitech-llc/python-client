# swagger_client.ResourcesApi

All URIs are relative to *https://edgestream-egress.azurewebsites.net/curaegis/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**resourcelog_get_by_date_range**](ResourcesApi.md#resourcelog_get_by_date_range) | **GET** /{id}/activities/{resource}/range/{basedate}/{enddate} | 
[**resourcelog_get_by_id**](ResourcesApi.md#resourcelog_get_by_id) | **GET** /{id}/activities/{resource}/date/{date}/{period} | 


# **resourcelog_get_by_date_range**
> InlineResponse2003 resourcelog_get_by_date_range(id, resource, basedate, enddate)



Get resource timeseries log by user id and date range

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
api_instance = swagger_client.ResourcesApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | 3P7JCB
resource = 'resource_example' # str | the resource path
basedate = 'basedate_example' # str | the range start date, in the format yyyy-MM-dd or today
enddate = 'enddate_example' # str | the end date of the range

try:
    api_response = api_instance.resourcelog_get_by_date_range(id, resource, basedate, enddate)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling ResourcesApi->resourcelog_get_by_date_range: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| 3P7JCB | 
 **resource** | **str**| the resource path | 
 **basedate** | **str**| the range start date, in the format yyyy-MM-dd or today | 
 **enddate** | **str**| the end date of the range | 

### Return type

[**InlineResponse2003**](InlineResponse2003.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **resourcelog_get_by_id**
> InlineResponse2003 resourcelog_get_by_id(id, resource, _date, period)



Get resource log by user id and date

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
api_instance = swagger_client.ResourcesApi(swagger_client.ApiClient(configuration))
id = 'id_example' # str | 3P7JCB
resource = 'resource_example' # str | the resource path
_date = '_date_example' # str | the end date of the period specified in the format yyyy-MM-dd or today
period = 'period_example' # str | The range for which data will be returned. Options are 1d, 7d, 30d, 1w, 1m

try:
    api_response = api_instance.resourcelog_get_by_id(id, resource, _date, period)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling ResourcesApi->resourcelog_get_by_id: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| 3P7JCB | 
 **resource** | **str**| the resource path | 
 **_date** | **str**| the end date of the period specified in the format yyyy-MM-dd or today | 
 **period** | **str**| The range for which data will be returned. Options are 1d, 7d, 30d, 1w, 1m | 

### Return type

[**InlineResponse2003**](InlineResponse2003.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

