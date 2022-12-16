<a name="__pageTop"></a>
# openapi_client.apis.tags.admissionregistration_v1_api.AdmissionregistrationV1Api

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_admissionregistration_v1_mutating_webhook_configuration**](#create_admissionregistration_v1_mutating_webhook_configuration) | **post** /apis/admissionregistration.k8s.io/v1/mutatingwebhookconfigurations | 
[**create_admissionregistration_v1_validating_webhook_configuration**](#create_admissionregistration_v1_validating_webhook_configuration) | **post** /apis/admissionregistration.k8s.io/v1/validatingwebhookconfigurations | 
[**delete_admissionregistration_v1_collection_mutating_webhook_configuration**](#delete_admissionregistration_v1_collection_mutating_webhook_configuration) | **delete** /apis/admissionregistration.k8s.io/v1/mutatingwebhookconfigurations | 
[**delete_admissionregistration_v1_collection_validating_webhook_configuration**](#delete_admissionregistration_v1_collection_validating_webhook_configuration) | **delete** /apis/admissionregistration.k8s.io/v1/validatingwebhookconfigurations | 
[**delete_admissionregistration_v1_mutating_webhook_configuration**](#delete_admissionregistration_v1_mutating_webhook_configuration) | **delete** /apis/admissionregistration.k8s.io/v1/mutatingwebhookconfigurations/{name} | 
[**delete_admissionregistration_v1_validating_webhook_configuration**](#delete_admissionregistration_v1_validating_webhook_configuration) | **delete** /apis/admissionregistration.k8s.io/v1/validatingwebhookconfigurations/{name} | 
[**get_admissionregistration_v1_api_resources**](#get_admissionregistration_v1_api_resources) | **get** /apis/admissionregistration.k8s.io/v1/ | 
[**list_admissionregistration_v1_mutating_webhook_configuration**](#list_admissionregistration_v1_mutating_webhook_configuration) | **get** /apis/admissionregistration.k8s.io/v1/mutatingwebhookconfigurations | 
[**list_admissionregistration_v1_validating_webhook_configuration**](#list_admissionregistration_v1_validating_webhook_configuration) | **get** /apis/admissionregistration.k8s.io/v1/validatingwebhookconfigurations | 
[**patch_admissionregistration_v1_mutating_webhook_configuration**](#patch_admissionregistration_v1_mutating_webhook_configuration) | **patch** /apis/admissionregistration.k8s.io/v1/mutatingwebhookconfigurations/{name} | 
[**patch_admissionregistration_v1_validating_webhook_configuration**](#patch_admissionregistration_v1_validating_webhook_configuration) | **patch** /apis/admissionregistration.k8s.io/v1/validatingwebhookconfigurations/{name} | 
[**read_admissionregistration_v1_mutating_webhook_configuration**](#read_admissionregistration_v1_mutating_webhook_configuration) | **get** /apis/admissionregistration.k8s.io/v1/mutatingwebhookconfigurations/{name} | 
[**read_admissionregistration_v1_validating_webhook_configuration**](#read_admissionregistration_v1_validating_webhook_configuration) | **get** /apis/admissionregistration.k8s.io/v1/validatingwebhookconfigurations/{name} | 
[**replace_admissionregistration_v1_mutating_webhook_configuration**](#replace_admissionregistration_v1_mutating_webhook_configuration) | **put** /apis/admissionregistration.k8s.io/v1/mutatingwebhookconfigurations/{name} | 
[**replace_admissionregistration_v1_validating_webhook_configuration**](#replace_admissionregistration_v1_validating_webhook_configuration) | **put** /apis/admissionregistration.k8s.io/v1/validatingwebhookconfigurations/{name} | 
[**watch_admissionregistration_v1_mutating_webhook_configuration**](#watch_admissionregistration_v1_mutating_webhook_configuration) | **get** /apis/admissionregistration.k8s.io/v1/watch/mutatingwebhookconfigurations/{name} | 
[**watch_admissionregistration_v1_mutating_webhook_configuration_list**](#watch_admissionregistration_v1_mutating_webhook_configuration_list) | **get** /apis/admissionregistration.k8s.io/v1/watch/mutatingwebhookconfigurations | 
[**watch_admissionregistration_v1_validating_webhook_configuration**](#watch_admissionregistration_v1_validating_webhook_configuration) | **get** /apis/admissionregistration.k8s.io/v1/watch/validatingwebhookconfigurations/{name} | 
[**watch_admissionregistration_v1_validating_webhook_configuration_list**](#watch_admissionregistration_v1_validating_webhook_configuration_list) | **get** /apis/admissionregistration.k8s.io/v1/watch/validatingwebhookconfigurations | 

# **create_admissionregistration_v1_mutating_webhook_configuration**
<a name="create_admissionregistration_v1_mutating_webhook_configuration"></a>
> IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration create_admissionregistration_v1_mutating_webhook_configuration(body)



create a MutatingWebhookConfiguration

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_api_admissionregistration_v1_mutating_webhook_configuration import IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only required values which don't have defaults set
    query_params = {
    }
    body = IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration(
        api_version="api_version_example",
        kind="kind_example",
        metadata=IoK8sApimachineryPkgApisMetaV1ObjectMeta(
            annotations=dict(
                "key": "key_example",
            ),
            creation_timestamp="1970-01-01T00:00:00.00Z",
            deletion_grace_period_seconds=1,
            deletion_timestamp="1970-01-01T00:00:00.00Z",
            finalizers=[
                "finalizers_example"
            ],
            generate_name="generate_name_example",
            generation=1,
            labels=dict(
                "key": "key_example",
            ),
            managed_fields=[
                IoK8sApimachineryPkgApisMetaV1ManagedFieldsEntry(
                    api_version="api_version_example",
                    fields_type="fields_type_example",
                    fields_v1=dict(),
                    manager="manager_example",
                    operation="operation_example",
                    subresource="subresource_example",
                    time="1970-01-01T00:00:00.00Z",
                )
            ],
            name="name_example",
            namespace="namespace_example",
            owner_references=[
                IoK8sApimachineryPkgApisMetaV1OwnerReference(
                    api_version="api_version_example",
                    block_owner_deletion=True,
                    controller=True,
                    kind="kind_example",
                    name="name_example",
                    uid="uid_example",
                )
            ],
            resource_version="resource_version_example",
            self_link="self_link_example",
            uid="uid_example",
        ),
        webhooks=[
            IoK8sApiAdmissionregistrationV1MutatingWebhook(
                admission_review_versions=[
                    "admission_review_versions_example"
                ],
                client_config=IoK8sApiAdmissionregistrationV1WebhookClientConfig(
                    ca_bundle='YQ==',
                    service=IoK8sApiAdmissionregistrationV1ServiceReference(
                        name="name_example",
                        namespace="namespace_example",
                        path="path_example",
                        port=1,
                    ),
                    url="url_example",
                ),
                failure_policy="failure_policy_example",
                match_policy="match_policy_example",
                name="name_example",
                namespace_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(
                    match_expressions=[
                        IoK8sApimachineryPkgApisMetaV1LabelSelectorRequirement(
                            key="key_example",
                            operator="operator_example",
                            values=[
                                "values_example"
                            ],
                        )
                    ],
                    match_labels=dict(
                        "key": "key_example",
                    ),
                ),
                object_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(),
                reinvocation_policy="reinvocation_policy_example",
                rules=[
                    IoK8sApiAdmissionregistrationV1RuleWithOperations(
                        api_groups=[
                            "api_groups_example"
                        ],
                        api_versions=[
                            "api_versions_example"
                        ],
                        operations=[
                            "operations_example"
                        ],
                        resources=[
                            "resources_example"
                        ],
                        scope="scope_example",
                    )
                ],
                side_effects="side_effects_example",
                timeout_seconds=1,
            )
        ],
    )
    try:
        api_response = api_instance.create_admissionregistration_v1_mutating_webhook_configuration(
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->create_admissionregistration_v1_mutating_webhook_configuration: %s\n" % e)

    # example passing only optional values
    query_params = {
        'pretty': "pretty_example",
        'dryRun': "dryRun_example",
        'fieldManager': "fieldManager_example",
        'fieldValidation': "fieldValidation_example",
    }
    body = IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration(
        api_version="api_version_example",
        kind="kind_example",
        metadata=IoK8sApimachineryPkgApisMetaV1ObjectMeta(
            annotations=dict(
                "key": "key_example",
            ),
            creation_timestamp="1970-01-01T00:00:00.00Z",
            deletion_grace_period_seconds=1,
            deletion_timestamp="1970-01-01T00:00:00.00Z",
            finalizers=[
                "finalizers_example"
            ],
            generate_name="generate_name_example",
            generation=1,
            labels=dict(
                "key": "key_example",
            ),
            managed_fields=[
                IoK8sApimachineryPkgApisMetaV1ManagedFieldsEntry(
                    api_version="api_version_example",
                    fields_type="fields_type_example",
                    fields_v1=dict(),
                    manager="manager_example",
                    operation="operation_example",
                    subresource="subresource_example",
                    time="1970-01-01T00:00:00.00Z",
                )
            ],
            name="name_example",
            namespace="namespace_example",
            owner_references=[
                IoK8sApimachineryPkgApisMetaV1OwnerReference(
                    api_version="api_version_example",
                    block_owner_deletion=True,
                    controller=True,
                    kind="kind_example",
                    name="name_example",
                    uid="uid_example",
                )
            ],
            resource_version="resource_version_example",
            self_link="self_link_example",
            uid="uid_example",
        ),
        webhooks=[
            IoK8sApiAdmissionregistrationV1MutatingWebhook(
                admission_review_versions=[
                    "admission_review_versions_example"
                ],
                client_config=IoK8sApiAdmissionregistrationV1WebhookClientConfig(
                    ca_bundle='YQ==',
                    service=IoK8sApiAdmissionregistrationV1ServiceReference(
                        name="name_example",
                        namespace="namespace_example",
                        path="path_example",
                        port=1,
                    ),
                    url="url_example",
                ),
                failure_policy="failure_policy_example",
                match_policy="match_policy_example",
                name="name_example",
                namespace_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(
                    match_expressions=[
                        IoK8sApimachineryPkgApisMetaV1LabelSelectorRequirement(
                            key="key_example",
                            operator="operator_example",
                            values=[
                                "values_example"
                            ],
                        )
                    ],
                    match_labels=dict(
                        "key": "key_example",
                    ),
                ),
                object_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(),
                reinvocation_policy="reinvocation_policy_example",
                rules=[
                    IoK8sApiAdmissionregistrationV1RuleWithOperations(
                        api_groups=[
                            "api_groups_example"
                        ],
                        api_versions=[
                            "api_versions_example"
                        ],
                        operations=[
                            "operations_example"
                        ],
                        resources=[
                            "resources_example"
                        ],
                        scope="scope_example",
                    )
                ],
                side_effects="side_effects_example",
                timeout_seconds=1,
            )
        ],
    )
    try:
        api_response = api_instance.create_admissionregistration_v1_mutating_webhook_configuration(
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->create_admissionregistration_v1_mutating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
body | typing.Union[SchemaForRequestBody] | required |
query_params | RequestQueryParams | |
content_type | str | optional, default is '*/*' | Selects the schema and serialization of the request body
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### body

# SchemaForRequestBody
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
pretty | PrettySchema | | optional
dryRun | DryRunSchema | | optional
fieldManager | FieldManagerSchema | | optional
fieldValidation | FieldValidationSchema | | optional


# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# DryRunSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldManagerSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldValidationSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#create_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor200) | OK
201 | [ApiResponseFor201](#create_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor201) | Created
202 | [ApiResponseFor202](#create_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor202) | Accepted
401 | [ApiResponseFor401](#create_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### create_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


#### create_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor201
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor201ResponseBodyApplicationJson, SchemaFor201ResponseBodyApplicationYaml, SchemaFor201ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor201ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor201ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor201ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


#### create_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor202
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor202ResponseBodyApplicationJson, SchemaFor202ResponseBodyApplicationYaml, SchemaFor202ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor202ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor202ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor202ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


#### create_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **create_admissionregistration_v1_validating_webhook_configuration**
<a name="create_admissionregistration_v1_validating_webhook_configuration"></a>
> IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration create_admissionregistration_v1_validating_webhook_configuration(body)



create a ValidatingWebhookConfiguration

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_api_admissionregistration_v1_validating_webhook_configuration import IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only required values which don't have defaults set
    query_params = {
    }
    body = IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration(
        api_version="api_version_example",
        kind="kind_example",
        metadata=IoK8sApimachineryPkgApisMetaV1ObjectMeta(
            annotations=dict(
                "key": "key_example",
            ),
            creation_timestamp="1970-01-01T00:00:00.00Z",
            deletion_grace_period_seconds=1,
            deletion_timestamp="1970-01-01T00:00:00.00Z",
            finalizers=[
                "finalizers_example"
            ],
            generate_name="generate_name_example",
            generation=1,
            labels=dict(
                "key": "key_example",
            ),
            managed_fields=[
                IoK8sApimachineryPkgApisMetaV1ManagedFieldsEntry(
                    api_version="api_version_example",
                    fields_type="fields_type_example",
                    fields_v1=dict(),
                    manager="manager_example",
                    operation="operation_example",
                    subresource="subresource_example",
                    time="1970-01-01T00:00:00.00Z",
                )
            ],
            name="name_example",
            namespace="namespace_example",
            owner_references=[
                IoK8sApimachineryPkgApisMetaV1OwnerReference(
                    api_version="api_version_example",
                    block_owner_deletion=True,
                    controller=True,
                    kind="kind_example",
                    name="name_example",
                    uid="uid_example",
                )
            ],
            resource_version="resource_version_example",
            self_link="self_link_example",
            uid="uid_example",
        ),
        webhooks=[
            IoK8sApiAdmissionregistrationV1ValidatingWebhook(
                admission_review_versions=[
                    "admission_review_versions_example"
                ],
                client_config=IoK8sApiAdmissionregistrationV1WebhookClientConfig(
                    ca_bundle='YQ==',
                    service=IoK8sApiAdmissionregistrationV1ServiceReference(
                        name="name_example",
                        namespace="namespace_example",
                        path="path_example",
                        port=1,
                    ),
                    url="url_example",
                ),
                failure_policy="failure_policy_example",
                match_policy="match_policy_example",
                name="name_example",
                namespace_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(
                    match_expressions=[
                        IoK8sApimachineryPkgApisMetaV1LabelSelectorRequirement(
                            key="key_example",
                            operator="operator_example",
                            values=[
                                "values_example"
                            ],
                        )
                    ],
                    match_labels=dict(
                        "key": "key_example",
                    ),
                ),
                object_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(),
                rules=[
                    IoK8sApiAdmissionregistrationV1RuleWithOperations(
                        api_groups=[
                            "api_groups_example"
                        ],
                        api_versions=[
                            "api_versions_example"
                        ],
                        operations=[
                            "operations_example"
                        ],
                        resources=[
                            "resources_example"
                        ],
                        scope="scope_example",
                    )
                ],
                side_effects="side_effects_example",
                timeout_seconds=1,
            )
        ],
    )
    try:
        api_response = api_instance.create_admissionregistration_v1_validating_webhook_configuration(
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->create_admissionregistration_v1_validating_webhook_configuration: %s\n" % e)

    # example passing only optional values
    query_params = {
        'pretty': "pretty_example",
        'dryRun': "dryRun_example",
        'fieldManager': "fieldManager_example",
        'fieldValidation': "fieldValidation_example",
    }
    body = IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration(
        api_version="api_version_example",
        kind="kind_example",
        metadata=IoK8sApimachineryPkgApisMetaV1ObjectMeta(
            annotations=dict(
                "key": "key_example",
            ),
            creation_timestamp="1970-01-01T00:00:00.00Z",
            deletion_grace_period_seconds=1,
            deletion_timestamp="1970-01-01T00:00:00.00Z",
            finalizers=[
                "finalizers_example"
            ],
            generate_name="generate_name_example",
            generation=1,
            labels=dict(
                "key": "key_example",
            ),
            managed_fields=[
                IoK8sApimachineryPkgApisMetaV1ManagedFieldsEntry(
                    api_version="api_version_example",
                    fields_type="fields_type_example",
                    fields_v1=dict(),
                    manager="manager_example",
                    operation="operation_example",
                    subresource="subresource_example",
                    time="1970-01-01T00:00:00.00Z",
                )
            ],
            name="name_example",
            namespace="namespace_example",
            owner_references=[
                IoK8sApimachineryPkgApisMetaV1OwnerReference(
                    api_version="api_version_example",
                    block_owner_deletion=True,
                    controller=True,
                    kind="kind_example",
                    name="name_example",
                    uid="uid_example",
                )
            ],
            resource_version="resource_version_example",
            self_link="self_link_example",
            uid="uid_example",
        ),
        webhooks=[
            IoK8sApiAdmissionregistrationV1ValidatingWebhook(
                admission_review_versions=[
                    "admission_review_versions_example"
                ],
                client_config=IoK8sApiAdmissionregistrationV1WebhookClientConfig(
                    ca_bundle='YQ==',
                    service=IoK8sApiAdmissionregistrationV1ServiceReference(
                        name="name_example",
                        namespace="namespace_example",
                        path="path_example",
                        port=1,
                    ),
                    url="url_example",
                ),
                failure_policy="failure_policy_example",
                match_policy="match_policy_example",
                name="name_example",
                namespace_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(
                    match_expressions=[
                        IoK8sApimachineryPkgApisMetaV1LabelSelectorRequirement(
                            key="key_example",
                            operator="operator_example",
                            values=[
                                "values_example"
                            ],
                        )
                    ],
                    match_labels=dict(
                        "key": "key_example",
                    ),
                ),
                object_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(),
                rules=[
                    IoK8sApiAdmissionregistrationV1RuleWithOperations(
                        api_groups=[
                            "api_groups_example"
                        ],
                        api_versions=[
                            "api_versions_example"
                        ],
                        operations=[
                            "operations_example"
                        ],
                        resources=[
                            "resources_example"
                        ],
                        scope="scope_example",
                    )
                ],
                side_effects="side_effects_example",
                timeout_seconds=1,
            )
        ],
    )
    try:
        api_response = api_instance.create_admissionregistration_v1_validating_webhook_configuration(
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->create_admissionregistration_v1_validating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
body | typing.Union[SchemaForRequestBody] | required |
query_params | RequestQueryParams | |
content_type | str | optional, default is '*/*' | Selects the schema and serialization of the request body
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### body

# SchemaForRequestBody
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
pretty | PrettySchema | | optional
dryRun | DryRunSchema | | optional
fieldManager | FieldManagerSchema | | optional
fieldValidation | FieldValidationSchema | | optional


# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# DryRunSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldManagerSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldValidationSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#create_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor200) | OK
201 | [ApiResponseFor201](#create_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor201) | Created
202 | [ApiResponseFor202](#create_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor202) | Accepted
401 | [ApiResponseFor401](#create_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### create_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


#### create_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor201
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor201ResponseBodyApplicationJson, SchemaFor201ResponseBodyApplicationYaml, SchemaFor201ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor201ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor201ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor201ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


#### create_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor202
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor202ResponseBodyApplicationJson, SchemaFor202ResponseBodyApplicationYaml, SchemaFor202ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor202ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor202ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor202ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


#### create_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **delete_admissionregistration_v1_collection_mutating_webhook_configuration**
<a name="delete_admissionregistration_v1_collection_mutating_webhook_configuration"></a>
> IoK8sApimachineryPkgApisMetaV1Status delete_admissionregistration_v1_collection_mutating_webhook_configuration()



delete collection of MutatingWebhookConfiguration

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_apimachinery_pkg_apis_meta_v1_delete_options import IoK8sApimachineryPkgApisMetaV1DeleteOptions
from openapi_client.model.io_k8s_apimachinery_pkg_apis_meta_v1_status import IoK8sApimachineryPkgApisMetaV1Status
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only optional values
    query_params = {
        'pretty': "pretty_example",
        'continue': "continue_example",
        'dryRun': "dryRun_example",
        'fieldSelector': "fieldSelector_example",
        'gracePeriodSeconds': 1,
        'labelSelector': "labelSelector_example",
        'limit': 1,
        'orphanDependents': True,
        'propagationPolicy': "propagationPolicy_example",
        'resourceVersion': "resourceVersion_example",
        'resourceVersionMatch': "resourceVersionMatch_example",
        'timeoutSeconds': 1,
    }
    body = IoK8sApimachineryPkgApisMetaV1DeleteOptions(
        api_version="api_version_example",
        dry_run=[
            "dry_run_example"
        ],
        grace_period_seconds=1,
        kind="kind_example",
        orphan_dependents=True,
        preconditions=IoK8sApimachineryPkgApisMetaV1Preconditions(
            resource_version="resource_version_example",
            uid="uid_example",
        ),
        propagation_policy="propagation_policy_example",
    )
    try:
        api_response = api_instance.delete_admissionregistration_v1_collection_mutating_webhook_configuration(
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->delete_admissionregistration_v1_collection_mutating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
body | typing.Union[SchemaForRequestBody, Unset] | optional, default is unset |
query_params | RequestQueryParams | |
content_type | str | optional, default is '*/*' | Selects the schema and serialization of the request body
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### body

# SchemaForRequestBody
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1DeleteOptions**](../../models/IoK8sApimachineryPkgApisMetaV1DeleteOptions.md) |  | 


### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
pretty | PrettySchema | | optional
continue | ModelContinueSchema | | optional
dryRun | DryRunSchema | | optional
fieldSelector | FieldSelectorSchema | | optional
gracePeriodSeconds | GracePeriodSecondsSchema | | optional
labelSelector | LabelSelectorSchema | | optional
limit | LimitSchema | | optional
orphanDependents | OrphanDependentsSchema | | optional
propagationPolicy | PropagationPolicySchema | | optional
resourceVersion | ResourceVersionSchema | | optional
resourceVersionMatch | ResourceVersionMatchSchema | | optional
timeoutSeconds | TimeoutSecondsSchema | | optional


# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ModelContinueSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# DryRunSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# GracePeriodSecondsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# LabelSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# LimitSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# OrphanDependentsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

# PropagationPolicySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ResourceVersionSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ResourceVersionMatchSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# TimeoutSecondsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#delete_admissionregistration_v1_collection_mutating_webhook_configuration.ApiResponseFor200) | OK
401 | [ApiResponseFor401](#delete_admissionregistration_v1_collection_mutating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### delete_admissionregistration_v1_collection_mutating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


#### delete_admissionregistration_v1_collection_mutating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **delete_admissionregistration_v1_collection_validating_webhook_configuration**
<a name="delete_admissionregistration_v1_collection_validating_webhook_configuration"></a>
> IoK8sApimachineryPkgApisMetaV1Status delete_admissionregistration_v1_collection_validating_webhook_configuration()



delete collection of ValidatingWebhookConfiguration

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_apimachinery_pkg_apis_meta_v1_delete_options import IoK8sApimachineryPkgApisMetaV1DeleteOptions
from openapi_client.model.io_k8s_apimachinery_pkg_apis_meta_v1_status import IoK8sApimachineryPkgApisMetaV1Status
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only optional values
    query_params = {
        'pretty': "pretty_example",
        'continue': "continue_example",
        'dryRun': "dryRun_example",
        'fieldSelector': "fieldSelector_example",
        'gracePeriodSeconds': 1,
        'labelSelector': "labelSelector_example",
        'limit': 1,
        'orphanDependents': True,
        'propagationPolicy': "propagationPolicy_example",
        'resourceVersion': "resourceVersion_example",
        'resourceVersionMatch': "resourceVersionMatch_example",
        'timeoutSeconds': 1,
    }
    body = IoK8sApimachineryPkgApisMetaV1DeleteOptions(
        api_version="api_version_example",
        dry_run=[
            "dry_run_example"
        ],
        grace_period_seconds=1,
        kind="kind_example",
        orphan_dependents=True,
        preconditions=IoK8sApimachineryPkgApisMetaV1Preconditions(
            resource_version="resource_version_example",
            uid="uid_example",
        ),
        propagation_policy="propagation_policy_example",
    )
    try:
        api_response = api_instance.delete_admissionregistration_v1_collection_validating_webhook_configuration(
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->delete_admissionregistration_v1_collection_validating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
body | typing.Union[SchemaForRequestBody, Unset] | optional, default is unset |
query_params | RequestQueryParams | |
content_type | str | optional, default is '*/*' | Selects the schema and serialization of the request body
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### body

# SchemaForRequestBody
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1DeleteOptions**](../../models/IoK8sApimachineryPkgApisMetaV1DeleteOptions.md) |  | 


### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
pretty | PrettySchema | | optional
continue | ModelContinueSchema | | optional
dryRun | DryRunSchema | | optional
fieldSelector | FieldSelectorSchema | | optional
gracePeriodSeconds | GracePeriodSecondsSchema | | optional
labelSelector | LabelSelectorSchema | | optional
limit | LimitSchema | | optional
orphanDependents | OrphanDependentsSchema | | optional
propagationPolicy | PropagationPolicySchema | | optional
resourceVersion | ResourceVersionSchema | | optional
resourceVersionMatch | ResourceVersionMatchSchema | | optional
timeoutSeconds | TimeoutSecondsSchema | | optional


# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ModelContinueSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# DryRunSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# GracePeriodSecondsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# LabelSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# LimitSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# OrphanDependentsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

# PropagationPolicySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ResourceVersionSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ResourceVersionMatchSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# TimeoutSecondsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#delete_admissionregistration_v1_collection_validating_webhook_configuration.ApiResponseFor200) | OK
401 | [ApiResponseFor401](#delete_admissionregistration_v1_collection_validating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### delete_admissionregistration_v1_collection_validating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


#### delete_admissionregistration_v1_collection_validating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **delete_admissionregistration_v1_mutating_webhook_configuration**
<a name="delete_admissionregistration_v1_mutating_webhook_configuration"></a>
> IoK8sApimachineryPkgApisMetaV1Status delete_admissionregistration_v1_mutating_webhook_configuration(name)



delete a MutatingWebhookConfiguration

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_apimachinery_pkg_apis_meta_v1_delete_options import IoK8sApimachineryPkgApisMetaV1DeleteOptions
from openapi_client.model.io_k8s_apimachinery_pkg_apis_meta_v1_status import IoK8sApimachineryPkgApisMetaV1Status
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only required values which don't have defaults set
    path_params = {
        'name': "name_example",
    }
    query_params = {
    }
    try:
        api_response = api_instance.delete_admissionregistration_v1_mutating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->delete_admissionregistration_v1_mutating_webhook_configuration: %s\n" % e)

    # example passing only optional values
    path_params = {
        'name': "name_example",
    }
    query_params = {
        'pretty': "pretty_example",
        'dryRun': "dryRun_example",
        'gracePeriodSeconds': 1,
        'orphanDependents': True,
        'propagationPolicy': "propagationPolicy_example",
    }
    body = IoK8sApimachineryPkgApisMetaV1DeleteOptions(
        api_version="api_version_example",
        dry_run=[
            "dry_run_example"
        ],
        grace_period_seconds=1,
        kind="kind_example",
        orphan_dependents=True,
        preconditions=IoK8sApimachineryPkgApisMetaV1Preconditions(
            resource_version="resource_version_example",
            uid="uid_example",
        ),
        propagation_policy="propagation_policy_example",
    )
    try:
        api_response = api_instance.delete_admissionregistration_v1_mutating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->delete_admissionregistration_v1_mutating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
body | typing.Union[SchemaForRequestBody, Unset] | optional, default is unset |
query_params | RequestQueryParams | |
path_params | RequestPathParams | |
content_type | str | optional, default is '*/*' | Selects the schema and serialization of the request body
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### body

# SchemaForRequestBody
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1DeleteOptions**](../../models/IoK8sApimachineryPkgApisMetaV1DeleteOptions.md) |  | 


### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
pretty | PrettySchema | | optional
dryRun | DryRunSchema | | optional
gracePeriodSeconds | GracePeriodSecondsSchema | | optional
orphanDependents | OrphanDependentsSchema | | optional
propagationPolicy | PropagationPolicySchema | | optional


# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# DryRunSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# GracePeriodSecondsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# OrphanDependentsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

# PropagationPolicySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### path_params
#### RequestPathParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
name | NameSchema | | 

# NameSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#delete_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor200) | OK
202 | [ApiResponseFor202](#delete_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor202) | Accepted
401 | [ApiResponseFor401](#delete_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### delete_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


#### delete_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor202
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor202ResponseBodyApplicationJson, SchemaFor202ResponseBodyApplicationYaml, SchemaFor202ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor202ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


# SchemaFor202ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


# SchemaFor202ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


#### delete_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **delete_admissionregistration_v1_validating_webhook_configuration**
<a name="delete_admissionregistration_v1_validating_webhook_configuration"></a>
> IoK8sApimachineryPkgApisMetaV1Status delete_admissionregistration_v1_validating_webhook_configuration(name)



delete a ValidatingWebhookConfiguration

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_apimachinery_pkg_apis_meta_v1_delete_options import IoK8sApimachineryPkgApisMetaV1DeleteOptions
from openapi_client.model.io_k8s_apimachinery_pkg_apis_meta_v1_status import IoK8sApimachineryPkgApisMetaV1Status
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only required values which don't have defaults set
    path_params = {
        'name': "name_example",
    }
    query_params = {
    }
    try:
        api_response = api_instance.delete_admissionregistration_v1_validating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->delete_admissionregistration_v1_validating_webhook_configuration: %s\n" % e)

    # example passing only optional values
    path_params = {
        'name': "name_example",
    }
    query_params = {
        'pretty': "pretty_example",
        'dryRun': "dryRun_example",
        'gracePeriodSeconds': 1,
        'orphanDependents': True,
        'propagationPolicy': "propagationPolicy_example",
    }
    body = IoK8sApimachineryPkgApisMetaV1DeleteOptions(
        api_version="api_version_example",
        dry_run=[
            "dry_run_example"
        ],
        grace_period_seconds=1,
        kind="kind_example",
        orphan_dependents=True,
        preconditions=IoK8sApimachineryPkgApisMetaV1Preconditions(
            resource_version="resource_version_example",
            uid="uid_example",
        ),
        propagation_policy="propagation_policy_example",
    )
    try:
        api_response = api_instance.delete_admissionregistration_v1_validating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->delete_admissionregistration_v1_validating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
body | typing.Union[SchemaForRequestBody, Unset] | optional, default is unset |
query_params | RequestQueryParams | |
path_params | RequestPathParams | |
content_type | str | optional, default is '*/*' | Selects the schema and serialization of the request body
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### body

# SchemaForRequestBody
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1DeleteOptions**](../../models/IoK8sApimachineryPkgApisMetaV1DeleteOptions.md) |  | 


### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
pretty | PrettySchema | | optional
dryRun | DryRunSchema | | optional
gracePeriodSeconds | GracePeriodSecondsSchema | | optional
orphanDependents | OrphanDependentsSchema | | optional
propagationPolicy | PropagationPolicySchema | | optional


# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# DryRunSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# GracePeriodSecondsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# OrphanDependentsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

# PropagationPolicySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### path_params
#### RequestPathParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
name | NameSchema | | 

# NameSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#delete_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor200) | OK
202 | [ApiResponseFor202](#delete_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor202) | Accepted
401 | [ApiResponseFor401](#delete_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### delete_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


#### delete_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor202
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor202ResponseBodyApplicationJson, SchemaFor202ResponseBodyApplicationYaml, SchemaFor202ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor202ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


# SchemaFor202ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


# SchemaFor202ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1Status**](../../models/IoK8sApimachineryPkgApisMetaV1Status.md) |  | 


#### delete_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **get_admissionregistration_v1_api_resources**
<a name="get_admissionregistration_v1_api_resources"></a>
> IoK8sApimachineryPkgApisMetaV1APIResourceList get_admissionregistration_v1_api_resources()



get available resources

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_apimachinery_pkg_apis_meta_v1_api_resource_list import IoK8sApimachineryPkgApisMetaV1APIResourceList
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example, this endpoint has no required or optional parameters
    try:
        api_response = api_instance.get_admissionregistration_v1_api_resources()
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->get_admissionregistration_v1_api_resources: %s\n" % e)
```
### Parameters
This endpoint does not need any parameter.

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#get_admissionregistration_v1_api_resources.ApiResponseFor200) | OK
401 | [ApiResponseFor401](#get_admissionregistration_v1_api_resources.ApiResponseFor401) | Unauthorized

#### get_admissionregistration_v1_api_resources.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1APIResourceList**](../../models/IoK8sApimachineryPkgApisMetaV1APIResourceList.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1APIResourceList**](../../models/IoK8sApimachineryPkgApisMetaV1APIResourceList.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1APIResourceList**](../../models/IoK8sApimachineryPkgApisMetaV1APIResourceList.md) |  | 


#### get_admissionregistration_v1_api_resources.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **list_admissionregistration_v1_mutating_webhook_configuration**
<a name="list_admissionregistration_v1_mutating_webhook_configuration"></a>
> IoK8sApiAdmissionregistrationV1MutatingWebhookConfigurationList list_admissionregistration_v1_mutating_webhook_configuration()



list or watch objects of kind MutatingWebhookConfiguration

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_api_admissionregistration_v1_mutating_webhook_configuration_list import IoK8sApiAdmissionregistrationV1MutatingWebhookConfigurationList
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only optional values
    query_params = {
        'pretty': "pretty_example",
        'allowWatchBookmarks': True,
        'continue': "continue_example",
        'fieldSelector': "fieldSelector_example",
        'labelSelector': "labelSelector_example",
        'limit': 1,
        'resourceVersion': "resourceVersion_example",
        'resourceVersionMatch': "resourceVersionMatch_example",
        'timeoutSeconds': 1,
        'watch': True,
    }
    try:
        api_response = api_instance.list_admissionregistration_v1_mutating_webhook_configuration(
            query_params=query_params,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->list_admissionregistration_v1_mutating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
query_params | RequestQueryParams | |
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', 'application/json;stream&#x3D;watch', 'application/vnd.kubernetes.protobuf;stream&#x3D;watch', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
pretty | PrettySchema | | optional
allowWatchBookmarks | AllowWatchBookmarksSchema | | optional
continue | ModelContinueSchema | | optional
fieldSelector | FieldSelectorSchema | | optional
labelSelector | LabelSelectorSchema | | optional
limit | LimitSchema | | optional
resourceVersion | ResourceVersionSchema | | optional
resourceVersionMatch | ResourceVersionMatchSchema | | optional
timeoutSeconds | TimeoutSecondsSchema | | optional
watch | WatchSchema | | optional


# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# AllowWatchBookmarksSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

# ModelContinueSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# LabelSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# LimitSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# ResourceVersionSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ResourceVersionMatchSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# TimeoutSecondsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# WatchSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#list_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor200) | OK
401 | [ApiResponseFor401](#list_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### list_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, SchemaFor200ResponseBodyApplicationJsonstreamwatch, SchemaFor200ResponseBodyApplicationVndKubernetesProtobufstreamwatch, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfigurationList**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfigurationList.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfigurationList**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfigurationList.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfigurationList**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfigurationList.md) |  | 


# SchemaFor200ResponseBodyApplicationJsonstreamwatch
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfigurationList**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfigurationList.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobufstreamwatch
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfigurationList**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfigurationList.md) |  | 


#### list_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **list_admissionregistration_v1_validating_webhook_configuration**
<a name="list_admissionregistration_v1_validating_webhook_configuration"></a>
> IoK8sApiAdmissionregistrationV1ValidatingWebhookConfigurationList list_admissionregistration_v1_validating_webhook_configuration()



list or watch objects of kind ValidatingWebhookConfiguration

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_api_admissionregistration_v1_validating_webhook_configuration_list import IoK8sApiAdmissionregistrationV1ValidatingWebhookConfigurationList
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only optional values
    query_params = {
        'pretty': "pretty_example",
        'allowWatchBookmarks': True,
        'continue': "continue_example",
        'fieldSelector': "fieldSelector_example",
        'labelSelector': "labelSelector_example",
        'limit': 1,
        'resourceVersion': "resourceVersion_example",
        'resourceVersionMatch': "resourceVersionMatch_example",
        'timeoutSeconds': 1,
        'watch': True,
    }
    try:
        api_response = api_instance.list_admissionregistration_v1_validating_webhook_configuration(
            query_params=query_params,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->list_admissionregistration_v1_validating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
query_params | RequestQueryParams | |
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', 'application/json;stream&#x3D;watch', 'application/vnd.kubernetes.protobuf;stream&#x3D;watch', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
pretty | PrettySchema | | optional
allowWatchBookmarks | AllowWatchBookmarksSchema | | optional
continue | ModelContinueSchema | | optional
fieldSelector | FieldSelectorSchema | | optional
labelSelector | LabelSelectorSchema | | optional
limit | LimitSchema | | optional
resourceVersion | ResourceVersionSchema | | optional
resourceVersionMatch | ResourceVersionMatchSchema | | optional
timeoutSeconds | TimeoutSecondsSchema | | optional
watch | WatchSchema | | optional


# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# AllowWatchBookmarksSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

# ModelContinueSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# LabelSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# LimitSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# ResourceVersionSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ResourceVersionMatchSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# TimeoutSecondsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# WatchSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#list_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor200) | OK
401 | [ApiResponseFor401](#list_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### list_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, SchemaFor200ResponseBodyApplicationJsonstreamwatch, SchemaFor200ResponseBodyApplicationVndKubernetesProtobufstreamwatch, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfigurationList**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfigurationList.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfigurationList**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfigurationList.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfigurationList**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfigurationList.md) |  | 


# SchemaFor200ResponseBodyApplicationJsonstreamwatch
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfigurationList**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfigurationList.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobufstreamwatch
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfigurationList**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfigurationList.md) |  | 


#### list_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **patch_admissionregistration_v1_mutating_webhook_configuration**
<a name="patch_admissionregistration_v1_mutating_webhook_configuration"></a>
> IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration patch_admissionregistration_v1_mutating_webhook_configuration(namebody)



partially update the specified MutatingWebhookConfiguration

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_api_admissionregistration_v1_mutating_webhook_configuration import IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only required values which don't have defaults set
    path_params = {
        'name': "name_example",
    }
    query_params = {
    }
    body = dict()
    try:
        api_response = api_instance.patch_admissionregistration_v1_mutating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->patch_admissionregistration_v1_mutating_webhook_configuration: %s\n" % e)

    # example passing only optional values
    path_params = {
        'name': "name_example",
    }
    query_params = {
        'pretty': "pretty_example",
        'dryRun': "dryRun_example",
        'fieldManager': "fieldManager_example",
        'fieldValidation': "fieldValidation_example",
        'force': True,
    }
    body = dict()
    try:
        api_response = api_instance.patch_admissionregistration_v1_mutating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->patch_admissionregistration_v1_mutating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
body | typing.Union[SchemaForRequestBodyApplicationJsonPatchjson, SchemaForRequestBodyApplicationMergePatchjson, SchemaForRequestBodyApplicationStrategicMergePatchjson, SchemaForRequestBodyApplicationApplyPatchyaml] | required |
query_params | RequestQueryParams | |
path_params | RequestPathParams | |
content_type | str | optional, default is 'application/json-patch+json' | Selects the schema and serialization of the request body
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### body

# SchemaForRequestBodyApplicationJsonPatchjson

Patch is provided to give a concrete name and type to the Kubernetes PATCH request body.

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
dict, frozendict.frozendict,  | frozendict.frozendict,  | Patch is provided to give a concrete name and type to the Kubernetes PATCH request body. | 

# SchemaForRequestBodyApplicationMergePatchjson

Patch is provided to give a concrete name and type to the Kubernetes PATCH request body.

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
dict, frozendict.frozendict,  | frozendict.frozendict,  | Patch is provided to give a concrete name and type to the Kubernetes PATCH request body. | 

# SchemaForRequestBodyApplicationStrategicMergePatchjson

Patch is provided to give a concrete name and type to the Kubernetes PATCH request body.

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
dict, frozendict.frozendict,  | frozendict.frozendict,  | Patch is provided to give a concrete name and type to the Kubernetes PATCH request body. | 

# SchemaForRequestBodyApplicationApplyPatchyaml

Patch is provided to give a concrete name and type to the Kubernetes PATCH request body.

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
dict, frozendict.frozendict,  | frozendict.frozendict,  | Patch is provided to give a concrete name and type to the Kubernetes PATCH request body. | 

### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
pretty | PrettySchema | | optional
dryRun | DryRunSchema | | optional
fieldManager | FieldManagerSchema | | optional
fieldValidation | FieldValidationSchema | | optional
force | ForceSchema | | optional


# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# DryRunSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldManagerSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldValidationSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ForceSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

### path_params
#### RequestPathParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
name | NameSchema | | 

# NameSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#patch_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor200) | OK
201 | [ApiResponseFor201](#patch_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor201) | Created
401 | [ApiResponseFor401](#patch_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### patch_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


#### patch_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor201
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor201ResponseBodyApplicationJson, SchemaFor201ResponseBodyApplicationYaml, SchemaFor201ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor201ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor201ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor201ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


#### patch_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **patch_admissionregistration_v1_validating_webhook_configuration**
<a name="patch_admissionregistration_v1_validating_webhook_configuration"></a>
> IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration patch_admissionregistration_v1_validating_webhook_configuration(namebody)



partially update the specified ValidatingWebhookConfiguration

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_api_admissionregistration_v1_validating_webhook_configuration import IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only required values which don't have defaults set
    path_params = {
        'name': "name_example",
    }
    query_params = {
    }
    body = dict()
    try:
        api_response = api_instance.patch_admissionregistration_v1_validating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->patch_admissionregistration_v1_validating_webhook_configuration: %s\n" % e)

    # example passing only optional values
    path_params = {
        'name': "name_example",
    }
    query_params = {
        'pretty': "pretty_example",
        'dryRun': "dryRun_example",
        'fieldManager': "fieldManager_example",
        'fieldValidation': "fieldValidation_example",
        'force': True,
    }
    body = dict()
    try:
        api_response = api_instance.patch_admissionregistration_v1_validating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->patch_admissionregistration_v1_validating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
body | typing.Union[SchemaForRequestBodyApplicationJsonPatchjson, SchemaForRequestBodyApplicationMergePatchjson, SchemaForRequestBodyApplicationStrategicMergePatchjson, SchemaForRequestBodyApplicationApplyPatchyaml] | required |
query_params | RequestQueryParams | |
path_params | RequestPathParams | |
content_type | str | optional, default is 'application/json-patch+json' | Selects the schema and serialization of the request body
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### body

# SchemaForRequestBodyApplicationJsonPatchjson

Patch is provided to give a concrete name and type to the Kubernetes PATCH request body.

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
dict, frozendict.frozendict,  | frozendict.frozendict,  | Patch is provided to give a concrete name and type to the Kubernetes PATCH request body. | 

# SchemaForRequestBodyApplicationMergePatchjson

Patch is provided to give a concrete name and type to the Kubernetes PATCH request body.

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
dict, frozendict.frozendict,  | frozendict.frozendict,  | Patch is provided to give a concrete name and type to the Kubernetes PATCH request body. | 

# SchemaForRequestBodyApplicationStrategicMergePatchjson

Patch is provided to give a concrete name and type to the Kubernetes PATCH request body.

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
dict, frozendict.frozendict,  | frozendict.frozendict,  | Patch is provided to give a concrete name and type to the Kubernetes PATCH request body. | 

# SchemaForRequestBodyApplicationApplyPatchyaml

Patch is provided to give a concrete name and type to the Kubernetes PATCH request body.

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
dict, frozendict.frozendict,  | frozendict.frozendict,  | Patch is provided to give a concrete name and type to the Kubernetes PATCH request body. | 

### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
pretty | PrettySchema | | optional
dryRun | DryRunSchema | | optional
fieldManager | FieldManagerSchema | | optional
fieldValidation | FieldValidationSchema | | optional
force | ForceSchema | | optional


# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# DryRunSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldManagerSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldValidationSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ForceSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

### path_params
#### RequestPathParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
name | NameSchema | | 

# NameSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#patch_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor200) | OK
201 | [ApiResponseFor201](#patch_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor201) | Created
401 | [ApiResponseFor401](#patch_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### patch_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


#### patch_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor201
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor201ResponseBodyApplicationJson, SchemaFor201ResponseBodyApplicationYaml, SchemaFor201ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor201ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor201ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor201ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


#### patch_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **read_admissionregistration_v1_mutating_webhook_configuration**
<a name="read_admissionregistration_v1_mutating_webhook_configuration"></a>
> IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration read_admissionregistration_v1_mutating_webhook_configuration(name)



read the specified MutatingWebhookConfiguration

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_api_admissionregistration_v1_mutating_webhook_configuration import IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only required values which don't have defaults set
    path_params = {
        'name': "name_example",
    }
    query_params = {
    }
    try:
        api_response = api_instance.read_admissionregistration_v1_mutating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->read_admissionregistration_v1_mutating_webhook_configuration: %s\n" % e)

    # example passing only optional values
    path_params = {
        'name': "name_example",
    }
    query_params = {
        'pretty': "pretty_example",
    }
    try:
        api_response = api_instance.read_admissionregistration_v1_mutating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->read_admissionregistration_v1_mutating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
query_params | RequestQueryParams | |
path_params | RequestPathParams | |
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
pretty | PrettySchema | | optional


# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### path_params
#### RequestPathParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
name | NameSchema | | 

# NameSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#read_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor200) | OK
401 | [ApiResponseFor401](#read_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### read_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


#### read_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **read_admissionregistration_v1_validating_webhook_configuration**
<a name="read_admissionregistration_v1_validating_webhook_configuration"></a>
> IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration read_admissionregistration_v1_validating_webhook_configuration(name)



read the specified ValidatingWebhookConfiguration

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_api_admissionregistration_v1_validating_webhook_configuration import IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only required values which don't have defaults set
    path_params = {
        'name': "name_example",
    }
    query_params = {
    }
    try:
        api_response = api_instance.read_admissionregistration_v1_validating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->read_admissionregistration_v1_validating_webhook_configuration: %s\n" % e)

    # example passing only optional values
    path_params = {
        'name': "name_example",
    }
    query_params = {
        'pretty': "pretty_example",
    }
    try:
        api_response = api_instance.read_admissionregistration_v1_validating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->read_admissionregistration_v1_validating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
query_params | RequestQueryParams | |
path_params | RequestPathParams | |
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
pretty | PrettySchema | | optional


# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### path_params
#### RequestPathParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
name | NameSchema | | 

# NameSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#read_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor200) | OK
401 | [ApiResponseFor401](#read_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### read_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


#### read_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **replace_admissionregistration_v1_mutating_webhook_configuration**
<a name="replace_admissionregistration_v1_mutating_webhook_configuration"></a>
> IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration replace_admissionregistration_v1_mutating_webhook_configuration(namebody)



replace the specified MutatingWebhookConfiguration

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_api_admissionregistration_v1_mutating_webhook_configuration import IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only required values which don't have defaults set
    path_params = {
        'name': "name_example",
    }
    query_params = {
    }
    body = IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration(
        api_version="api_version_example",
        kind="kind_example",
        metadata=IoK8sApimachineryPkgApisMetaV1ObjectMeta(
            annotations=dict(
                "key": "key_example",
            ),
            creation_timestamp="1970-01-01T00:00:00.00Z",
            deletion_grace_period_seconds=1,
            deletion_timestamp="1970-01-01T00:00:00.00Z",
            finalizers=[
                "finalizers_example"
            ],
            generate_name="generate_name_example",
            generation=1,
            labels=dict(
                "key": "key_example",
            ),
            managed_fields=[
                IoK8sApimachineryPkgApisMetaV1ManagedFieldsEntry(
                    api_version="api_version_example",
                    fields_type="fields_type_example",
                    fields_v1=dict(),
                    manager="manager_example",
                    operation="operation_example",
                    subresource="subresource_example",
                    time="1970-01-01T00:00:00.00Z",
                )
            ],
            name="name_example",
            namespace="namespace_example",
            owner_references=[
                IoK8sApimachineryPkgApisMetaV1OwnerReference(
                    api_version="api_version_example",
                    block_owner_deletion=True,
                    controller=True,
                    kind="kind_example",
                    name="name_example",
                    uid="uid_example",
                )
            ],
            resource_version="resource_version_example",
            self_link="self_link_example",
            uid="uid_example",
        ),
        webhooks=[
            IoK8sApiAdmissionregistrationV1MutatingWebhook(
                admission_review_versions=[
                    "admission_review_versions_example"
                ],
                client_config=IoK8sApiAdmissionregistrationV1WebhookClientConfig(
                    ca_bundle='YQ==',
                    service=IoK8sApiAdmissionregistrationV1ServiceReference(
                        name="name_example",
                        namespace="namespace_example",
                        path="path_example",
                        port=1,
                    ),
                    url="url_example",
                ),
                failure_policy="failure_policy_example",
                match_policy="match_policy_example",
                name="name_example",
                namespace_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(
                    match_expressions=[
                        IoK8sApimachineryPkgApisMetaV1LabelSelectorRequirement(
                            key="key_example",
                            operator="operator_example",
                            values=[
                                "values_example"
                            ],
                        )
                    ],
                    match_labels=dict(
                        "key": "key_example",
                    ),
                ),
                object_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(),
                reinvocation_policy="reinvocation_policy_example",
                rules=[
                    IoK8sApiAdmissionregistrationV1RuleWithOperations(
                        api_groups=[
                            "api_groups_example"
                        ],
                        api_versions=[
                            "api_versions_example"
                        ],
                        operations=[
                            "operations_example"
                        ],
                        resources=[
                            "resources_example"
                        ],
                        scope="scope_example",
                    )
                ],
                side_effects="side_effects_example",
                timeout_seconds=1,
            )
        ],
    )
    try:
        api_response = api_instance.replace_admissionregistration_v1_mutating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->replace_admissionregistration_v1_mutating_webhook_configuration: %s\n" % e)

    # example passing only optional values
    path_params = {
        'name': "name_example",
    }
    query_params = {
        'pretty': "pretty_example",
        'dryRun': "dryRun_example",
        'fieldManager': "fieldManager_example",
        'fieldValidation': "fieldValidation_example",
    }
    body = IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration(
        api_version="api_version_example",
        kind="kind_example",
        metadata=IoK8sApimachineryPkgApisMetaV1ObjectMeta(
            annotations=dict(
                "key": "key_example",
            ),
            creation_timestamp="1970-01-01T00:00:00.00Z",
            deletion_grace_period_seconds=1,
            deletion_timestamp="1970-01-01T00:00:00.00Z",
            finalizers=[
                "finalizers_example"
            ],
            generate_name="generate_name_example",
            generation=1,
            labels=dict(
                "key": "key_example",
            ),
            managed_fields=[
                IoK8sApimachineryPkgApisMetaV1ManagedFieldsEntry(
                    api_version="api_version_example",
                    fields_type="fields_type_example",
                    fields_v1=dict(),
                    manager="manager_example",
                    operation="operation_example",
                    subresource="subresource_example",
                    time="1970-01-01T00:00:00.00Z",
                )
            ],
            name="name_example",
            namespace="namespace_example",
            owner_references=[
                IoK8sApimachineryPkgApisMetaV1OwnerReference(
                    api_version="api_version_example",
                    block_owner_deletion=True,
                    controller=True,
                    kind="kind_example",
                    name="name_example",
                    uid="uid_example",
                )
            ],
            resource_version="resource_version_example",
            self_link="self_link_example",
            uid="uid_example",
        ),
        webhooks=[
            IoK8sApiAdmissionregistrationV1MutatingWebhook(
                admission_review_versions=[
                    "admission_review_versions_example"
                ],
                client_config=IoK8sApiAdmissionregistrationV1WebhookClientConfig(
                    ca_bundle='YQ==',
                    service=IoK8sApiAdmissionregistrationV1ServiceReference(
                        name="name_example",
                        namespace="namespace_example",
                        path="path_example",
                        port=1,
                    ),
                    url="url_example",
                ),
                failure_policy="failure_policy_example",
                match_policy="match_policy_example",
                name="name_example",
                namespace_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(
                    match_expressions=[
                        IoK8sApimachineryPkgApisMetaV1LabelSelectorRequirement(
                            key="key_example",
                            operator="operator_example",
                            values=[
                                "values_example"
                            ],
                        )
                    ],
                    match_labels=dict(
                        "key": "key_example",
                    ),
                ),
                object_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(),
                reinvocation_policy="reinvocation_policy_example",
                rules=[
                    IoK8sApiAdmissionregistrationV1RuleWithOperations(
                        api_groups=[
                            "api_groups_example"
                        ],
                        api_versions=[
                            "api_versions_example"
                        ],
                        operations=[
                            "operations_example"
                        ],
                        resources=[
                            "resources_example"
                        ],
                        scope="scope_example",
                    )
                ],
                side_effects="side_effects_example",
                timeout_seconds=1,
            )
        ],
    )
    try:
        api_response = api_instance.replace_admissionregistration_v1_mutating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->replace_admissionregistration_v1_mutating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
body | typing.Union[SchemaForRequestBody] | required |
query_params | RequestQueryParams | |
path_params | RequestPathParams | |
content_type | str | optional, default is '*/*' | Selects the schema and serialization of the request body
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### body

# SchemaForRequestBody
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
pretty | PrettySchema | | optional
dryRun | DryRunSchema | | optional
fieldManager | FieldManagerSchema | | optional
fieldValidation | FieldValidationSchema | | optional


# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# DryRunSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldManagerSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldValidationSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### path_params
#### RequestPathParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
name | NameSchema | | 

# NameSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#replace_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor200) | OK
201 | [ApiResponseFor201](#replace_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor201) | Created
401 | [ApiResponseFor401](#replace_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### replace_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


#### replace_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor201
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor201ResponseBodyApplicationJson, SchemaFor201ResponseBodyApplicationYaml, SchemaFor201ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor201ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor201ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


# SchemaFor201ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md) |  | 


#### replace_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **replace_admissionregistration_v1_validating_webhook_configuration**
<a name="replace_admissionregistration_v1_validating_webhook_configuration"></a>
> IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration replace_admissionregistration_v1_validating_webhook_configuration(namebody)



replace the specified ValidatingWebhookConfiguration

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_api_admissionregistration_v1_validating_webhook_configuration import IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only required values which don't have defaults set
    path_params = {
        'name': "name_example",
    }
    query_params = {
    }
    body = IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration(
        api_version="api_version_example",
        kind="kind_example",
        metadata=IoK8sApimachineryPkgApisMetaV1ObjectMeta(
            annotations=dict(
                "key": "key_example",
            ),
            creation_timestamp="1970-01-01T00:00:00.00Z",
            deletion_grace_period_seconds=1,
            deletion_timestamp="1970-01-01T00:00:00.00Z",
            finalizers=[
                "finalizers_example"
            ],
            generate_name="generate_name_example",
            generation=1,
            labels=dict(
                "key": "key_example",
            ),
            managed_fields=[
                IoK8sApimachineryPkgApisMetaV1ManagedFieldsEntry(
                    api_version="api_version_example",
                    fields_type="fields_type_example",
                    fields_v1=dict(),
                    manager="manager_example",
                    operation="operation_example",
                    subresource="subresource_example",
                    time="1970-01-01T00:00:00.00Z",
                )
            ],
            name="name_example",
            namespace="namespace_example",
            owner_references=[
                IoK8sApimachineryPkgApisMetaV1OwnerReference(
                    api_version="api_version_example",
                    block_owner_deletion=True,
                    controller=True,
                    kind="kind_example",
                    name="name_example",
                    uid="uid_example",
                )
            ],
            resource_version="resource_version_example",
            self_link="self_link_example",
            uid="uid_example",
        ),
        webhooks=[
            IoK8sApiAdmissionregistrationV1ValidatingWebhook(
                admission_review_versions=[
                    "admission_review_versions_example"
                ],
                client_config=IoK8sApiAdmissionregistrationV1WebhookClientConfig(
                    ca_bundle='YQ==',
                    service=IoK8sApiAdmissionregistrationV1ServiceReference(
                        name="name_example",
                        namespace="namespace_example",
                        path="path_example",
                        port=1,
                    ),
                    url="url_example",
                ),
                failure_policy="failure_policy_example",
                match_policy="match_policy_example",
                name="name_example",
                namespace_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(
                    match_expressions=[
                        IoK8sApimachineryPkgApisMetaV1LabelSelectorRequirement(
                            key="key_example",
                            operator="operator_example",
                            values=[
                                "values_example"
                            ],
                        )
                    ],
                    match_labels=dict(
                        "key": "key_example",
                    ),
                ),
                object_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(),
                rules=[
                    IoK8sApiAdmissionregistrationV1RuleWithOperations(
                        api_groups=[
                            "api_groups_example"
                        ],
                        api_versions=[
                            "api_versions_example"
                        ],
                        operations=[
                            "operations_example"
                        ],
                        resources=[
                            "resources_example"
                        ],
                        scope="scope_example",
                    )
                ],
                side_effects="side_effects_example",
                timeout_seconds=1,
            )
        ],
    )
    try:
        api_response = api_instance.replace_admissionregistration_v1_validating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->replace_admissionregistration_v1_validating_webhook_configuration: %s\n" % e)

    # example passing only optional values
    path_params = {
        'name': "name_example",
    }
    query_params = {
        'pretty': "pretty_example",
        'dryRun': "dryRun_example",
        'fieldManager': "fieldManager_example",
        'fieldValidation': "fieldValidation_example",
    }
    body = IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration(
        api_version="api_version_example",
        kind="kind_example",
        metadata=IoK8sApimachineryPkgApisMetaV1ObjectMeta(
            annotations=dict(
                "key": "key_example",
            ),
            creation_timestamp="1970-01-01T00:00:00.00Z",
            deletion_grace_period_seconds=1,
            deletion_timestamp="1970-01-01T00:00:00.00Z",
            finalizers=[
                "finalizers_example"
            ],
            generate_name="generate_name_example",
            generation=1,
            labels=dict(
                "key": "key_example",
            ),
            managed_fields=[
                IoK8sApimachineryPkgApisMetaV1ManagedFieldsEntry(
                    api_version="api_version_example",
                    fields_type="fields_type_example",
                    fields_v1=dict(),
                    manager="manager_example",
                    operation="operation_example",
                    subresource="subresource_example",
                    time="1970-01-01T00:00:00.00Z",
                )
            ],
            name="name_example",
            namespace="namespace_example",
            owner_references=[
                IoK8sApimachineryPkgApisMetaV1OwnerReference(
                    api_version="api_version_example",
                    block_owner_deletion=True,
                    controller=True,
                    kind="kind_example",
                    name="name_example",
                    uid="uid_example",
                )
            ],
            resource_version="resource_version_example",
            self_link="self_link_example",
            uid="uid_example",
        ),
        webhooks=[
            IoK8sApiAdmissionregistrationV1ValidatingWebhook(
                admission_review_versions=[
                    "admission_review_versions_example"
                ],
                client_config=IoK8sApiAdmissionregistrationV1WebhookClientConfig(
                    ca_bundle='YQ==',
                    service=IoK8sApiAdmissionregistrationV1ServiceReference(
                        name="name_example",
                        namespace="namespace_example",
                        path="path_example",
                        port=1,
                    ),
                    url="url_example",
                ),
                failure_policy="failure_policy_example",
                match_policy="match_policy_example",
                name="name_example",
                namespace_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(
                    match_expressions=[
                        IoK8sApimachineryPkgApisMetaV1LabelSelectorRequirement(
                            key="key_example",
                            operator="operator_example",
                            values=[
                                "values_example"
                            ],
                        )
                    ],
                    match_labels=dict(
                        "key": "key_example",
                    ),
                ),
                object_selector=IoK8sApimachineryPkgApisMetaV1LabelSelector(),
                rules=[
                    IoK8sApiAdmissionregistrationV1RuleWithOperations(
                        api_groups=[
                            "api_groups_example"
                        ],
                        api_versions=[
                            "api_versions_example"
                        ],
                        operations=[
                            "operations_example"
                        ],
                        resources=[
                            "resources_example"
                        ],
                        scope="scope_example",
                    )
                ],
                side_effects="side_effects_example",
                timeout_seconds=1,
            )
        ],
    )
    try:
        api_response = api_instance.replace_admissionregistration_v1_validating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
            body=body,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->replace_admissionregistration_v1_validating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
body | typing.Union[SchemaForRequestBody] | required |
query_params | RequestQueryParams | |
path_params | RequestPathParams | |
content_type | str | optional, default is '*/*' | Selects the schema and serialization of the request body
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### body

# SchemaForRequestBody
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
pretty | PrettySchema | | optional
dryRun | DryRunSchema | | optional
fieldManager | FieldManagerSchema | | optional
fieldValidation | FieldValidationSchema | | optional


# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# DryRunSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldManagerSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldValidationSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### path_params
#### RequestPathParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
name | NameSchema | | 

# NameSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#replace_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor200) | OK
201 | [ApiResponseFor201](#replace_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor201) | Created
401 | [ApiResponseFor401](#replace_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### replace_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


#### replace_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor201
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor201ResponseBodyApplicationJson, SchemaFor201ResponseBodyApplicationYaml, SchemaFor201ResponseBodyApplicationVndKubernetesProtobuf, ] |  |
headers | Unset | headers were not defined |

# SchemaFor201ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor201ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


# SchemaFor201ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration**](../../models/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md) |  | 


#### replace_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **watch_admissionregistration_v1_mutating_webhook_configuration**
<a name="watch_admissionregistration_v1_mutating_webhook_configuration"></a>
> IoK8sApimachineryPkgApisMetaV1WatchEvent watch_admissionregistration_v1_mutating_webhook_configuration(name)



watch changes to an object of kind MutatingWebhookConfiguration. deprecated: use the 'watch' parameter with a list operation instead, filtered to a single item with the 'fieldSelector' parameter.

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_apimachinery_pkg_apis_meta_v1_watch_event import IoK8sApimachineryPkgApisMetaV1WatchEvent
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only required values which don't have defaults set
    path_params = {
        'name': "name_example",
    }
    query_params = {
    }
    try:
        api_response = api_instance.watch_admissionregistration_v1_mutating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->watch_admissionregistration_v1_mutating_webhook_configuration: %s\n" % e)

    # example passing only optional values
    path_params = {
        'name': "name_example",
    }
    query_params = {
        'allowWatchBookmarks': True,
        'continue': "continue_example",
        'fieldSelector': "fieldSelector_example",
        'labelSelector': "labelSelector_example",
        'limit': 1,
        'pretty': "pretty_example",
        'resourceVersion': "resourceVersion_example",
        'resourceVersionMatch': "resourceVersionMatch_example",
        'timeoutSeconds': 1,
        'watch': True,
    }
    try:
        api_response = api_instance.watch_admissionregistration_v1_mutating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->watch_admissionregistration_v1_mutating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
query_params | RequestQueryParams | |
path_params | RequestPathParams | |
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', 'application/json;stream&#x3D;watch', 'application/vnd.kubernetes.protobuf;stream&#x3D;watch', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
allowWatchBookmarks | AllowWatchBookmarksSchema | | optional
continue | ModelContinueSchema | | optional
fieldSelector | FieldSelectorSchema | | optional
labelSelector | LabelSelectorSchema | | optional
limit | LimitSchema | | optional
pretty | PrettySchema | | optional
resourceVersion | ResourceVersionSchema | | optional
resourceVersionMatch | ResourceVersionMatchSchema | | optional
timeoutSeconds | TimeoutSecondsSchema | | optional
watch | WatchSchema | | optional


# AllowWatchBookmarksSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

# ModelContinueSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# LabelSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# LimitSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ResourceVersionSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ResourceVersionMatchSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# TimeoutSecondsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# WatchSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

### path_params
#### RequestPathParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
name | NameSchema | | 

# NameSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#watch_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor200) | OK
401 | [ApiResponseFor401](#watch_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### watch_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, SchemaFor200ResponseBodyApplicationJsonstreamwatch, SchemaFor200ResponseBodyApplicationVndKubernetesProtobufstreamwatch, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationJsonstreamwatch
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobufstreamwatch
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


#### watch_admissionregistration_v1_mutating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **watch_admissionregistration_v1_mutating_webhook_configuration_list**
<a name="watch_admissionregistration_v1_mutating_webhook_configuration_list"></a>
> IoK8sApimachineryPkgApisMetaV1WatchEvent watch_admissionregistration_v1_mutating_webhook_configuration_list()



watch individual changes to a list of MutatingWebhookConfiguration. deprecated: use the 'watch' parameter with a list operation instead.

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_apimachinery_pkg_apis_meta_v1_watch_event import IoK8sApimachineryPkgApisMetaV1WatchEvent
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only optional values
    query_params = {
        'allowWatchBookmarks': True,
        'continue': "continue_example",
        'fieldSelector': "fieldSelector_example",
        'labelSelector': "labelSelector_example",
        'limit': 1,
        'pretty': "pretty_example",
        'resourceVersion': "resourceVersion_example",
        'resourceVersionMatch': "resourceVersionMatch_example",
        'timeoutSeconds': 1,
        'watch': True,
    }
    try:
        api_response = api_instance.watch_admissionregistration_v1_mutating_webhook_configuration_list(
            query_params=query_params,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->watch_admissionregistration_v1_mutating_webhook_configuration_list: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
query_params | RequestQueryParams | |
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', 'application/json;stream&#x3D;watch', 'application/vnd.kubernetes.protobuf;stream&#x3D;watch', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
allowWatchBookmarks | AllowWatchBookmarksSchema | | optional
continue | ModelContinueSchema | | optional
fieldSelector | FieldSelectorSchema | | optional
labelSelector | LabelSelectorSchema | | optional
limit | LimitSchema | | optional
pretty | PrettySchema | | optional
resourceVersion | ResourceVersionSchema | | optional
resourceVersionMatch | ResourceVersionMatchSchema | | optional
timeoutSeconds | TimeoutSecondsSchema | | optional
watch | WatchSchema | | optional


# AllowWatchBookmarksSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

# ModelContinueSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# LabelSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# LimitSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ResourceVersionSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ResourceVersionMatchSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# TimeoutSecondsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# WatchSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#watch_admissionregistration_v1_mutating_webhook_configuration_list.ApiResponseFor200) | OK
401 | [ApiResponseFor401](#watch_admissionregistration_v1_mutating_webhook_configuration_list.ApiResponseFor401) | Unauthorized

#### watch_admissionregistration_v1_mutating_webhook_configuration_list.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, SchemaFor200ResponseBodyApplicationJsonstreamwatch, SchemaFor200ResponseBodyApplicationVndKubernetesProtobufstreamwatch, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationJsonstreamwatch
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobufstreamwatch
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


#### watch_admissionregistration_v1_mutating_webhook_configuration_list.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **watch_admissionregistration_v1_validating_webhook_configuration**
<a name="watch_admissionregistration_v1_validating_webhook_configuration"></a>
> IoK8sApimachineryPkgApisMetaV1WatchEvent watch_admissionregistration_v1_validating_webhook_configuration(name)



watch changes to an object of kind ValidatingWebhookConfiguration. deprecated: use the 'watch' parameter with a list operation instead, filtered to a single item with the 'fieldSelector' parameter.

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_apimachinery_pkg_apis_meta_v1_watch_event import IoK8sApimachineryPkgApisMetaV1WatchEvent
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only required values which don't have defaults set
    path_params = {
        'name': "name_example",
    }
    query_params = {
    }
    try:
        api_response = api_instance.watch_admissionregistration_v1_validating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->watch_admissionregistration_v1_validating_webhook_configuration: %s\n" % e)

    # example passing only optional values
    path_params = {
        'name': "name_example",
    }
    query_params = {
        'allowWatchBookmarks': True,
        'continue': "continue_example",
        'fieldSelector': "fieldSelector_example",
        'labelSelector': "labelSelector_example",
        'limit': 1,
        'pretty': "pretty_example",
        'resourceVersion': "resourceVersion_example",
        'resourceVersionMatch': "resourceVersionMatch_example",
        'timeoutSeconds': 1,
        'watch': True,
    }
    try:
        api_response = api_instance.watch_admissionregistration_v1_validating_webhook_configuration(
            path_params=path_params,
            query_params=query_params,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->watch_admissionregistration_v1_validating_webhook_configuration: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
query_params | RequestQueryParams | |
path_params | RequestPathParams | |
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', 'application/json;stream&#x3D;watch', 'application/vnd.kubernetes.protobuf;stream&#x3D;watch', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
allowWatchBookmarks | AllowWatchBookmarksSchema | | optional
continue | ModelContinueSchema | | optional
fieldSelector | FieldSelectorSchema | | optional
labelSelector | LabelSelectorSchema | | optional
limit | LimitSchema | | optional
pretty | PrettySchema | | optional
resourceVersion | ResourceVersionSchema | | optional
resourceVersionMatch | ResourceVersionMatchSchema | | optional
timeoutSeconds | TimeoutSecondsSchema | | optional
watch | WatchSchema | | optional


# AllowWatchBookmarksSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

# ModelContinueSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# LabelSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# LimitSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ResourceVersionSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ResourceVersionMatchSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# TimeoutSecondsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# WatchSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

### path_params
#### RequestPathParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
name | NameSchema | | 

# NameSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#watch_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor200) | OK
401 | [ApiResponseFor401](#watch_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor401) | Unauthorized

#### watch_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, SchemaFor200ResponseBodyApplicationJsonstreamwatch, SchemaFor200ResponseBodyApplicationVndKubernetesProtobufstreamwatch, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationJsonstreamwatch
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobufstreamwatch
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


#### watch_admissionregistration_v1_validating_webhook_configuration.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

# **watch_admissionregistration_v1_validating_webhook_configuration_list**
<a name="watch_admissionregistration_v1_validating_webhook_configuration_list"></a>
> IoK8sApimachineryPkgApisMetaV1WatchEvent watch_admissionregistration_v1_validating_webhook_configuration_list()



watch individual changes to a list of ValidatingWebhookConfiguration. deprecated: use the 'watch' parameter with a list operation instead.

### Example

* Api Key Authentication (BearerToken):
```python
import openapi_client
from openapi_client.apis.tags import admissionregistration_v1_api
from openapi_client.model.io_k8s_apimachinery_pkg_apis_meta_v1_watch_event import IoK8sApimachineryPkgApisMetaV1WatchEvent
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: BearerToken
configuration.api_key['BearerToken'] = 'YOUR_API_KEY'

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['BearerToken'] = 'Bearer'
# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = admissionregistration_v1_api.AdmissionregistrationV1Api(api_client)

    # example passing only optional values
    query_params = {
        'allowWatchBookmarks': True,
        'continue': "continue_example",
        'fieldSelector': "fieldSelector_example",
        'labelSelector': "labelSelector_example",
        'limit': 1,
        'pretty': "pretty_example",
        'resourceVersion': "resourceVersion_example",
        'resourceVersionMatch': "resourceVersionMatch_example",
        'timeoutSeconds': 1,
        'watch': True,
    }
    try:
        api_response = api_instance.watch_admissionregistration_v1_validating_webhook_configuration_list(
            query_params=query_params,
        )
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling AdmissionregistrationV1Api->watch_admissionregistration_v1_validating_webhook_configuration_list: %s\n" % e)
```
### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
query_params | RequestQueryParams | |
accept_content_types | typing.Tuple[str] | default is ('application/json', 'application/yaml', 'application/vnd.kubernetes.protobuf', 'application/json;stream&#x3D;watch', 'application/vnd.kubernetes.protobuf;stream&#x3D;watch', ) | Tells the server the content type(s) that are accepted by the client
stream | bool | default is False | if True then the response.content will be streamed and loaded from a file like object. When downloading a file, set this to True to force the code to deserialize the content to a FileSchema file
timeout | typing.Optional[typing.Union[int, typing.Tuple]] | default is None | the timeout used by the rest client
skip_deserialization | bool | default is False | when True, headers and body will be unset and an instance of api_client.ApiResponseWithoutDeserialization will be returned

### query_params
#### RequestQueryParams

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
allowWatchBookmarks | AllowWatchBookmarksSchema | | optional
continue | ModelContinueSchema | | optional
fieldSelector | FieldSelectorSchema | | optional
labelSelector | LabelSelectorSchema | | optional
limit | LimitSchema | | optional
pretty | PrettySchema | | optional
resourceVersion | ResourceVersionSchema | | optional
resourceVersionMatch | ResourceVersionMatchSchema | | optional
timeoutSeconds | TimeoutSecondsSchema | | optional
watch | WatchSchema | | optional


# AllowWatchBookmarksSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

# ModelContinueSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# FieldSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# LabelSelectorSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# LimitSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# PrettySchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ResourceVersionSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# ResourceVersionMatchSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
str,  | str,  |  | 

# TimeoutSecondsSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
decimal.Decimal, int,  | decimal.Decimal,  |  | 

# WatchSchema

## Model Type Info
Input Type | Accessed Type | Description | Notes
------------ | ------------- | ------------- | -------------
bool,  | BoolClass,  |  | 

### Return Types, Responses

Code | Class | Description
------------- | ------------- | -------------
n/a | api_client.ApiResponseWithoutDeserialization | When skip_deserialization is True this response is returned
200 | [ApiResponseFor200](#watch_admissionregistration_v1_validating_webhook_configuration_list.ApiResponseFor200) | OK
401 | [ApiResponseFor401](#watch_admissionregistration_v1_validating_webhook_configuration_list.ApiResponseFor401) | Unauthorized

#### watch_admissionregistration_v1_validating_webhook_configuration_list.ApiResponseFor200
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[SchemaFor200ResponseBodyApplicationJson, SchemaFor200ResponseBodyApplicationYaml, SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf, SchemaFor200ResponseBodyApplicationJsonstreamwatch, SchemaFor200ResponseBodyApplicationVndKubernetesProtobufstreamwatch, ] |  |
headers | Unset | headers were not defined |

# SchemaFor200ResponseBodyApplicationJson
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationYaml
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobuf
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationJsonstreamwatch
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


# SchemaFor200ResponseBodyApplicationVndKubernetesProtobufstreamwatch
Type | Description  | Notes
------------- | ------------- | -------------
[**IoK8sApimachineryPkgApisMetaV1WatchEvent**](../../models/IoK8sApimachineryPkgApisMetaV1WatchEvent.md) |  | 


#### watch_admissionregistration_v1_validating_webhook_configuration_list.ApiResponseFor401
Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
response | urllib3.HTTPResponse | Raw response |
body | typing.Union[] |  |
headers | Unset | headers were not defined |

### Authorization

[BearerToken](../../../README.md#BearerToken)

[[Back to top]](#__pageTop) [[Back to API list]](../../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../../README.md#documentation-for-models) [[Back to README]](../../../README.md)

