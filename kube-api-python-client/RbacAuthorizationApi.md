# swagger_client.RbacAuthorizationApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_rbac_authorization_api_group**](RbacAuthorizationApi.md#get_rbac_authorization_api_group) | **GET** /apis/rbac.authorization.k8s.io/ | 


# **get_rbac_authorization_api_group**
> IoK8sApimachineryPkgApisMetaV1APIGroup get_rbac_authorization_api_group()



get information of a group

### Example 
```python
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: BearerToken
swagger_client.configuration.api_key['authorization'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# swagger_client.configuration.api_key_prefix['authorization'] = 'Bearer'

# create an instance of the API class
api_instance = swagger_client.RbacAuthorizationApi()

try: 
    api_response = api_instance.get_rbac_authorization_api_group()
    pprint(api_response)
except ApiException as e:
    print "Exception when calling RbacAuthorizationApi->get_rbac_authorization_api_group: %s\n" % e
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**IoK8sApimachineryPkgApisMetaV1APIGroup**](IoK8sApimachineryPkgApisMetaV1APIGroup.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

 - **Content-Type**: application/json, application/yaml, application/vnd.kubernetes.protobuf
 - **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
