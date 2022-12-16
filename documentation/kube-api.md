# Kubernetes API Python Client

- API version: 1.26
- Package version: 1.0.0
- Build date: 2022-12-16

## Requirements.

Python 2.7 and 3.4+

## Installation & Usage
### pip install

If the python package is hosted on Github, you can install directly from Github

```sh
pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
```
(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)

Then import the package:
```python
import swagger_client 
```

### Setuptools

Install via [Setuptools](http://pypi.python.org/pypi/setuptools).

```sh
python setup.py install --user
```
(or `sudo python setup.py install` to install the package for all users)

Then import the package:
```python
import swagger_client
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

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
api_instance = swagger_client.AdmissionregistrationApi

try:
    api_response = api_instance.get_admissionregistration_api_group()
    pprint(api_response)
except ApiException as e:
    print "Exception when calling AdmissionregistrationApi->get_admissionregistration_api_group: %s\n" % e

```

## Documentation for API Endpoints

All URIs are relative to *https://localhost*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AdmissionregistrationApi* | [**get_admissionregistration_api_group**](docs/AdmissionregistrationApi.md#get_admissionregistration_api_group) | **GET** /apis/admissionregistration.k8s.io/ | 
*AdmissionregistrationvApi* | [**create_admissionregistration_v1_mutating_webhook_configuration**](docs/AdmissionregistrationvApi.md#create_admissionregistration_v1_mutating_webhook_configuration) | **POST** /apis/admissionregistration.k8s.io/v1/mutatingwebhookconfigurations | 
*AdmissionregistrationvApi* | [**create_admissionregistration_v1_validating_webhook_configuration**](docs/AdmissionregistrationvApi.md#create_admissionregistration_v1_validating_webhook_configuration) | **POST** /apis/admissionregistration.k8s.io/v1/validatingwebhookconfigurations | 
*AdmissionregistrationvApi* | [**delete_admissionregistration_v1_collection_mutating_webhook_configuration**](docs/AdmissionregistrationvApi.md#delete_admissionregistration_v1_collection_mutating_webhook_configuration) | **DELETE** /apis/admissionregistration.k8s.io/v1/mutatingwebhookconfigurations | 
*AdmissionregistrationvApi* | [**delete_admissionregistration_v1_collection_validating_webhook_configuration**](docs/AdmissionregistrationvApi.md#delete_admissionregistration_v1_collection_validating_webhook_configuration) | **DELETE** /apis/admissionregistration.k8s.io/v1/validatingwebhookconfigurations | 
*AdmissionregistrationvApi* | [**delete_admissionregistration_v1_mutating_webhook_configuration**](docs/AdmissionregistrationvApi.md#delete_admissionregistration_v1_mutating_webhook_configuration) | **DELETE** /apis/admissionregistration.k8s.io/v1/mutatingwebhookconfigurations/{name} | 
*AdmissionregistrationvApi* | [**delete_admissionregistration_v1_validating_webhook_configuration**](docs/AdmissionregistrationvApi.md#delete_admissionregistration_v1_validating_webhook_configuration) | **DELETE** /apis/admissionregistration.k8s.io/v1/validatingwebhookconfigurations/{name} | 
*AdmissionregistrationvApi* | [**get_admissionregistration_v1_api_resources**](docs/AdmissionregistrationvApi.md#get_admissionregistration_v1_api_resources) | **GET** /apis/admissionregistration.k8s.io/v1/ | 
*AdmissionregistrationvApi* | [**list_admissionregistration_v1_mutating_webhook_configuration**](docs/AdmissionregistrationvApi.md#list_admissionregistration_v1_mutating_webhook_configuration) | **GET** /apis/admissionregistration.k8s.io/v1/mutatingwebhookconfigurations | 
*AdmissionregistrationvApi* | [**list_admissionregistration_v1_validating_webhook_configuration**](docs/AdmissionregistrationvApi.md#list_admissionregistration_v1_validating_webhook_configuration) | **GET** /apis/admissionregistration.k8s.io/v1/validatingwebhookconfigurations | 
*AdmissionregistrationvApi* | [**patch_admissionregistration_v1_mutating_webhook_configuration**](docs/AdmissionregistrationvApi.md#patch_admissionregistration_v1_mutating_webhook_configuration) | **PATCH** /apis/admissionregistration.k8s.io/v1/mutatingwebhookconfigurations/{name} | 
*AdmissionregistrationvApi* | [**patch_admissionregistration_v1_validating_webhook_configuration**](docs/AdmissionregistrationvApi.md#patch_admissionregistration_v1_validating_webhook_configuration) | **PATCH** /apis/admissionregistration.k8s.io/v1/validatingwebhookconfigurations/{name} | 
*AdmissionregistrationvApi* | [**read_admissionregistration_v1_mutating_webhook_configuration**](docs/AdmissionregistrationvApi.md#read_admissionregistration_v1_mutating_webhook_configuration) | **GET** /apis/admissionregistration.k8s.io/v1/mutatingwebhookconfigurations/{name} | 
*AdmissionregistrationvApi* | [**read_admissionregistration_v1_validating_webhook_configuration**](docs/AdmissionregistrationvApi.md#read_admissionregistration_v1_validating_webhook_configuration) | **GET** /apis/admissionregistration.k8s.io/v1/validatingwebhookconfigurations/{name} | 
*AdmissionregistrationvApi* | [**replace_admissionregistration_v1_mutating_webhook_configuration**](docs/AdmissionregistrationvApi.md#replace_admissionregistration_v1_mutating_webhook_configuration) | **PUT** /apis/admissionregistration.k8s.io/v1/mutatingwebhookconfigurations/{name} | 
*AdmissionregistrationvApi* | [**replace_admissionregistration_v1_validating_webhook_configuration**](docs/AdmissionregistrationvApi.md#replace_admissionregistration_v1_validating_webhook_configuration) | **PUT** /apis/admissionregistration.k8s.io/v1/validatingwebhookconfigurations/{name} | 
*AdmissionregistrationvApi* | [**watch_admissionregistration_v1_mutating_webhook_configuration**](docs/AdmissionregistrationvApi.md#watch_admissionregistration_v1_mutating_webhook_configuration) | **GET** /apis/admissionregistration.k8s.io/v1/watch/mutatingwebhookconfigurations/{name} | 
*AdmissionregistrationvApi* | [**watch_admissionregistration_v1_mutating_webhook_configuration_list**](docs/AdmissionregistrationvApi.md#watch_admissionregistration_v1_mutating_webhook_configuration_list) | **GET** /apis/admissionregistration.k8s.io/v1/watch/mutatingwebhookconfigurations | 
*AdmissionregistrationvApi* | [**watch_admissionregistration_v1_validating_webhook_configuration**](docs/AdmissionregistrationvApi.md#watch_admissionregistration_v1_validating_webhook_configuration) | **GET** /apis/admissionregistration.k8s.io/v1/watch/validatingwebhookconfigurations/{name} | 
*AdmissionregistrationvApi* | [**watch_admissionregistration_v1_validating_webhook_configuration_list**](docs/AdmissionregistrationvApi.md#watch_admissionregistration_v1_validating_webhook_configuration_list) | **GET** /apis/admissionregistration.k8s.io/v1/watch/validatingwebhookconfigurations | 
*AdmissionregistrationvalphaApi* | [**create_admissionregistration_v1alpha1_validating_admission_policy**](docs/AdmissionregistrationvalphaApi.md#create_admissionregistration_v1alpha1_validating_admission_policy) | **POST** /apis/admissionregistration.k8s.io/v1alpha1/validatingadmissionpolicies | 
*AdmissionregistrationvalphaApi* | [**create_admissionregistration_v1alpha1_validating_admission_policy_binding**](docs/AdmissionregistrationvalphaApi.md#create_admissionregistration_v1alpha1_validating_admission_policy_binding) | **POST** /apis/admissionregistration.k8s.io/v1alpha1/validatingadmissionpolicybindings | 
*AdmissionregistrationvalphaApi* | [**delete_admissionregistration_v1alpha1_collection_validating_admission_policy**](docs/AdmissionregistrationvalphaApi.md#delete_admissionregistration_v1alpha1_collection_validating_admission_policy) | **DELETE** /apis/admissionregistration.k8s.io/v1alpha1/validatingadmissionpolicies | 
*AdmissionregistrationvalphaApi* | [**delete_admissionregistration_v1alpha1_collection_validating_admission_policy_binding**](docs/AdmissionregistrationvalphaApi.md#delete_admissionregistration_v1alpha1_collection_validating_admission_policy_binding) | **DELETE** /apis/admissionregistration.k8s.io/v1alpha1/validatingadmissionpolicybindings | 
*AdmissionregistrationvalphaApi* | [**delete_admissionregistration_v1alpha1_validating_admission_policy**](docs/AdmissionregistrationvalphaApi.md#delete_admissionregistration_v1alpha1_validating_admission_policy) | **DELETE** /apis/admissionregistration.k8s.io/v1alpha1/validatingadmissionpolicies/{name} | 
*AdmissionregistrationvalphaApi* | [**delete_admissionregistration_v1alpha1_validating_admission_policy_binding**](docs/AdmissionregistrationvalphaApi.md#delete_admissionregistration_v1alpha1_validating_admission_policy_binding) | **DELETE** /apis/admissionregistration.k8s.io/v1alpha1/validatingadmissionpolicybindings/{name} | 
*AdmissionregistrationvalphaApi* | [**get_admissionregistration_v1alpha1_api_resources**](docs/AdmissionregistrationvalphaApi.md#get_admissionregistration_v1alpha1_api_resources) | **GET** /apis/admissionregistration.k8s.io/v1alpha1/ | 
*AdmissionregistrationvalphaApi* | [**list_admissionregistration_v1alpha1_validating_admission_policy**](docs/AdmissionregistrationvalphaApi.md#list_admissionregistration_v1alpha1_validating_admission_policy) | **GET** /apis/admissionregistration.k8s.io/v1alpha1/validatingadmissionpolicies | 
*AdmissionregistrationvalphaApi* | [**list_admissionregistration_v1alpha1_validating_admission_policy_binding**](docs/AdmissionregistrationvalphaApi.md#list_admissionregistration_v1alpha1_validating_admission_policy_binding) | **GET** /apis/admissionregistration.k8s.io/v1alpha1/validatingadmissionpolicybindings | 
*AdmissionregistrationvalphaApi* | [**patch_admissionregistration_v1alpha1_validating_admission_policy**](docs/AdmissionregistrationvalphaApi.md#patch_admissionregistration_v1alpha1_validating_admission_policy) | **PATCH** /apis/admissionregistration.k8s.io/v1alpha1/validatingadmissionpolicies/{name} | 
*AdmissionregistrationvalphaApi* | [**patch_admissionregistration_v1alpha1_validating_admission_policy_binding**](docs/AdmissionregistrationvalphaApi.md#patch_admissionregistration_v1alpha1_validating_admission_policy_binding) | **PATCH** /apis/admissionregistration.k8s.io/v1alpha1/validatingadmissionpolicybindings/{name} | 
*AdmissionregistrationvalphaApi* | [**read_admissionregistration_v1alpha1_validating_admission_policy**](docs/AdmissionregistrationvalphaApi.md#read_admissionregistration_v1alpha1_validating_admission_policy) | **GET** /apis/admissionregistration.k8s.io/v1alpha1/validatingadmissionpolicies/{name} | 
*AdmissionregistrationvalphaApi* | [**read_admissionregistration_v1alpha1_validating_admission_policy_binding**](docs/AdmissionregistrationvalphaApi.md#read_admissionregistration_v1alpha1_validating_admission_policy_binding) | **GET** /apis/admissionregistration.k8s.io/v1alpha1/validatingadmissionpolicybindings/{name} | 
*AdmissionregistrationvalphaApi* | [**replace_admissionregistration_v1alpha1_validating_admission_policy**](docs/AdmissionregistrationvalphaApi.md#replace_admissionregistration_v1alpha1_validating_admission_policy) | **PUT** /apis/admissionregistration.k8s.io/v1alpha1/validatingadmissionpolicies/{name} | 
*AdmissionregistrationvalphaApi* | [**replace_admissionregistration_v1alpha1_validating_admission_policy_binding**](docs/AdmissionregistrationvalphaApi.md#replace_admissionregistration_v1alpha1_validating_admission_policy_binding) | **PUT** /apis/admissionregistration.k8s.io/v1alpha1/validatingadmissionpolicybindings/{name} | 
*AdmissionregistrationvalphaApi* | [**watch_admissionregistration_v1alpha1_validating_admission_policy**](docs/AdmissionregistrationvalphaApi.md#watch_admissionregistration_v1alpha1_validating_admission_policy) | **GET** /apis/admissionregistration.k8s.io/v1alpha1/watch/validatingadmissionpolicies/{name} | 
*AdmissionregistrationvalphaApi* | [**watch_admissionregistration_v1alpha1_validating_admission_policy_binding**](docs/AdmissionregistrationvalphaApi.md#watch_admissionregistration_v1alpha1_validating_admission_policy_binding) | **GET** /apis/admissionregistration.k8s.io/v1alpha1/watch/validatingadmissionpolicybindings/{name} | 
*AdmissionregistrationvalphaApi* | [**watch_admissionregistration_v1alpha1_validating_admission_policy_binding_list**](docs/AdmissionregistrationvalphaApi.md#watch_admissionregistration_v1alpha1_validating_admission_policy_binding_list) | **GET** /apis/admissionregistration.k8s.io/v1alpha1/watch/validatingadmissionpolicybindings | 
*AdmissionregistrationvalphaApi* | [**watch_admissionregistration_v1alpha1_validating_admission_policy_list**](docs/AdmissionregistrationvalphaApi.md#watch_admissionregistration_v1alpha1_validating_admission_policy_list) | **GET** /apis/admissionregistration.k8s.io/v1alpha1/watch/validatingadmissionpolicies | 
*ApiextensionsApi* | [**get_apiextensions_api_group**](docs/ApiextensionsApi.md#get_apiextensions_api_group) | **GET** /apis/apiextensions.k8s.io/ | 
*ApiextensionsvApi* | [**create_apiextensions_v1_custom_resource_definition**](docs/ApiextensionsvApi.md#create_apiextensions_v1_custom_resource_definition) | **POST** /apis/apiextensions.k8s.io/v1/customresourcedefinitions | 
*ApiextensionsvApi* | [**delete_apiextensions_v1_collection_custom_resource_definition**](docs/ApiextensionsvApi.md#delete_apiextensions_v1_collection_custom_resource_definition) | **DELETE** /apis/apiextensions.k8s.io/v1/customresourcedefinitions | 
*ApiextensionsvApi* | [**delete_apiextensions_v1_custom_resource_definition**](docs/ApiextensionsvApi.md#delete_apiextensions_v1_custom_resource_definition) | **DELETE** /apis/apiextensions.k8s.io/v1/customresourcedefinitions/{name} | 
*ApiextensionsvApi* | [**get_apiextensions_v1_api_resources**](docs/ApiextensionsvApi.md#get_apiextensions_v1_api_resources) | **GET** /apis/apiextensions.k8s.io/v1/ | 
*ApiextensionsvApi* | [**list_apiextensions_v1_custom_resource_definition**](docs/ApiextensionsvApi.md#list_apiextensions_v1_custom_resource_definition) | **GET** /apis/apiextensions.k8s.io/v1/customresourcedefinitions | 
*ApiextensionsvApi* | [**patch_apiextensions_v1_custom_resource_definition**](docs/ApiextensionsvApi.md#patch_apiextensions_v1_custom_resource_definition) | **PATCH** /apis/apiextensions.k8s.io/v1/customresourcedefinitions/{name} | 
*ApiextensionsvApi* | [**patch_apiextensions_v1_custom_resource_definition_status**](docs/ApiextensionsvApi.md#patch_apiextensions_v1_custom_resource_definition_status) | **PATCH** /apis/apiextensions.k8s.io/v1/customresourcedefinitions/{name}/status | 
*ApiextensionsvApi* | [**read_apiextensions_v1_custom_resource_definition**](docs/ApiextensionsvApi.md#read_apiextensions_v1_custom_resource_definition) | **GET** /apis/apiextensions.k8s.io/v1/customresourcedefinitions/{name} | 
*ApiextensionsvApi* | [**read_apiextensions_v1_custom_resource_definition_status**](docs/ApiextensionsvApi.md#read_apiextensions_v1_custom_resource_definition_status) | **GET** /apis/apiextensions.k8s.io/v1/customresourcedefinitions/{name}/status | 
*ApiextensionsvApi* | [**replace_apiextensions_v1_custom_resource_definition**](docs/ApiextensionsvApi.md#replace_apiextensions_v1_custom_resource_definition) | **PUT** /apis/apiextensions.k8s.io/v1/customresourcedefinitions/{name} | 
*ApiextensionsvApi* | [**replace_apiextensions_v1_custom_resource_definition_status**](docs/ApiextensionsvApi.md#replace_apiextensions_v1_custom_resource_definition_status) | **PUT** /apis/apiextensions.k8s.io/v1/customresourcedefinitions/{name}/status | 
*ApiextensionsvApi* | [**watch_apiextensions_v1_custom_resource_definition**](docs/ApiextensionsvApi.md#watch_apiextensions_v1_custom_resource_definition) | **GET** /apis/apiextensions.k8s.io/v1/watch/customresourcedefinitions/{name} | 
*ApiextensionsvApi* | [**watch_apiextensions_v1_custom_resource_definition_list**](docs/ApiextensionsvApi.md#watch_apiextensions_v1_custom_resource_definition_list) | **GET** /apis/apiextensions.k8s.io/v1/watch/customresourcedefinitions | 
*ApiregistrationApi* | [**get_apiregistration_api_group**](docs/ApiregistrationApi.md#get_apiregistration_api_group) | **GET** /apis/apiregistration.k8s.io/ | 
*ApiregistrationvApi* | [**create_apiregistration_v1_api_service**](docs/ApiregistrationvApi.md#create_apiregistration_v1_api_service) | **POST** /apis/apiregistration.k8s.io/v1/apiservices | 
*ApiregistrationvApi* | [**delete_apiregistration_v1_api_service**](docs/ApiregistrationvApi.md#delete_apiregistration_v1_api_service) | **DELETE** /apis/apiregistration.k8s.io/v1/apiservices/{name} | 
*ApiregistrationvApi* | [**delete_apiregistration_v1_collection_api_service**](docs/ApiregistrationvApi.md#delete_apiregistration_v1_collection_api_service) | **DELETE** /apis/apiregistration.k8s.io/v1/apiservices | 
*ApiregistrationvApi* | [**get_apiregistration_v1_api_resources**](docs/ApiregistrationvApi.md#get_apiregistration_v1_api_resources) | **GET** /apis/apiregistration.k8s.io/v1/ | 
*ApiregistrationvApi* | [**list_apiregistration_v1_api_service**](docs/ApiregistrationvApi.md#list_apiregistration_v1_api_service) | **GET** /apis/apiregistration.k8s.io/v1/apiservices | 
*ApiregistrationvApi* | [**patch_apiregistration_v1_api_service**](docs/ApiregistrationvApi.md#patch_apiregistration_v1_api_service) | **PATCH** /apis/apiregistration.k8s.io/v1/apiservices/{name} | 
*ApiregistrationvApi* | [**patch_apiregistration_v1_api_service_status**](docs/ApiregistrationvApi.md#patch_apiregistration_v1_api_service_status) | **PATCH** /apis/apiregistration.k8s.io/v1/apiservices/{name}/status | 
*ApiregistrationvApi* | [**read_apiregistration_v1_api_service**](docs/ApiregistrationvApi.md#read_apiregistration_v1_api_service) | **GET** /apis/apiregistration.k8s.io/v1/apiservices/{name} | 
*ApiregistrationvApi* | [**read_apiregistration_v1_api_service_status**](docs/ApiregistrationvApi.md#read_apiregistration_v1_api_service_status) | **GET** /apis/apiregistration.k8s.io/v1/apiservices/{name}/status | 
*ApiregistrationvApi* | [**replace_apiregistration_v1_api_service**](docs/ApiregistrationvApi.md#replace_apiregistration_v1_api_service) | **PUT** /apis/apiregistration.k8s.io/v1/apiservices/{name} | 
*ApiregistrationvApi* | [**replace_apiregistration_v1_api_service_status**](docs/ApiregistrationvApi.md#replace_apiregistration_v1_api_service_status) | **PUT** /apis/apiregistration.k8s.io/v1/apiservices/{name}/status | 
*ApiregistrationvApi* | [**watch_apiregistration_v1_api_service**](docs/ApiregistrationvApi.md#watch_apiregistration_v1_api_service) | **GET** /apis/apiregistration.k8s.io/v1/watch/apiservices/{name} | 
*ApiregistrationvApi* | [**watch_apiregistration_v1_api_service_list**](docs/ApiregistrationvApi.md#watch_apiregistration_v1_api_service_list) | **GET** /apis/apiregistration.k8s.io/v1/watch/apiservices | 
*ApisApi* | [**get_api_versions**](docs/ApisApi.md#get_api_versions) | **GET** /apis/ | 
*AppsApi* | [**get_apps_api_group**](docs/AppsApi.md#get_apps_api_group) | **GET** /apis/apps/ | 
*AppsvApi* | [**create_apps_v1_namespaced_controller_revision**](docs/AppsvApi.md#create_apps_v1_namespaced_controller_revision) | **POST** /apis/apps/v1/namespaces/{namespace}/controllerrevisions | 
*AppsvApi* | [**create_apps_v1_namespaced_daemon_set**](docs/AppsvApi.md#create_apps_v1_namespaced_daemon_set) | **POST** /apis/apps/v1/namespaces/{namespace}/daemonsets | 
*AppsvApi* | [**create_apps_v1_namespaced_deployment**](docs/AppsvApi.md#create_apps_v1_namespaced_deployment) | **POST** /apis/apps/v1/namespaces/{namespace}/deployments | 
*AppsvApi* | [**create_apps_v1_namespaced_replica_set**](docs/AppsvApi.md#create_apps_v1_namespaced_replica_set) | **POST** /apis/apps/v1/namespaces/{namespace}/replicasets | 
*AppsvApi* | [**create_apps_v1_namespaced_stateful_set**](docs/AppsvApi.md#create_apps_v1_namespaced_stateful_set) | **POST** /apis/apps/v1/namespaces/{namespace}/statefulsets | 
*AppsvApi* | [**delete_apps_v1_collection_namespaced_controller_revision**](docs/AppsvApi.md#delete_apps_v1_collection_namespaced_controller_revision) | **DELETE** /apis/apps/v1/namespaces/{namespace}/controllerrevisions | 
*AppsvApi* | [**delete_apps_v1_collection_namespaced_daemon_set**](docs/AppsvApi.md#delete_apps_v1_collection_namespaced_daemon_set) | **DELETE** /apis/apps/v1/namespaces/{namespace}/daemonsets | 
*AppsvApi* | [**delete_apps_v1_collection_namespaced_deployment**](docs/AppsvApi.md#delete_apps_v1_collection_namespaced_deployment) | **DELETE** /apis/apps/v1/namespaces/{namespace}/deployments | 
*AppsvApi* | [**delete_apps_v1_collection_namespaced_replica_set**](docs/AppsvApi.md#delete_apps_v1_collection_namespaced_replica_set) | **DELETE** /apis/apps/v1/namespaces/{namespace}/replicasets | 
*AppsvApi* | [**delete_apps_v1_collection_namespaced_stateful_set**](docs/AppsvApi.md#delete_apps_v1_collection_namespaced_stateful_set) | **DELETE** /apis/apps/v1/namespaces/{namespace}/statefulsets | 
*AppsvApi* | [**delete_apps_v1_namespaced_controller_revision**](docs/AppsvApi.md#delete_apps_v1_namespaced_controller_revision) | **DELETE** /apis/apps/v1/namespaces/{namespace}/controllerrevisions/{name} | 
*AppsvApi* | [**delete_apps_v1_namespaced_daemon_set**](docs/AppsvApi.md#delete_apps_v1_namespaced_daemon_set) | **DELETE** /apis/apps/v1/namespaces/{namespace}/daemonsets/{name} | 
*AppsvApi* | [**delete_apps_v1_namespaced_deployment**](docs/AppsvApi.md#delete_apps_v1_namespaced_deployment) | **DELETE** /apis/apps/v1/namespaces/{namespace}/deployments/{name} | 
*AppsvApi* | [**delete_apps_v1_namespaced_replica_set**](docs/AppsvApi.md#delete_apps_v1_namespaced_replica_set) | **DELETE** /apis/apps/v1/namespaces/{namespace}/replicasets/{name} | 
*AppsvApi* | [**delete_apps_v1_namespaced_stateful_set**](docs/AppsvApi.md#delete_apps_v1_namespaced_stateful_set) | **DELETE** /apis/apps/v1/namespaces/{namespace}/statefulsets/{name} | 
*AppsvApi* | [**get_apps_v1_api_resources**](docs/AppsvApi.md#get_apps_v1_api_resources) | **GET** /apis/apps/v1/ | 
*AppsvApi* | [**list_apps_v1_controller_revision_for_all_namespaces**](docs/AppsvApi.md#list_apps_v1_controller_revision_for_all_namespaces) | **GET** /apis/apps/v1/controllerrevisions | 
*AppsvApi* | [**list_apps_v1_daemon_set_for_all_namespaces**](docs/AppsvApi.md#list_apps_v1_daemon_set_for_all_namespaces) | **GET** /apis/apps/v1/daemonsets | 
*AppsvApi* | [**list_apps_v1_deployment_for_all_namespaces**](docs/AppsvApi.md#list_apps_v1_deployment_for_all_namespaces) | **GET** /apis/apps/v1/deployments | 
*AppsvApi* | [**list_apps_v1_namespaced_controller_revision**](docs/AppsvApi.md#list_apps_v1_namespaced_controller_revision) | **GET** /apis/apps/v1/namespaces/{namespace}/controllerrevisions | 
*AppsvApi* | [**list_apps_v1_namespaced_daemon_set**](docs/AppsvApi.md#list_apps_v1_namespaced_daemon_set) | **GET** /apis/apps/v1/namespaces/{namespace}/daemonsets | 
*AppsvApi* | [**list_apps_v1_namespaced_deployment**](docs/AppsvApi.md#list_apps_v1_namespaced_deployment) | **GET** /apis/apps/v1/namespaces/{namespace}/deployments | 
*AppsvApi* | [**list_apps_v1_namespaced_replica_set**](docs/AppsvApi.md#list_apps_v1_namespaced_replica_set) | **GET** /apis/apps/v1/namespaces/{namespace}/replicasets | 
*AppsvApi* | [**list_apps_v1_namespaced_stateful_set**](docs/AppsvApi.md#list_apps_v1_namespaced_stateful_set) | **GET** /apis/apps/v1/namespaces/{namespace}/statefulsets | 
*AppsvApi* | [**list_apps_v1_replica_set_for_all_namespaces**](docs/AppsvApi.md#list_apps_v1_replica_set_for_all_namespaces) | **GET** /apis/apps/v1/replicasets | 
*AppsvApi* | [**list_apps_v1_stateful_set_for_all_namespaces**](docs/AppsvApi.md#list_apps_v1_stateful_set_for_all_namespaces) | **GET** /apis/apps/v1/statefulsets | 
*AppsvApi* | [**patch_apps_v1_namespaced_controller_revision**](docs/AppsvApi.md#patch_apps_v1_namespaced_controller_revision) | **PATCH** /apis/apps/v1/namespaces/{namespace}/controllerrevisions/{name} | 
*AppsvApi* | [**patch_apps_v1_namespaced_daemon_set**](docs/AppsvApi.md#patch_apps_v1_namespaced_daemon_set) | **PATCH** /apis/apps/v1/namespaces/{namespace}/daemonsets/{name} | 
*AppsvApi* | [**patch_apps_v1_namespaced_daemon_set_status**](docs/AppsvApi.md#patch_apps_v1_namespaced_daemon_set_status) | **PATCH** /apis/apps/v1/namespaces/{namespace}/daemonsets/{name}/status | 
*AppsvApi* | [**patch_apps_v1_namespaced_deployment**](docs/AppsvApi.md#patch_apps_v1_namespaced_deployment) | **PATCH** /apis/apps/v1/namespaces/{namespace}/deployments/{name} | 
*AppsvApi* | [**patch_apps_v1_namespaced_deployment_scale**](docs/AppsvApi.md#patch_apps_v1_namespaced_deployment_scale) | **PATCH** /apis/apps/v1/namespaces/{namespace}/deployments/{name}/scale | 
*AppsvApi* | [**patch_apps_v1_namespaced_deployment_status**](docs/AppsvApi.md#patch_apps_v1_namespaced_deployment_status) | **PATCH** /apis/apps/v1/namespaces/{namespace}/deployments/{name}/status | 
*AppsvApi* | [**patch_apps_v1_namespaced_replica_set**](docs/AppsvApi.md#patch_apps_v1_namespaced_replica_set) | **PATCH** /apis/apps/v1/namespaces/{namespace}/replicasets/{name} | 
*AppsvApi* | [**patch_apps_v1_namespaced_replica_set_scale**](docs/AppsvApi.md#patch_apps_v1_namespaced_replica_set_scale) | **PATCH** /apis/apps/v1/namespaces/{namespace}/replicasets/{name}/scale | 
*AppsvApi* | [**patch_apps_v1_namespaced_replica_set_status**](docs/AppsvApi.md#patch_apps_v1_namespaced_replica_set_status) | **PATCH** /apis/apps/v1/namespaces/{namespace}/replicasets/{name}/status | 
*AppsvApi* | [**patch_apps_v1_namespaced_stateful_set**](docs/AppsvApi.md#patch_apps_v1_namespaced_stateful_set) | **PATCH** /apis/apps/v1/namespaces/{namespace}/statefulsets/{name} | 
*AppsvApi* | [**patch_apps_v1_namespaced_stateful_set_scale**](docs/AppsvApi.md#patch_apps_v1_namespaced_stateful_set_scale) | **PATCH** /apis/apps/v1/namespaces/{namespace}/statefulsets/{name}/scale | 
*AppsvApi* | [**patch_apps_v1_namespaced_stateful_set_status**](docs/AppsvApi.md#patch_apps_v1_namespaced_stateful_set_status) | **PATCH** /apis/apps/v1/namespaces/{namespace}/statefulsets/{name}/status | 
*AppsvApi* | [**read_apps_v1_namespaced_controller_revision**](docs/AppsvApi.md#read_apps_v1_namespaced_controller_revision) | **GET** /apis/apps/v1/namespaces/{namespace}/controllerrevisions/{name} | 
*AppsvApi* | [**read_apps_v1_namespaced_daemon_set**](docs/AppsvApi.md#read_apps_v1_namespaced_daemon_set) | **GET** /apis/apps/v1/namespaces/{namespace}/daemonsets/{name} | 
*AppsvApi* | [**read_apps_v1_namespaced_daemon_set_status**](docs/AppsvApi.md#read_apps_v1_namespaced_daemon_set_status) | **GET** /apis/apps/v1/namespaces/{namespace}/daemonsets/{name}/status | 
*AppsvApi* | [**read_apps_v1_namespaced_deployment**](docs/AppsvApi.md#read_apps_v1_namespaced_deployment) | **GET** /apis/apps/v1/namespaces/{namespace}/deployments/{name} | 
*AppsvApi* | [**read_apps_v1_namespaced_deployment_scale**](docs/AppsvApi.md#read_apps_v1_namespaced_deployment_scale) | **GET** /apis/apps/v1/namespaces/{namespace}/deployments/{name}/scale | 
*AppsvApi* | [**read_apps_v1_namespaced_deployment_status**](docs/AppsvApi.md#read_apps_v1_namespaced_deployment_status) | **GET** /apis/apps/v1/namespaces/{namespace}/deployments/{name}/status | 
*AppsvApi* | [**read_apps_v1_namespaced_replica_set**](docs/AppsvApi.md#read_apps_v1_namespaced_replica_set) | **GET** /apis/apps/v1/namespaces/{namespace}/replicasets/{name} | 
*AppsvApi* | [**read_apps_v1_namespaced_replica_set_scale**](docs/AppsvApi.md#read_apps_v1_namespaced_replica_set_scale) | **GET** /apis/apps/v1/namespaces/{namespace}/replicasets/{name}/scale | 
*AppsvApi* | [**read_apps_v1_namespaced_replica_set_status**](docs/AppsvApi.md#read_apps_v1_namespaced_replica_set_status) | **GET** /apis/apps/v1/namespaces/{namespace}/replicasets/{name}/status | 
*AppsvApi* | [**read_apps_v1_namespaced_stateful_set**](docs/AppsvApi.md#read_apps_v1_namespaced_stateful_set) | **GET** /apis/apps/v1/namespaces/{namespace}/statefulsets/{name} | 
*AppsvApi* | [**read_apps_v1_namespaced_stateful_set_scale**](docs/AppsvApi.md#read_apps_v1_namespaced_stateful_set_scale) | **GET** /apis/apps/v1/namespaces/{namespace}/statefulsets/{name}/scale | 
*AppsvApi* | [**read_apps_v1_namespaced_stateful_set_status**](docs/AppsvApi.md#read_apps_v1_namespaced_stateful_set_status) | **GET** /apis/apps/v1/namespaces/{namespace}/statefulsets/{name}/status | 
*AppsvApi* | [**replace_apps_v1_namespaced_controller_revision**](docs/AppsvApi.md#replace_apps_v1_namespaced_controller_revision) | **PUT** /apis/apps/v1/namespaces/{namespace}/controllerrevisions/{name} | 
*AppsvApi* | [**replace_apps_v1_namespaced_daemon_set**](docs/AppsvApi.md#replace_apps_v1_namespaced_daemon_set) | **PUT** /apis/apps/v1/namespaces/{namespace}/daemonsets/{name} | 
*AppsvApi* | [**replace_apps_v1_namespaced_daemon_set_status**](docs/AppsvApi.md#replace_apps_v1_namespaced_daemon_set_status) | **PUT** /apis/apps/v1/namespaces/{namespace}/daemonsets/{name}/status | 
*AppsvApi* | [**replace_apps_v1_namespaced_deployment**](docs/AppsvApi.md#replace_apps_v1_namespaced_deployment) | **PUT** /apis/apps/v1/namespaces/{namespace}/deployments/{name} | 
*AppsvApi* | [**replace_apps_v1_namespaced_deployment_scale**](docs/AppsvApi.md#replace_apps_v1_namespaced_deployment_scale) | **PUT** /apis/apps/v1/namespaces/{namespace}/deployments/{name}/scale | 
*AppsvApi* | [**replace_apps_v1_namespaced_deployment_status**](docs/AppsvApi.md#replace_apps_v1_namespaced_deployment_status) | **PUT** /apis/apps/v1/namespaces/{namespace}/deployments/{name}/status | 
*AppsvApi* | [**replace_apps_v1_namespaced_replica_set**](docs/AppsvApi.md#replace_apps_v1_namespaced_replica_set) | **PUT** /apis/apps/v1/namespaces/{namespace}/replicasets/{name} | 
*AppsvApi* | [**replace_apps_v1_namespaced_replica_set_scale**](docs/AppsvApi.md#replace_apps_v1_namespaced_replica_set_scale) | **PUT** /apis/apps/v1/namespaces/{namespace}/replicasets/{name}/scale | 
*AppsvApi* | [**replace_apps_v1_namespaced_replica_set_status**](docs/AppsvApi.md#replace_apps_v1_namespaced_replica_set_status) | **PUT** /apis/apps/v1/namespaces/{namespace}/replicasets/{name}/status | 
*AppsvApi* | [**replace_apps_v1_namespaced_stateful_set**](docs/AppsvApi.md#replace_apps_v1_namespaced_stateful_set) | **PUT** /apis/apps/v1/namespaces/{namespace}/statefulsets/{name} | 
*AppsvApi* | [**replace_apps_v1_namespaced_stateful_set_scale**](docs/AppsvApi.md#replace_apps_v1_namespaced_stateful_set_scale) | **PUT** /apis/apps/v1/namespaces/{namespace}/statefulsets/{name}/scale | 
*AppsvApi* | [**replace_apps_v1_namespaced_stateful_set_status**](docs/AppsvApi.md#replace_apps_v1_namespaced_stateful_set_status) | **PUT** /apis/apps/v1/namespaces/{namespace}/statefulsets/{name}/status | 
*AppsvApi* | [**watch_apps_v1_controller_revision_list_for_all_namespaces**](docs/AppsvApi.md#watch_apps_v1_controller_revision_list_for_all_namespaces) | **GET** /apis/apps/v1/watch/controllerrevisions | 
*AppsvApi* | [**watch_apps_v1_daemon_set_list_for_all_namespaces**](docs/AppsvApi.md#watch_apps_v1_daemon_set_list_for_all_namespaces) | **GET** /apis/apps/v1/watch/daemonsets | 
*AppsvApi* | [**watch_apps_v1_deployment_list_for_all_namespaces**](docs/AppsvApi.md#watch_apps_v1_deployment_list_for_all_namespaces) | **GET** /apis/apps/v1/watch/deployments | 
*AppsvApi* | [**watch_apps_v1_namespaced_controller_revision**](docs/AppsvApi.md#watch_apps_v1_namespaced_controller_revision) | **GET** /apis/apps/v1/watch/namespaces/{namespace}/controllerrevisions/{name} | 
*AppsvApi* | [**watch_apps_v1_namespaced_controller_revision_list**](docs/AppsvApi.md#watch_apps_v1_namespaced_controller_revision_list) | **GET** /apis/apps/v1/watch/namespaces/{namespace}/controllerrevisions | 
*AppsvApi* | [**watch_apps_v1_namespaced_daemon_set**](docs/AppsvApi.md#watch_apps_v1_namespaced_daemon_set) | **GET** /apis/apps/v1/watch/namespaces/{namespace}/daemonsets/{name} | 
*AppsvApi* | [**watch_apps_v1_namespaced_daemon_set_list**](docs/AppsvApi.md#watch_apps_v1_namespaced_daemon_set_list) | **GET** /apis/apps/v1/watch/namespaces/{namespace}/daemonsets | 
*AppsvApi* | [**watch_apps_v1_namespaced_deployment**](docs/AppsvApi.md#watch_apps_v1_namespaced_deployment) | **GET** /apis/apps/v1/watch/namespaces/{namespace}/deployments/{name} | 
*AppsvApi* | [**watch_apps_v1_namespaced_deployment_list**](docs/AppsvApi.md#watch_apps_v1_namespaced_deployment_list) | **GET** /apis/apps/v1/watch/namespaces/{namespace}/deployments | 
*AppsvApi* | [**watch_apps_v1_namespaced_replica_set**](docs/AppsvApi.md#watch_apps_v1_namespaced_replica_set) | **GET** /apis/apps/v1/watch/namespaces/{namespace}/replicasets/{name} | 
*AppsvApi* | [**watch_apps_v1_namespaced_replica_set_list**](docs/AppsvApi.md#watch_apps_v1_namespaced_replica_set_list) | **GET** /apis/apps/v1/watch/namespaces/{namespace}/replicasets | 
*AppsvApi* | [**watch_apps_v1_namespaced_stateful_set**](docs/AppsvApi.md#watch_apps_v1_namespaced_stateful_set) | **GET** /apis/apps/v1/watch/namespaces/{namespace}/statefulsets/{name} | 
*AppsvApi* | [**watch_apps_v1_namespaced_stateful_set_list**](docs/AppsvApi.md#watch_apps_v1_namespaced_stateful_set_list) | **GET** /apis/apps/v1/watch/namespaces/{namespace}/statefulsets | 
*AppsvApi* | [**watch_apps_v1_replica_set_list_for_all_namespaces**](docs/AppsvApi.md#watch_apps_v1_replica_set_list_for_all_namespaces) | **GET** /apis/apps/v1/watch/replicasets | 
*AppsvApi* | [**watch_apps_v1_stateful_set_list_for_all_namespaces**](docs/AppsvApi.md#watch_apps_v1_stateful_set_list_for_all_namespaces) | **GET** /apis/apps/v1/watch/statefulsets | 
*AuthenticationApi* | [**get_authentication_api_group**](docs/AuthenticationApi.md#get_authentication_api_group) | **GET** /apis/authentication.k8s.io/ | 
*AuthenticationvApi* | [**create_authentication_v1_token_review**](docs/AuthenticationvApi.md#create_authentication_v1_token_review) | **POST** /apis/authentication.k8s.io/v1/tokenreviews | 
*AuthenticationvApi* | [**get_authentication_v1_api_resources**](docs/AuthenticationvApi.md#get_authentication_v1_api_resources) | **GET** /apis/authentication.k8s.io/v1/ | 
*AuthenticationvalphaApi* | [**create_authentication_v1alpha1_self_subject_review**](docs/AuthenticationvalphaApi.md#create_authentication_v1alpha1_self_subject_review) | **POST** /apis/authentication.k8s.io/v1alpha1/selfsubjectreviews | 
*AuthenticationvalphaApi* | [**get_authentication_v1alpha1_api_resources**](docs/AuthenticationvalphaApi.md#get_authentication_v1alpha1_api_resources) | **GET** /apis/authentication.k8s.io/v1alpha1/ | 
*AuthorizationApi* | [**get_authorization_api_group**](docs/AuthorizationApi.md#get_authorization_api_group) | **GET** /apis/authorization.k8s.io/ | 
*AuthorizationvApi* | [**create_authorization_v1_namespaced_local_subject_access_review**](docs/AuthorizationvApi.md#create_authorization_v1_namespaced_local_subject_access_review) | **POST** /apis/authorization.k8s.io/v1/namespaces/{namespace}/localsubjectaccessreviews | 
*AuthorizationvApi* | [**create_authorization_v1_self_subject_access_review**](docs/AuthorizationvApi.md#create_authorization_v1_self_subject_access_review) | **POST** /apis/authorization.k8s.io/v1/selfsubjectaccessreviews | 
*AuthorizationvApi* | [**create_authorization_v1_self_subject_rules_review**](docs/AuthorizationvApi.md#create_authorization_v1_self_subject_rules_review) | **POST** /apis/authorization.k8s.io/v1/selfsubjectrulesreviews | 
*AuthorizationvApi* | [**create_authorization_v1_subject_access_review**](docs/AuthorizationvApi.md#create_authorization_v1_subject_access_review) | **POST** /apis/authorization.k8s.io/v1/subjectaccessreviews | 
*AuthorizationvApi* | [**get_authorization_v1_api_resources**](docs/AuthorizationvApi.md#get_authorization_v1_api_resources) | **GET** /apis/authorization.k8s.io/v1/ | 
*AutoscalingApi* | [**get_autoscaling_api_group**](docs/AutoscalingApi.md#get_autoscaling_api_group) | **GET** /apis/autoscaling/ | 
*AutoscalingvApi* | [**create_autoscaling_v1_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#create_autoscaling_v1_namespaced_horizontal_pod_autoscaler) | **POST** /apis/autoscaling/v1/namespaces/{namespace}/horizontalpodautoscalers | 
*AutoscalingvApi* | [**create_autoscaling_v2_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#create_autoscaling_v2_namespaced_horizontal_pod_autoscaler) | **POST** /apis/autoscaling/v2/namespaces/{namespace}/horizontalpodautoscalers | 
*AutoscalingvApi* | [**delete_autoscaling_v1_collection_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#delete_autoscaling_v1_collection_namespaced_horizontal_pod_autoscaler) | **DELETE** /apis/autoscaling/v1/namespaces/{namespace}/horizontalpodautoscalers | 
*AutoscalingvApi* | [**delete_autoscaling_v1_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#delete_autoscaling_v1_namespaced_horizontal_pod_autoscaler) | **DELETE** /apis/autoscaling/v1/namespaces/{namespace}/horizontalpodautoscalers/{name} | 
*AutoscalingvApi* | [**delete_autoscaling_v2_collection_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#delete_autoscaling_v2_collection_namespaced_horizontal_pod_autoscaler) | **DELETE** /apis/autoscaling/v2/namespaces/{namespace}/horizontalpodautoscalers | 
*AutoscalingvApi* | [**delete_autoscaling_v2_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#delete_autoscaling_v2_namespaced_horizontal_pod_autoscaler) | **DELETE** /apis/autoscaling/v2/namespaces/{namespace}/horizontalpodautoscalers/{name} | 
*AutoscalingvApi* | [**get_autoscaling_v1_api_resources**](docs/AutoscalingvApi.md#get_autoscaling_v1_api_resources) | **GET** /apis/autoscaling/v1/ | 
*AutoscalingvApi* | [**get_autoscaling_v2_api_resources**](docs/AutoscalingvApi.md#get_autoscaling_v2_api_resources) | **GET** /apis/autoscaling/v2/ | 
*AutoscalingvApi* | [**list_autoscaling_v1_horizontal_pod_autoscaler_for_all_namespaces**](docs/AutoscalingvApi.md#list_autoscaling_v1_horizontal_pod_autoscaler_for_all_namespaces) | **GET** /apis/autoscaling/v1/horizontalpodautoscalers | 
*AutoscalingvApi* | [**list_autoscaling_v1_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#list_autoscaling_v1_namespaced_horizontal_pod_autoscaler) | **GET** /apis/autoscaling/v1/namespaces/{namespace}/horizontalpodautoscalers | 
*AutoscalingvApi* | [**list_autoscaling_v2_horizontal_pod_autoscaler_for_all_namespaces**](docs/AutoscalingvApi.md#list_autoscaling_v2_horizontal_pod_autoscaler_for_all_namespaces) | **GET** /apis/autoscaling/v2/horizontalpodautoscalers | 
*AutoscalingvApi* | [**list_autoscaling_v2_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#list_autoscaling_v2_namespaced_horizontal_pod_autoscaler) | **GET** /apis/autoscaling/v2/namespaces/{namespace}/horizontalpodautoscalers | 
*AutoscalingvApi* | [**patch_autoscaling_v1_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#patch_autoscaling_v1_namespaced_horizontal_pod_autoscaler) | **PATCH** /apis/autoscaling/v1/namespaces/{namespace}/horizontalpodautoscalers/{name} | 
*AutoscalingvApi* | [**patch_autoscaling_v1_namespaced_horizontal_pod_autoscaler_status**](docs/AutoscalingvApi.md#patch_autoscaling_v1_namespaced_horizontal_pod_autoscaler_status) | **PATCH** /apis/autoscaling/v1/namespaces/{namespace}/horizontalpodautoscalers/{name}/status | 
*AutoscalingvApi* | [**patch_autoscaling_v2_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#patch_autoscaling_v2_namespaced_horizontal_pod_autoscaler) | **PATCH** /apis/autoscaling/v2/namespaces/{namespace}/horizontalpodautoscalers/{name} | 
*AutoscalingvApi* | [**patch_autoscaling_v2_namespaced_horizontal_pod_autoscaler_status**](docs/AutoscalingvApi.md#patch_autoscaling_v2_namespaced_horizontal_pod_autoscaler_status) | **PATCH** /apis/autoscaling/v2/namespaces/{namespace}/horizontalpodautoscalers/{name}/status | 
*AutoscalingvApi* | [**read_autoscaling_v1_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#read_autoscaling_v1_namespaced_horizontal_pod_autoscaler) | **GET** /apis/autoscaling/v1/namespaces/{namespace}/horizontalpodautoscalers/{name} | 
*AutoscalingvApi* | [**read_autoscaling_v1_namespaced_horizontal_pod_autoscaler_status**](docs/AutoscalingvApi.md#read_autoscaling_v1_namespaced_horizontal_pod_autoscaler_status) | **GET** /apis/autoscaling/v1/namespaces/{namespace}/horizontalpodautoscalers/{name}/status | 
*AutoscalingvApi* | [**read_autoscaling_v2_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#read_autoscaling_v2_namespaced_horizontal_pod_autoscaler) | **GET** /apis/autoscaling/v2/namespaces/{namespace}/horizontalpodautoscalers/{name} | 
*AutoscalingvApi* | [**read_autoscaling_v2_namespaced_horizontal_pod_autoscaler_status**](docs/AutoscalingvApi.md#read_autoscaling_v2_namespaced_horizontal_pod_autoscaler_status) | **GET** /apis/autoscaling/v2/namespaces/{namespace}/horizontalpodautoscalers/{name}/status | 
*AutoscalingvApi* | [**replace_autoscaling_v1_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#replace_autoscaling_v1_namespaced_horizontal_pod_autoscaler) | **PUT** /apis/autoscaling/v1/namespaces/{namespace}/horizontalpodautoscalers/{name} | 
*AutoscalingvApi* | [**replace_autoscaling_v1_namespaced_horizontal_pod_autoscaler_status**](docs/AutoscalingvApi.md#replace_autoscaling_v1_namespaced_horizontal_pod_autoscaler_status) | **PUT** /apis/autoscaling/v1/namespaces/{namespace}/horizontalpodautoscalers/{name}/status | 
*AutoscalingvApi* | [**replace_autoscaling_v2_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#replace_autoscaling_v2_namespaced_horizontal_pod_autoscaler) | **PUT** /apis/autoscaling/v2/namespaces/{namespace}/horizontalpodautoscalers/{name} | 
*AutoscalingvApi* | [**replace_autoscaling_v2_namespaced_horizontal_pod_autoscaler_status**](docs/AutoscalingvApi.md#replace_autoscaling_v2_namespaced_horizontal_pod_autoscaler_status) | **PUT** /apis/autoscaling/v2/namespaces/{namespace}/horizontalpodautoscalers/{name}/status | 
*AutoscalingvApi* | [**watch_autoscaling_v1_horizontal_pod_autoscaler_list_for_all_namespaces**](docs/AutoscalingvApi.md#watch_autoscaling_v1_horizontal_pod_autoscaler_list_for_all_namespaces) | **GET** /apis/autoscaling/v1/watch/horizontalpodautoscalers | 
*AutoscalingvApi* | [**watch_autoscaling_v1_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#watch_autoscaling_v1_namespaced_horizontal_pod_autoscaler) | **GET** /apis/autoscaling/v1/watch/namespaces/{namespace}/horizontalpodautoscalers/{name} | 
*AutoscalingvApi* | [**watch_autoscaling_v1_namespaced_horizontal_pod_autoscaler_list**](docs/AutoscalingvApi.md#watch_autoscaling_v1_namespaced_horizontal_pod_autoscaler_list) | **GET** /apis/autoscaling/v1/watch/namespaces/{namespace}/horizontalpodautoscalers | 
*AutoscalingvApi* | [**watch_autoscaling_v2_horizontal_pod_autoscaler_list_for_all_namespaces**](docs/AutoscalingvApi.md#watch_autoscaling_v2_horizontal_pod_autoscaler_list_for_all_namespaces) | **GET** /apis/autoscaling/v2/watch/horizontalpodautoscalers | 
*AutoscalingvApi* | [**watch_autoscaling_v2_namespaced_horizontal_pod_autoscaler**](docs/AutoscalingvApi.md#watch_autoscaling_v2_namespaced_horizontal_pod_autoscaler) | **GET** /apis/autoscaling/v2/watch/namespaces/{namespace}/horizontalpodautoscalers/{name} | 
*AutoscalingvApi* | [**watch_autoscaling_v2_namespaced_horizontal_pod_autoscaler_list**](docs/AutoscalingvApi.md#watch_autoscaling_v2_namespaced_horizontal_pod_autoscaler_list) | **GET** /apis/autoscaling/v2/watch/namespaces/{namespace}/horizontalpodautoscalers | 
*BatchApi* | [**get_batch_api_group**](docs/BatchApi.md#get_batch_api_group) | **GET** /apis/batch/ | 
*BatchvApi* | [**create_batch_v1_namespaced_cron_job**](docs/BatchvApi.md#create_batch_v1_namespaced_cron_job) | **POST** /apis/batch/v1/namespaces/{namespace}/cronjobs | 
*BatchvApi* | [**create_batch_v1_namespaced_job**](docs/BatchvApi.md#create_batch_v1_namespaced_job) | **POST** /apis/batch/v1/namespaces/{namespace}/jobs | 
*BatchvApi* | [**delete_batch_v1_collection_namespaced_cron_job**](docs/BatchvApi.md#delete_batch_v1_collection_namespaced_cron_job) | **DELETE** /apis/batch/v1/namespaces/{namespace}/cronjobs | 
*BatchvApi* | [**delete_batch_v1_collection_namespaced_job**](docs/BatchvApi.md#delete_batch_v1_collection_namespaced_job) | **DELETE** /apis/batch/v1/namespaces/{namespace}/jobs | 
*BatchvApi* | [**delete_batch_v1_namespaced_cron_job**](docs/BatchvApi.md#delete_batch_v1_namespaced_cron_job) | **DELETE** /apis/batch/v1/namespaces/{namespace}/cronjobs/{name} | 
*BatchvApi* | [**delete_batch_v1_namespaced_job**](docs/BatchvApi.md#delete_batch_v1_namespaced_job) | **DELETE** /apis/batch/v1/namespaces/{namespace}/jobs/{name} | 
*BatchvApi* | [**get_batch_v1_api_resources**](docs/BatchvApi.md#get_batch_v1_api_resources) | **GET** /apis/batch/v1/ | 
*BatchvApi* | [**list_batch_v1_cron_job_for_all_namespaces**](docs/BatchvApi.md#list_batch_v1_cron_job_for_all_namespaces) | **GET** /apis/batch/v1/cronjobs | 
*BatchvApi* | [**list_batch_v1_job_for_all_namespaces**](docs/BatchvApi.md#list_batch_v1_job_for_all_namespaces) | **GET** /apis/batch/v1/jobs | 
*BatchvApi* | [**list_batch_v1_namespaced_cron_job**](docs/BatchvApi.md#list_batch_v1_namespaced_cron_job) | **GET** /apis/batch/v1/namespaces/{namespace}/cronjobs | 
*BatchvApi* | [**list_batch_v1_namespaced_job**](docs/BatchvApi.md#list_batch_v1_namespaced_job) | **GET** /apis/batch/v1/namespaces/{namespace}/jobs | 
*BatchvApi* | [**patch_batch_v1_namespaced_cron_job**](docs/BatchvApi.md#patch_batch_v1_namespaced_cron_job) | **PATCH** /apis/batch/v1/namespaces/{namespace}/cronjobs/{name} | 
*BatchvApi* | [**patch_batch_v1_namespaced_cron_job_status**](docs/BatchvApi.md#patch_batch_v1_namespaced_cron_job_status) | **PATCH** /apis/batch/v1/namespaces/{namespace}/cronjobs/{name}/status | 
*BatchvApi* | [**patch_batch_v1_namespaced_job**](docs/BatchvApi.md#patch_batch_v1_namespaced_job) | **PATCH** /apis/batch/v1/namespaces/{namespace}/jobs/{name} | 
*BatchvApi* | [**patch_batch_v1_namespaced_job_status**](docs/BatchvApi.md#patch_batch_v1_namespaced_job_status) | **PATCH** /apis/batch/v1/namespaces/{namespace}/jobs/{name}/status | 
*BatchvApi* | [**read_batch_v1_namespaced_cron_job**](docs/BatchvApi.md#read_batch_v1_namespaced_cron_job) | **GET** /apis/batch/v1/namespaces/{namespace}/cronjobs/{name} | 
*BatchvApi* | [**read_batch_v1_namespaced_cron_job_status**](docs/BatchvApi.md#read_batch_v1_namespaced_cron_job_status) | **GET** /apis/batch/v1/namespaces/{namespace}/cronjobs/{name}/status | 
*BatchvApi* | [**read_batch_v1_namespaced_job**](docs/BatchvApi.md#read_batch_v1_namespaced_job) | **GET** /apis/batch/v1/namespaces/{namespace}/jobs/{name} | 
*BatchvApi* | [**read_batch_v1_namespaced_job_status**](docs/BatchvApi.md#read_batch_v1_namespaced_job_status) | **GET** /apis/batch/v1/namespaces/{namespace}/jobs/{name}/status | 
*BatchvApi* | [**replace_batch_v1_namespaced_cron_job**](docs/BatchvApi.md#replace_batch_v1_namespaced_cron_job) | **PUT** /apis/batch/v1/namespaces/{namespace}/cronjobs/{name} | 
*BatchvApi* | [**replace_batch_v1_namespaced_cron_job_status**](docs/BatchvApi.md#replace_batch_v1_namespaced_cron_job_status) | **PUT** /apis/batch/v1/namespaces/{namespace}/cronjobs/{name}/status | 
*BatchvApi* | [**replace_batch_v1_namespaced_job**](docs/BatchvApi.md#replace_batch_v1_namespaced_job) | **PUT** /apis/batch/v1/namespaces/{namespace}/jobs/{name} | 
*BatchvApi* | [**replace_batch_v1_namespaced_job_status**](docs/BatchvApi.md#replace_batch_v1_namespaced_job_status) | **PUT** /apis/batch/v1/namespaces/{namespace}/jobs/{name}/status | 
*BatchvApi* | [**watch_batch_v1_cron_job_list_for_all_namespaces**](docs/BatchvApi.md#watch_batch_v1_cron_job_list_for_all_namespaces) | **GET** /apis/batch/v1/watch/cronjobs | 
*BatchvApi* | [**watch_batch_v1_job_list_for_all_namespaces**](docs/BatchvApi.md#watch_batch_v1_job_list_for_all_namespaces) | **GET** /apis/batch/v1/watch/jobs | 
*BatchvApi* | [**watch_batch_v1_namespaced_cron_job**](docs/BatchvApi.md#watch_batch_v1_namespaced_cron_job) | **GET** /apis/batch/v1/watch/namespaces/{namespace}/cronjobs/{name} | 
*BatchvApi* | [**watch_batch_v1_namespaced_cron_job_list**](docs/BatchvApi.md#watch_batch_v1_namespaced_cron_job_list) | **GET** /apis/batch/v1/watch/namespaces/{namespace}/cronjobs | 
*BatchvApi* | [**watch_batch_v1_namespaced_job**](docs/BatchvApi.md#watch_batch_v1_namespaced_job) | **GET** /apis/batch/v1/watch/namespaces/{namespace}/jobs/{name} | 
*BatchvApi* | [**watch_batch_v1_namespaced_job_list**](docs/BatchvApi.md#watch_batch_v1_namespaced_job_list) | **GET** /apis/batch/v1/watch/namespaces/{namespace}/jobs | 
*CertificatesApi* | [**get_certificates_api_group**](docs/CertificatesApi.md#get_certificates_api_group) | **GET** /apis/certificates.k8s.io/ | 
*CertificatesvApi* | [**create_certificates_v1_certificate_signing_request**](docs/CertificatesvApi.md#create_certificates_v1_certificate_signing_request) | **POST** /apis/certificates.k8s.io/v1/certificatesigningrequests | 
*CertificatesvApi* | [**delete_certificates_v1_certificate_signing_request**](docs/CertificatesvApi.md#delete_certificates_v1_certificate_signing_request) | **DELETE** /apis/certificates.k8s.io/v1/certificatesigningrequests/{name} | 
*CertificatesvApi* | [**delete_certificates_v1_collection_certificate_signing_request**](docs/CertificatesvApi.md#delete_certificates_v1_collection_certificate_signing_request) | **DELETE** /apis/certificates.k8s.io/v1/certificatesigningrequests | 
*CertificatesvApi* | [**get_certificates_v1_api_resources**](docs/CertificatesvApi.md#get_certificates_v1_api_resources) | **GET** /apis/certificates.k8s.io/v1/ | 
*CertificatesvApi* | [**list_certificates_v1_certificate_signing_request**](docs/CertificatesvApi.md#list_certificates_v1_certificate_signing_request) | **GET** /apis/certificates.k8s.io/v1/certificatesigningrequests | 
*CertificatesvApi* | [**patch_certificates_v1_certificate_signing_request**](docs/CertificatesvApi.md#patch_certificates_v1_certificate_signing_request) | **PATCH** /apis/certificates.k8s.io/v1/certificatesigningrequests/{name} | 
*CertificatesvApi* | [**patch_certificates_v1_certificate_signing_request_approval**](docs/CertificatesvApi.md#patch_certificates_v1_certificate_signing_request_approval) | **PATCH** /apis/certificates.k8s.io/v1/certificatesigningrequests/{name}/approval | 
*CertificatesvApi* | [**patch_certificates_v1_certificate_signing_request_status**](docs/CertificatesvApi.md#patch_certificates_v1_certificate_signing_request_status) | **PATCH** /apis/certificates.k8s.io/v1/certificatesigningrequests/{name}/status | 
*CertificatesvApi* | [**read_certificates_v1_certificate_signing_request**](docs/CertificatesvApi.md#read_certificates_v1_certificate_signing_request) | **GET** /apis/certificates.k8s.io/v1/certificatesigningrequests/{name} | 
*CertificatesvApi* | [**read_certificates_v1_certificate_signing_request_approval**](docs/CertificatesvApi.md#read_certificates_v1_certificate_signing_request_approval) | **GET** /apis/certificates.k8s.io/v1/certificatesigningrequests/{name}/approval | 
*CertificatesvApi* | [**read_certificates_v1_certificate_signing_request_status**](docs/CertificatesvApi.md#read_certificates_v1_certificate_signing_request_status) | **GET** /apis/certificates.k8s.io/v1/certificatesigningrequests/{name}/status | 
*CertificatesvApi* | [**replace_certificates_v1_certificate_signing_request**](docs/CertificatesvApi.md#replace_certificates_v1_certificate_signing_request) | **PUT** /apis/certificates.k8s.io/v1/certificatesigningrequests/{name} | 
*CertificatesvApi* | [**replace_certificates_v1_certificate_signing_request_approval**](docs/CertificatesvApi.md#replace_certificates_v1_certificate_signing_request_approval) | **PUT** /apis/certificates.k8s.io/v1/certificatesigningrequests/{name}/approval | 
*CertificatesvApi* | [**replace_certificates_v1_certificate_signing_request_status**](docs/CertificatesvApi.md#replace_certificates_v1_certificate_signing_request_status) | **PUT** /apis/certificates.k8s.io/v1/certificatesigningrequests/{name}/status | 
*CertificatesvApi* | [**watch_certificates_v1_certificate_signing_request**](docs/CertificatesvApi.md#watch_certificates_v1_certificate_signing_request) | **GET** /apis/certificates.k8s.io/v1/watch/certificatesigningrequests/{name} | 
*CertificatesvApi* | [**watch_certificates_v1_certificate_signing_request_list**](docs/CertificatesvApi.md#watch_certificates_v1_certificate_signing_request_list) | **GET** /apis/certificates.k8s.io/v1/watch/certificatesigningrequests | 
*CoordinationApi* | [**get_coordination_api_group**](docs/CoordinationApi.md#get_coordination_api_group) | **GET** /apis/coordination.k8s.io/ | 
*CoordinationvApi* | [**create_coordination_v1_namespaced_lease**](docs/CoordinationvApi.md#create_coordination_v1_namespaced_lease) | **POST** /apis/coordination.k8s.io/v1/namespaces/{namespace}/leases | 
*CoordinationvApi* | [**delete_coordination_v1_collection_namespaced_lease**](docs/CoordinationvApi.md#delete_coordination_v1_collection_namespaced_lease) | **DELETE** /apis/coordination.k8s.io/v1/namespaces/{namespace}/leases | 
*CoordinationvApi* | [**delete_coordination_v1_namespaced_lease**](docs/CoordinationvApi.md#delete_coordination_v1_namespaced_lease) | **DELETE** /apis/coordination.k8s.io/v1/namespaces/{namespace}/leases/{name} | 
*CoordinationvApi* | [**get_coordination_v1_api_resources**](docs/CoordinationvApi.md#get_coordination_v1_api_resources) | **GET** /apis/coordination.k8s.io/v1/ | 
*CoordinationvApi* | [**list_coordination_v1_lease_for_all_namespaces**](docs/CoordinationvApi.md#list_coordination_v1_lease_for_all_namespaces) | **GET** /apis/coordination.k8s.io/v1/leases | 
*CoordinationvApi* | [**list_coordination_v1_namespaced_lease**](docs/CoordinationvApi.md#list_coordination_v1_namespaced_lease) | **GET** /apis/coordination.k8s.io/v1/namespaces/{namespace}/leases | 
*CoordinationvApi* | [**patch_coordination_v1_namespaced_lease**](docs/CoordinationvApi.md#patch_coordination_v1_namespaced_lease) | **PATCH** /apis/coordination.k8s.io/v1/namespaces/{namespace}/leases/{name} | 
*CoordinationvApi* | [**read_coordination_v1_namespaced_lease**](docs/CoordinationvApi.md#read_coordination_v1_namespaced_lease) | **GET** /apis/coordination.k8s.io/v1/namespaces/{namespace}/leases/{name} | 
*CoordinationvApi* | [**replace_coordination_v1_namespaced_lease**](docs/CoordinationvApi.md#replace_coordination_v1_namespaced_lease) | **PUT** /apis/coordination.k8s.io/v1/namespaces/{namespace}/leases/{name} | 
*CoordinationvApi* | [**watch_coordination_v1_lease_list_for_all_namespaces**](docs/CoordinationvApi.md#watch_coordination_v1_lease_list_for_all_namespaces) | **GET** /apis/coordination.k8s.io/v1/watch/leases | 
*CoordinationvApi* | [**watch_coordination_v1_namespaced_lease**](docs/CoordinationvApi.md#watch_coordination_v1_namespaced_lease) | **GET** /apis/coordination.k8s.io/v1/watch/namespaces/{namespace}/leases/{name} | 
*CoordinationvApi* | [**watch_coordination_v1_namespaced_lease_list**](docs/CoordinationvApi.md#watch_coordination_v1_namespaced_lease_list) | **GET** /apis/coordination.k8s.io/v1/watch/namespaces/{namespace}/leases | 
*CoreApi* | [**get_core_api_versions**](docs/CoreApi.md#get_core_api_versions) | **GET** /api/ | 
*CorevApi* | [**connect_core_v1_delete_namespaced_pod_proxy**](docs/CorevApi.md#connect_core_v1_delete_namespaced_pod_proxy) | **DELETE** /api/v1/namespaces/{namespace}/pods/{name}/proxy | 
*CorevApi* | [**connect_core_v1_delete_namespaced_pod_proxy_with_path**](docs/CorevApi.md#connect_core_v1_delete_namespaced_pod_proxy_with_path) | **DELETE** /api/v1/namespaces/{namespace}/pods/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_delete_namespaced_service_proxy**](docs/CorevApi.md#connect_core_v1_delete_namespaced_service_proxy) | **DELETE** /api/v1/namespaces/{namespace}/services/{name}/proxy | 
*CorevApi* | [**connect_core_v1_delete_namespaced_service_proxy_with_path**](docs/CorevApi.md#connect_core_v1_delete_namespaced_service_proxy_with_path) | **DELETE** /api/v1/namespaces/{namespace}/services/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_delete_node_proxy**](docs/CorevApi.md#connect_core_v1_delete_node_proxy) | **DELETE** /api/v1/nodes/{name}/proxy | 
*CorevApi* | [**connect_core_v1_delete_node_proxy_with_path**](docs/CorevApi.md#connect_core_v1_delete_node_proxy_with_path) | **DELETE** /api/v1/nodes/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_get_namespaced_pod_attach**](docs/CorevApi.md#connect_core_v1_get_namespaced_pod_attach) | **GET** /api/v1/namespaces/{namespace}/pods/{name}/attach | 
*CorevApi* | [**connect_core_v1_get_namespaced_pod_exec**](docs/CorevApi.md#connect_core_v1_get_namespaced_pod_exec) | **GET** /api/v1/namespaces/{namespace}/pods/{name}/exec | 
*CorevApi* | [**connect_core_v1_get_namespaced_pod_portforward**](docs/CorevApi.md#connect_core_v1_get_namespaced_pod_portforward) | **GET** /api/v1/namespaces/{namespace}/pods/{name}/portforward | 
*CorevApi* | [**connect_core_v1_get_namespaced_pod_proxy**](docs/CorevApi.md#connect_core_v1_get_namespaced_pod_proxy) | **GET** /api/v1/namespaces/{namespace}/pods/{name}/proxy | 
*CorevApi* | [**connect_core_v1_get_namespaced_pod_proxy_with_path**](docs/CorevApi.md#connect_core_v1_get_namespaced_pod_proxy_with_path) | **GET** /api/v1/namespaces/{namespace}/pods/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_get_namespaced_service_proxy**](docs/CorevApi.md#connect_core_v1_get_namespaced_service_proxy) | **GET** /api/v1/namespaces/{namespace}/services/{name}/proxy | 
*CorevApi* | [**connect_core_v1_get_namespaced_service_proxy_with_path**](docs/CorevApi.md#connect_core_v1_get_namespaced_service_proxy_with_path) | **GET** /api/v1/namespaces/{namespace}/services/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_get_node_proxy**](docs/CorevApi.md#connect_core_v1_get_node_proxy) | **GET** /api/v1/nodes/{name}/proxy | 
*CorevApi* | [**connect_core_v1_get_node_proxy_with_path**](docs/CorevApi.md#connect_core_v1_get_node_proxy_with_path) | **GET** /api/v1/nodes/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_head_namespaced_pod_proxy**](docs/CorevApi.md#connect_core_v1_head_namespaced_pod_proxy) | **HEAD** /api/v1/namespaces/{namespace}/pods/{name}/proxy | 
*CorevApi* | [**connect_core_v1_head_namespaced_pod_proxy_with_path**](docs/CorevApi.md#connect_core_v1_head_namespaced_pod_proxy_with_path) | **HEAD** /api/v1/namespaces/{namespace}/pods/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_head_namespaced_service_proxy**](docs/CorevApi.md#connect_core_v1_head_namespaced_service_proxy) | **HEAD** /api/v1/namespaces/{namespace}/services/{name}/proxy | 
*CorevApi* | [**connect_core_v1_head_namespaced_service_proxy_with_path**](docs/CorevApi.md#connect_core_v1_head_namespaced_service_proxy_with_path) | **HEAD** /api/v1/namespaces/{namespace}/services/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_head_node_proxy**](docs/CorevApi.md#connect_core_v1_head_node_proxy) | **HEAD** /api/v1/nodes/{name}/proxy | 
*CorevApi* | [**connect_core_v1_head_node_proxy_with_path**](docs/CorevApi.md#connect_core_v1_head_node_proxy_with_path) | **HEAD** /api/v1/nodes/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_options_namespaced_pod_proxy**](docs/CorevApi.md#connect_core_v1_options_namespaced_pod_proxy) | **OPTIONS** /api/v1/namespaces/{namespace}/pods/{name}/proxy | 
*CorevApi* | [**connect_core_v1_options_namespaced_pod_proxy_with_path**](docs/CorevApi.md#connect_core_v1_options_namespaced_pod_proxy_with_path) | **OPTIONS** /api/v1/namespaces/{namespace}/pods/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_options_namespaced_service_proxy**](docs/CorevApi.md#connect_core_v1_options_namespaced_service_proxy) | **OPTIONS** /api/v1/namespaces/{namespace}/services/{name}/proxy | 
*CorevApi* | [**connect_core_v1_options_namespaced_service_proxy_with_path**](docs/CorevApi.md#connect_core_v1_options_namespaced_service_proxy_with_path) | **OPTIONS** /api/v1/namespaces/{namespace}/services/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_options_node_proxy**](docs/CorevApi.md#connect_core_v1_options_node_proxy) | **OPTIONS** /api/v1/nodes/{name}/proxy | 
*CorevApi* | [**connect_core_v1_options_node_proxy_with_path**](docs/CorevApi.md#connect_core_v1_options_node_proxy_with_path) | **OPTIONS** /api/v1/nodes/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_patch_namespaced_pod_proxy**](docs/CorevApi.md#connect_core_v1_patch_namespaced_pod_proxy) | **PATCH** /api/v1/namespaces/{namespace}/pods/{name}/proxy | 
*CorevApi* | [**connect_core_v1_patch_namespaced_pod_proxy_with_path**](docs/CorevApi.md#connect_core_v1_patch_namespaced_pod_proxy_with_path) | **PATCH** /api/v1/namespaces/{namespace}/pods/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_patch_namespaced_service_proxy**](docs/CorevApi.md#connect_core_v1_patch_namespaced_service_proxy) | **PATCH** /api/v1/namespaces/{namespace}/services/{name}/proxy | 
*CorevApi* | [**connect_core_v1_patch_namespaced_service_proxy_with_path**](docs/CorevApi.md#connect_core_v1_patch_namespaced_service_proxy_with_path) | **PATCH** /api/v1/namespaces/{namespace}/services/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_patch_node_proxy**](docs/CorevApi.md#connect_core_v1_patch_node_proxy) | **PATCH** /api/v1/nodes/{name}/proxy | 
*CorevApi* | [**connect_core_v1_patch_node_proxy_with_path**](docs/CorevApi.md#connect_core_v1_patch_node_proxy_with_path) | **PATCH** /api/v1/nodes/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_post_namespaced_pod_attach**](docs/CorevApi.md#connect_core_v1_post_namespaced_pod_attach) | **POST** /api/v1/namespaces/{namespace}/pods/{name}/attach | 
*CorevApi* | [**connect_core_v1_post_namespaced_pod_exec**](docs/CorevApi.md#connect_core_v1_post_namespaced_pod_exec) | **POST** /api/v1/namespaces/{namespace}/pods/{name}/exec | 
*CorevApi* | [**connect_core_v1_post_namespaced_pod_portforward**](docs/CorevApi.md#connect_core_v1_post_namespaced_pod_portforward) | **POST** /api/v1/namespaces/{namespace}/pods/{name}/portforward | 
*CorevApi* | [**connect_core_v1_post_namespaced_pod_proxy**](docs/CorevApi.md#connect_core_v1_post_namespaced_pod_proxy) | **POST** /api/v1/namespaces/{namespace}/pods/{name}/proxy | 
*CorevApi* | [**connect_core_v1_post_namespaced_pod_proxy_with_path**](docs/CorevApi.md#connect_core_v1_post_namespaced_pod_proxy_with_path) | **POST** /api/v1/namespaces/{namespace}/pods/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_post_namespaced_service_proxy**](docs/CorevApi.md#connect_core_v1_post_namespaced_service_proxy) | **POST** /api/v1/namespaces/{namespace}/services/{name}/proxy | 
*CorevApi* | [**connect_core_v1_post_namespaced_service_proxy_with_path**](docs/CorevApi.md#connect_core_v1_post_namespaced_service_proxy_with_path) | **POST** /api/v1/namespaces/{namespace}/services/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_post_node_proxy**](docs/CorevApi.md#connect_core_v1_post_node_proxy) | **POST** /api/v1/nodes/{name}/proxy | 
*CorevApi* | [**connect_core_v1_post_node_proxy_with_path**](docs/CorevApi.md#connect_core_v1_post_node_proxy_with_path) | **POST** /api/v1/nodes/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_put_namespaced_pod_proxy**](docs/CorevApi.md#connect_core_v1_put_namespaced_pod_proxy) | **PUT** /api/v1/namespaces/{namespace}/pods/{name}/proxy | 
*CorevApi* | [**connect_core_v1_put_namespaced_pod_proxy_with_path**](docs/CorevApi.md#connect_core_v1_put_namespaced_pod_proxy_with_path) | **PUT** /api/v1/namespaces/{namespace}/pods/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_put_namespaced_service_proxy**](docs/CorevApi.md#connect_core_v1_put_namespaced_service_proxy) | **PUT** /api/v1/namespaces/{namespace}/services/{name}/proxy | 
*CorevApi* | [**connect_core_v1_put_namespaced_service_proxy_with_path**](docs/CorevApi.md#connect_core_v1_put_namespaced_service_proxy_with_path) | **PUT** /api/v1/namespaces/{namespace}/services/{name}/proxy/{path} | 
*CorevApi* | [**connect_core_v1_put_node_proxy**](docs/CorevApi.md#connect_core_v1_put_node_proxy) | **PUT** /api/v1/nodes/{name}/proxy | 
*CorevApi* | [**connect_core_v1_put_node_proxy_with_path**](docs/CorevApi.md#connect_core_v1_put_node_proxy_with_path) | **PUT** /api/v1/nodes/{name}/proxy/{path} | 
*CorevApi* | [**create_core_v1_namespace**](docs/CorevApi.md#create_core_v1_namespace) | **POST** /api/v1/namespaces | 
*CorevApi* | [**create_core_v1_namespaced_binding**](docs/CorevApi.md#create_core_v1_namespaced_binding) | **POST** /api/v1/namespaces/{namespace}/bindings | 
*CorevApi* | [**create_core_v1_namespaced_config_map**](docs/CorevApi.md#create_core_v1_namespaced_config_map) | **POST** /api/v1/namespaces/{namespace}/configmaps | 
*CorevApi* | [**create_core_v1_namespaced_endpoints**](docs/CorevApi.md#create_core_v1_namespaced_endpoints) | **POST** /api/v1/namespaces/{namespace}/endpoints | 
*CorevApi* | [**create_core_v1_namespaced_event**](docs/CorevApi.md#create_core_v1_namespaced_event) | **POST** /api/v1/namespaces/{namespace}/events | 
*CorevApi* | [**create_core_v1_namespaced_limit_range**](docs/CorevApi.md#create_core_v1_namespaced_limit_range) | **POST** /api/v1/namespaces/{namespace}/limitranges | 
*CorevApi* | [**create_core_v1_namespaced_persistent_volume_claim**](docs/CorevApi.md#create_core_v1_namespaced_persistent_volume_claim) | **POST** /api/v1/namespaces/{namespace}/persistentvolumeclaims | 
*CorevApi* | [**create_core_v1_namespaced_pod**](docs/CorevApi.md#create_core_v1_namespaced_pod) | **POST** /api/v1/namespaces/{namespace}/pods | 
*CorevApi* | [**create_core_v1_namespaced_pod_binding**](docs/CorevApi.md#create_core_v1_namespaced_pod_binding) | **POST** /api/v1/namespaces/{namespace}/pods/{name}/binding | 
*CorevApi* | [**create_core_v1_namespaced_pod_eviction**](docs/CorevApi.md#create_core_v1_namespaced_pod_eviction) | **POST** /api/v1/namespaces/{namespace}/pods/{name}/eviction | 
*CorevApi* | [**create_core_v1_namespaced_pod_template**](docs/CorevApi.md#create_core_v1_namespaced_pod_template) | **POST** /api/v1/namespaces/{namespace}/podtemplates | 
*CorevApi* | [**create_core_v1_namespaced_replication_controller**](docs/CorevApi.md#create_core_v1_namespaced_replication_controller) | **POST** /api/v1/namespaces/{namespace}/replicationcontrollers | 
*CorevApi* | [**create_core_v1_namespaced_resource_quota**](docs/CorevApi.md#create_core_v1_namespaced_resource_quota) | **POST** /api/v1/namespaces/{namespace}/resourcequotas | 
*CorevApi* | [**create_core_v1_namespaced_secret**](docs/CorevApi.md#create_core_v1_namespaced_secret) | **POST** /api/v1/namespaces/{namespace}/secrets | 
*CorevApi* | [**create_core_v1_namespaced_service**](docs/CorevApi.md#create_core_v1_namespaced_service) | **POST** /api/v1/namespaces/{namespace}/services | 
*CorevApi* | [**create_core_v1_namespaced_service_account**](docs/CorevApi.md#create_core_v1_namespaced_service_account) | **POST** /api/v1/namespaces/{namespace}/serviceaccounts | 
*CorevApi* | [**create_core_v1_namespaced_service_account_token**](docs/CorevApi.md#create_core_v1_namespaced_service_account_token) | **POST** /api/v1/namespaces/{namespace}/serviceaccounts/{name}/token | 
*CorevApi* | [**create_core_v1_node**](docs/CorevApi.md#create_core_v1_node) | **POST** /api/v1/nodes | 
*CorevApi* | [**create_core_v1_persistent_volume**](docs/CorevApi.md#create_core_v1_persistent_volume) | **POST** /api/v1/persistentvolumes | 
*CorevApi* | [**delete_core_v1_collection_namespaced_config_map**](docs/CorevApi.md#delete_core_v1_collection_namespaced_config_map) | **DELETE** /api/v1/namespaces/{namespace}/configmaps | 
*CorevApi* | [**delete_core_v1_collection_namespaced_endpoints**](docs/CorevApi.md#delete_core_v1_collection_namespaced_endpoints) | **DELETE** /api/v1/namespaces/{namespace}/endpoints | 
*CorevApi* | [**delete_core_v1_collection_namespaced_event**](docs/CorevApi.md#delete_core_v1_collection_namespaced_event) | **DELETE** /api/v1/namespaces/{namespace}/events | 
*CorevApi* | [**delete_core_v1_collection_namespaced_limit_range**](docs/CorevApi.md#delete_core_v1_collection_namespaced_limit_range) | **DELETE** /api/v1/namespaces/{namespace}/limitranges | 
*CorevApi* | [**delete_core_v1_collection_namespaced_persistent_volume_claim**](docs/CorevApi.md#delete_core_v1_collection_namespaced_persistent_volume_claim) | **DELETE** /api/v1/namespaces/{namespace}/persistentvolumeclaims | 
*CorevApi* | [**delete_core_v1_collection_namespaced_pod**](docs/CorevApi.md#delete_core_v1_collection_namespaced_pod) | **DELETE** /api/v1/namespaces/{namespace}/pods | 
*CorevApi* | [**delete_core_v1_collection_namespaced_pod_template**](docs/CorevApi.md#delete_core_v1_collection_namespaced_pod_template) | **DELETE** /api/v1/namespaces/{namespace}/podtemplates | 
*CorevApi* | [**delete_core_v1_collection_namespaced_replication_controller**](docs/CorevApi.md#delete_core_v1_collection_namespaced_replication_controller) | **DELETE** /api/v1/namespaces/{namespace}/replicationcontrollers | 
*CorevApi* | [**delete_core_v1_collection_namespaced_resource_quota**](docs/CorevApi.md#delete_core_v1_collection_namespaced_resource_quota) | **DELETE** /api/v1/namespaces/{namespace}/resourcequotas | 
*CorevApi* | [**delete_core_v1_collection_namespaced_secret**](docs/CorevApi.md#delete_core_v1_collection_namespaced_secret) | **DELETE** /api/v1/namespaces/{namespace}/secrets | 
*CorevApi* | [**delete_core_v1_collection_namespaced_service**](docs/CorevApi.md#delete_core_v1_collection_namespaced_service) | **DELETE** /api/v1/namespaces/{namespace}/services | 
*CorevApi* | [**delete_core_v1_collection_namespaced_service_account**](docs/CorevApi.md#delete_core_v1_collection_namespaced_service_account) | **DELETE** /api/v1/namespaces/{namespace}/serviceaccounts | 
*CorevApi* | [**delete_core_v1_collection_node**](docs/CorevApi.md#delete_core_v1_collection_node) | **DELETE** /api/v1/nodes | 
*CorevApi* | [**delete_core_v1_collection_persistent_volume**](docs/CorevApi.md#delete_core_v1_collection_persistent_volume) | **DELETE** /api/v1/persistentvolumes | 
*CorevApi* | [**delete_core_v1_namespace**](docs/CorevApi.md#delete_core_v1_namespace) | **DELETE** /api/v1/namespaces/{name} | 
*CorevApi* | [**delete_core_v1_namespaced_config_map**](docs/CorevApi.md#delete_core_v1_namespaced_config_map) | **DELETE** /api/v1/namespaces/{namespace}/configmaps/{name} | 
*CorevApi* | [**delete_core_v1_namespaced_endpoints**](docs/CorevApi.md#delete_core_v1_namespaced_endpoints) | **DELETE** /api/v1/namespaces/{namespace}/endpoints/{name} | 
*CorevApi* | [**delete_core_v1_namespaced_event**](docs/CorevApi.md#delete_core_v1_namespaced_event) | **DELETE** /api/v1/namespaces/{namespace}/events/{name} | 
*CorevApi* | [**delete_core_v1_namespaced_limit_range**](docs/CorevApi.md#delete_core_v1_namespaced_limit_range) | **DELETE** /api/v1/namespaces/{namespace}/limitranges/{name} | 
*CorevApi* | [**delete_core_v1_namespaced_persistent_volume_claim**](docs/CorevApi.md#delete_core_v1_namespaced_persistent_volume_claim) | **DELETE** /api/v1/namespaces/{namespace}/persistentvolumeclaims/{name} | 
*CorevApi* | [**delete_core_v1_namespaced_pod**](docs/CorevApi.md#delete_core_v1_namespaced_pod) | **DELETE** /api/v1/namespaces/{namespace}/pods/{name} | 
*CorevApi* | [**delete_core_v1_namespaced_pod_template**](docs/CorevApi.md#delete_core_v1_namespaced_pod_template) | **DELETE** /api/v1/namespaces/{namespace}/podtemplates/{name} | 
*CorevApi* | [**delete_core_v1_namespaced_replication_controller**](docs/CorevApi.md#delete_core_v1_namespaced_replication_controller) | **DELETE** /api/v1/namespaces/{namespace}/replicationcontrollers/{name} | 
*CorevApi* | [**delete_core_v1_namespaced_resource_quota**](docs/CorevApi.md#delete_core_v1_namespaced_resource_quota) | **DELETE** /api/v1/namespaces/{namespace}/resourcequotas/{name} | 
*CorevApi* | [**delete_core_v1_namespaced_secret**](docs/CorevApi.md#delete_core_v1_namespaced_secret) | **DELETE** /api/v1/namespaces/{namespace}/secrets/{name} | 
*CorevApi* | [**delete_core_v1_namespaced_service**](docs/CorevApi.md#delete_core_v1_namespaced_service) | **DELETE** /api/v1/namespaces/{namespace}/services/{name} | 
*CorevApi* | [**delete_core_v1_namespaced_service_account**](docs/CorevApi.md#delete_core_v1_namespaced_service_account) | **DELETE** /api/v1/namespaces/{namespace}/serviceaccounts/{name} | 
*CorevApi* | [**delete_core_v1_node**](docs/CorevApi.md#delete_core_v1_node) | **DELETE** /api/v1/nodes/{name} | 
*CorevApi* | [**delete_core_v1_persistent_volume**](docs/CorevApi.md#delete_core_v1_persistent_volume) | **DELETE** /api/v1/persistentvolumes/{name} | 
*CorevApi* | [**get_core_v1_api_resources**](docs/CorevApi.md#get_core_v1_api_resources) | **GET** /api/v1/ | 
*CorevApi* | [**list_core_v1_component_status**](docs/CorevApi.md#list_core_v1_component_status) | **GET** /api/v1/componentstatuses | 
*CorevApi* | [**list_core_v1_config_map_for_all_namespaces**](docs/CorevApi.md#list_core_v1_config_map_for_all_namespaces) | **GET** /api/v1/configmaps | 
*CorevApi* | [**list_core_v1_endpoints_for_all_namespaces**](docs/CorevApi.md#list_core_v1_endpoints_for_all_namespaces) | **GET** /api/v1/endpoints | 
*CorevApi* | [**list_core_v1_event_for_all_namespaces**](docs/CorevApi.md#list_core_v1_event_for_all_namespaces) | **GET** /api/v1/events | 
*CorevApi* | [**list_core_v1_limit_range_for_all_namespaces**](docs/CorevApi.md#list_core_v1_limit_range_for_all_namespaces) | **GET** /api/v1/limitranges | 
*CorevApi* | [**list_core_v1_namespace**](docs/CorevApi.md#list_core_v1_namespace) | **GET** /api/v1/namespaces | 
*CorevApi* | [**list_core_v1_namespaced_config_map**](docs/CorevApi.md#list_core_v1_namespaced_config_map) | **GET** /api/v1/namespaces/{namespace}/configmaps | 
*CorevApi* | [**list_core_v1_namespaced_endpoints**](docs/CorevApi.md#list_core_v1_namespaced_endpoints) | **GET** /api/v1/namespaces/{namespace}/endpoints | 
*CorevApi* | [**list_core_v1_namespaced_event**](docs/CorevApi.md#list_core_v1_namespaced_event) | **GET** /api/v1/namespaces/{namespace}/events | 
*CorevApi* | [**list_core_v1_namespaced_limit_range**](docs/CorevApi.md#list_core_v1_namespaced_limit_range) | **GET** /api/v1/namespaces/{namespace}/limitranges | 
*CorevApi* | [**list_core_v1_namespaced_persistent_volume_claim**](docs/CorevApi.md#list_core_v1_namespaced_persistent_volume_claim) | **GET** /api/v1/namespaces/{namespace}/persistentvolumeclaims | 
*CorevApi* | [**list_core_v1_namespaced_pod**](docs/CorevApi.md#list_core_v1_namespaced_pod) | **GET** /api/v1/namespaces/{namespace}/pods | 
*CorevApi* | [**list_core_v1_namespaced_pod_template**](docs/CorevApi.md#list_core_v1_namespaced_pod_template) | **GET** /api/v1/namespaces/{namespace}/podtemplates | 
*CorevApi* | [**list_core_v1_namespaced_replication_controller**](docs/CorevApi.md#list_core_v1_namespaced_replication_controller) | **GET** /api/v1/namespaces/{namespace}/replicationcontrollers | 
*CorevApi* | [**list_core_v1_namespaced_resource_quota**](docs/CorevApi.md#list_core_v1_namespaced_resource_quota) | **GET** /api/v1/namespaces/{namespace}/resourcequotas | 
*CorevApi* | [**list_core_v1_namespaced_secret**](docs/CorevApi.md#list_core_v1_namespaced_secret) | **GET** /api/v1/namespaces/{namespace}/secrets | 
*CorevApi* | [**list_core_v1_namespaced_service**](docs/CorevApi.md#list_core_v1_namespaced_service) | **GET** /api/v1/namespaces/{namespace}/services | 
*CorevApi* | [**list_core_v1_namespaced_service_account**](docs/CorevApi.md#list_core_v1_namespaced_service_account) | **GET** /api/v1/namespaces/{namespace}/serviceaccounts | 
*CorevApi* | [**list_core_v1_node**](docs/CorevApi.md#list_core_v1_node) | **GET** /api/v1/nodes | 
*CorevApi* | [**list_core_v1_persistent_volume**](docs/CorevApi.md#list_core_v1_persistent_volume) | **GET** /api/v1/persistentvolumes | 
*CorevApi* | [**list_core_v1_persistent_volume_claim_for_all_namespaces**](docs/CorevApi.md#list_core_v1_persistent_volume_claim_for_all_namespaces) | **GET** /api/v1/persistentvolumeclaims | 
*CorevApi* | [**list_core_v1_pod_for_all_namespaces**](docs/CorevApi.md#list_core_v1_pod_for_all_namespaces) | **GET** /api/v1/pods | 
*CorevApi* | [**list_core_v1_pod_template_for_all_namespaces**](docs/CorevApi.md#list_core_v1_pod_template_for_all_namespaces) | **GET** /api/v1/podtemplates | 
*CorevApi* | [**list_core_v1_replication_controller_for_all_namespaces**](docs/CorevApi.md#list_core_v1_replication_controller_for_all_namespaces) | **GET** /api/v1/replicationcontrollers | 
*CorevApi* | [**list_core_v1_resource_quota_for_all_namespaces**](docs/CorevApi.md#list_core_v1_resource_quota_for_all_namespaces) | **GET** /api/v1/resourcequotas | 
*CorevApi* | [**list_core_v1_secret_for_all_namespaces**](docs/CorevApi.md#list_core_v1_secret_for_all_namespaces) | **GET** /api/v1/secrets | 
*CorevApi* | [**list_core_v1_service_account_for_all_namespaces**](docs/CorevApi.md#list_core_v1_service_account_for_all_namespaces) | **GET** /api/v1/serviceaccounts | 
*CorevApi* | [**list_core_v1_service_for_all_namespaces**](docs/CorevApi.md#list_core_v1_service_for_all_namespaces) | **GET** /api/v1/services | 
*CorevApi* | [**patch_core_v1_namespace**](docs/CorevApi.md#patch_core_v1_namespace) | **PATCH** /api/v1/namespaces/{name} | 
*CorevApi* | [**patch_core_v1_namespace_status**](docs/CorevApi.md#patch_core_v1_namespace_status) | **PATCH** /api/v1/namespaces/{name}/status | 
*CorevApi* | [**patch_core_v1_namespaced_config_map**](docs/CorevApi.md#patch_core_v1_namespaced_config_map) | **PATCH** /api/v1/namespaces/{namespace}/configmaps/{name} | 
*CorevApi* | [**patch_core_v1_namespaced_endpoints**](docs/CorevApi.md#patch_core_v1_namespaced_endpoints) | **PATCH** /api/v1/namespaces/{namespace}/endpoints/{name} | 
*CorevApi* | [**patch_core_v1_namespaced_event**](docs/CorevApi.md#patch_core_v1_namespaced_event) | **PATCH** /api/v1/namespaces/{namespace}/events/{name} | 
*CorevApi* | [**patch_core_v1_namespaced_limit_range**](docs/CorevApi.md#patch_core_v1_namespaced_limit_range) | **PATCH** /api/v1/namespaces/{namespace}/limitranges/{name} | 
*CorevApi* | [**patch_core_v1_namespaced_persistent_volume_claim**](docs/CorevApi.md#patch_core_v1_namespaced_persistent_volume_claim) | **PATCH** /api/v1/namespaces/{namespace}/persistentvolumeclaims/{name} | 
*CorevApi* | [**patch_core_v1_namespaced_persistent_volume_claim_status**](docs/CorevApi.md#patch_core_v1_namespaced_persistent_volume_claim_status) | **PATCH** /api/v1/namespaces/{namespace}/persistentvolumeclaims/{name}/status | 
*CorevApi* | [**patch_core_v1_namespaced_pod**](docs/CorevApi.md#patch_core_v1_namespaced_pod) | **PATCH** /api/v1/namespaces/{namespace}/pods/{name} | 
*CorevApi* | [**patch_core_v1_namespaced_pod_ephemeralcontainers**](docs/CorevApi.md#patch_core_v1_namespaced_pod_ephemeralcontainers) | **PATCH** /api/v1/namespaces/{namespace}/pods/{name}/ephemeralcontainers | 
*CorevApi* | [**patch_core_v1_namespaced_pod_status**](docs/CorevApi.md#patch_core_v1_namespaced_pod_status) | **PATCH** /api/v1/namespaces/{namespace}/pods/{name}/status | 
*CorevApi* | [**patch_core_v1_namespaced_pod_template**](docs/CorevApi.md#patch_core_v1_namespaced_pod_template) | **PATCH** /api/v1/namespaces/{namespace}/podtemplates/{name} | 
*CorevApi* | [**patch_core_v1_namespaced_replication_controller**](docs/CorevApi.md#patch_core_v1_namespaced_replication_controller) | **PATCH** /api/v1/namespaces/{namespace}/replicationcontrollers/{name} | 
*CorevApi* | [**patch_core_v1_namespaced_replication_controller_scale**](docs/CorevApi.md#patch_core_v1_namespaced_replication_controller_scale) | **PATCH** /api/v1/namespaces/{namespace}/replicationcontrollers/{name}/scale | 
*CorevApi* | [**patch_core_v1_namespaced_replication_controller_status**](docs/CorevApi.md#patch_core_v1_namespaced_replication_controller_status) | **PATCH** /api/v1/namespaces/{namespace}/replicationcontrollers/{name}/status | 
*CorevApi* | [**patch_core_v1_namespaced_resource_quota**](docs/CorevApi.md#patch_core_v1_namespaced_resource_quota) | **PATCH** /api/v1/namespaces/{namespace}/resourcequotas/{name} | 
*CorevApi* | [**patch_core_v1_namespaced_resource_quota_status**](docs/CorevApi.md#patch_core_v1_namespaced_resource_quota_status) | **PATCH** /api/v1/namespaces/{namespace}/resourcequotas/{name}/status | 
*CorevApi* | [**patch_core_v1_namespaced_secret**](docs/CorevApi.md#patch_core_v1_namespaced_secret) | **PATCH** /api/v1/namespaces/{namespace}/secrets/{name} | 
*CorevApi* | [**patch_core_v1_namespaced_service**](docs/CorevApi.md#patch_core_v1_namespaced_service) | **PATCH** /api/v1/namespaces/{namespace}/services/{name} | 
*CorevApi* | [**patch_core_v1_namespaced_service_account**](docs/CorevApi.md#patch_core_v1_namespaced_service_account) | **PATCH** /api/v1/namespaces/{namespace}/serviceaccounts/{name} | 
*CorevApi* | [**patch_core_v1_namespaced_service_status**](docs/CorevApi.md#patch_core_v1_namespaced_service_status) | **PATCH** /api/v1/namespaces/{namespace}/services/{name}/status | 
*CorevApi* | [**patch_core_v1_node**](docs/CorevApi.md#patch_core_v1_node) | **PATCH** /api/v1/nodes/{name} | 
*CorevApi* | [**patch_core_v1_node_status**](docs/CorevApi.md#patch_core_v1_node_status) | **PATCH** /api/v1/nodes/{name}/status | 
*CorevApi* | [**patch_core_v1_persistent_volume**](docs/CorevApi.md#patch_core_v1_persistent_volume) | **PATCH** /api/v1/persistentvolumes/{name} | 
*CorevApi* | [**patch_core_v1_persistent_volume_status**](docs/CorevApi.md#patch_core_v1_persistent_volume_status) | **PATCH** /api/v1/persistentvolumes/{name}/status | 
*CorevApi* | [**read_core_v1_component_status**](docs/CorevApi.md#read_core_v1_component_status) | **GET** /api/v1/componentstatuses/{name} | 
*CorevApi* | [**read_core_v1_namespace**](docs/CorevApi.md#read_core_v1_namespace) | **GET** /api/v1/namespaces/{name} | 
*CorevApi* | [**read_core_v1_namespace_status**](docs/CorevApi.md#read_core_v1_namespace_status) | **GET** /api/v1/namespaces/{name}/status | 
*CorevApi* | [**read_core_v1_namespaced_config_map**](docs/CorevApi.md#read_core_v1_namespaced_config_map) | **GET** /api/v1/namespaces/{namespace}/configmaps/{name} | 
*CorevApi* | [**read_core_v1_namespaced_endpoints**](docs/CorevApi.md#read_core_v1_namespaced_endpoints) | **GET** /api/v1/namespaces/{namespace}/endpoints/{name} | 
*CorevApi* | [**read_core_v1_namespaced_event**](docs/CorevApi.md#read_core_v1_namespaced_event) | **GET** /api/v1/namespaces/{namespace}/events/{name} | 
*CorevApi* | [**read_core_v1_namespaced_limit_range**](docs/CorevApi.md#read_core_v1_namespaced_limit_range) | **GET** /api/v1/namespaces/{namespace}/limitranges/{name} | 
*CorevApi* | [**read_core_v1_namespaced_persistent_volume_claim**](docs/CorevApi.md#read_core_v1_namespaced_persistent_volume_claim) | **GET** /api/v1/namespaces/{namespace}/persistentvolumeclaims/{name} | 
*CorevApi* | [**read_core_v1_namespaced_persistent_volume_claim_status**](docs/CorevApi.md#read_core_v1_namespaced_persistent_volume_claim_status) | **GET** /api/v1/namespaces/{namespace}/persistentvolumeclaims/{name}/status | 
*CorevApi* | [**read_core_v1_namespaced_pod**](docs/CorevApi.md#read_core_v1_namespaced_pod) | **GET** /api/v1/namespaces/{namespace}/pods/{name} | 
*CorevApi* | [**read_core_v1_namespaced_pod_ephemeralcontainers**](docs/CorevApi.md#read_core_v1_namespaced_pod_ephemeralcontainers) | **GET** /api/v1/namespaces/{namespace}/pods/{name}/ephemeralcontainers | 
*CorevApi* | [**read_core_v1_namespaced_pod_log**](docs/CorevApi.md#read_core_v1_namespaced_pod_log) | **GET** /api/v1/namespaces/{namespace}/pods/{name}/log | 
*CorevApi* | [**read_core_v1_namespaced_pod_status**](docs/CorevApi.md#read_core_v1_namespaced_pod_status) | **GET** /api/v1/namespaces/{namespace}/pods/{name}/status | 
*CorevApi* | [**read_core_v1_namespaced_pod_template**](docs/CorevApi.md#read_core_v1_namespaced_pod_template) | **GET** /api/v1/namespaces/{namespace}/podtemplates/{name} | 
*CorevApi* | [**read_core_v1_namespaced_replication_controller**](docs/CorevApi.md#read_core_v1_namespaced_replication_controller) | **GET** /api/v1/namespaces/{namespace}/replicationcontrollers/{name} | 
*CorevApi* | [**read_core_v1_namespaced_replication_controller_scale**](docs/CorevApi.md#read_core_v1_namespaced_replication_controller_scale) | **GET** /api/v1/namespaces/{namespace}/replicationcontrollers/{name}/scale | 
*CorevApi* | [**read_core_v1_namespaced_replication_controller_status**](docs/CorevApi.md#read_core_v1_namespaced_replication_controller_status) | **GET** /api/v1/namespaces/{namespace}/replicationcontrollers/{name}/status | 
*CorevApi* | [**read_core_v1_namespaced_resource_quota**](docs/CorevApi.md#read_core_v1_namespaced_resource_quota) | **GET** /api/v1/namespaces/{namespace}/resourcequotas/{name} | 
*CorevApi* | [**read_core_v1_namespaced_resource_quota_status**](docs/CorevApi.md#read_core_v1_namespaced_resource_quota_status) | **GET** /api/v1/namespaces/{namespace}/resourcequotas/{name}/status | 
*CorevApi* | [**read_core_v1_namespaced_secret**](docs/CorevApi.md#read_core_v1_namespaced_secret) | **GET** /api/v1/namespaces/{namespace}/secrets/{name} | 
*CorevApi* | [**read_core_v1_namespaced_service**](docs/CorevApi.md#read_core_v1_namespaced_service) | **GET** /api/v1/namespaces/{namespace}/services/{name} | 
*CorevApi* | [**read_core_v1_namespaced_service_account**](docs/CorevApi.md#read_core_v1_namespaced_service_account) | **GET** /api/v1/namespaces/{namespace}/serviceaccounts/{name} | 
*CorevApi* | [**read_core_v1_namespaced_service_status**](docs/CorevApi.md#read_core_v1_namespaced_service_status) | **GET** /api/v1/namespaces/{namespace}/services/{name}/status | 
*CorevApi* | [**read_core_v1_node**](docs/CorevApi.md#read_core_v1_node) | **GET** /api/v1/nodes/{name} | 
*CorevApi* | [**read_core_v1_node_status**](docs/CorevApi.md#read_core_v1_node_status) | **GET** /api/v1/nodes/{name}/status | 
*CorevApi* | [**read_core_v1_persistent_volume**](docs/CorevApi.md#read_core_v1_persistent_volume) | **GET** /api/v1/persistentvolumes/{name} | 
*CorevApi* | [**read_core_v1_persistent_volume_status**](docs/CorevApi.md#read_core_v1_persistent_volume_status) | **GET** /api/v1/persistentvolumes/{name}/status | 
*CorevApi* | [**replace_core_v1_namespace**](docs/CorevApi.md#replace_core_v1_namespace) | **PUT** /api/v1/namespaces/{name} | 
*CorevApi* | [**replace_core_v1_namespace_finalize**](docs/CorevApi.md#replace_core_v1_namespace_finalize) | **PUT** /api/v1/namespaces/{name}/finalize | 
*CorevApi* | [**replace_core_v1_namespace_status**](docs/CorevApi.md#replace_core_v1_namespace_status) | **PUT** /api/v1/namespaces/{name}/status | 
*CorevApi* | [**replace_core_v1_namespaced_config_map**](docs/CorevApi.md#replace_core_v1_namespaced_config_map) | **PUT** /api/v1/namespaces/{namespace}/configmaps/{name} | 
*CorevApi* | [**replace_core_v1_namespaced_endpoints**](docs/CorevApi.md#replace_core_v1_namespaced_endpoints) | **PUT** /api/v1/namespaces/{namespace}/endpoints/{name} | 
*CorevApi* | [**replace_core_v1_namespaced_event**](docs/CorevApi.md#replace_core_v1_namespaced_event) | **PUT** /api/v1/namespaces/{namespace}/events/{name} | 
*CorevApi* | [**replace_core_v1_namespaced_limit_range**](docs/CorevApi.md#replace_core_v1_namespaced_limit_range) | **PUT** /api/v1/namespaces/{namespace}/limitranges/{name} | 
*CorevApi* | [**replace_core_v1_namespaced_persistent_volume_claim**](docs/CorevApi.md#replace_core_v1_namespaced_persistent_volume_claim) | **PUT** /api/v1/namespaces/{namespace}/persistentvolumeclaims/{name} | 
*CorevApi* | [**replace_core_v1_namespaced_persistent_volume_claim_status**](docs/CorevApi.md#replace_core_v1_namespaced_persistent_volume_claim_status) | **PUT** /api/v1/namespaces/{namespace}/persistentvolumeclaims/{name}/status | 
*CorevApi* | [**replace_core_v1_namespaced_pod**](docs/CorevApi.md#replace_core_v1_namespaced_pod) | **PUT** /api/v1/namespaces/{namespace}/pods/{name} | 
*CorevApi* | [**replace_core_v1_namespaced_pod_ephemeralcontainers**](docs/CorevApi.md#replace_core_v1_namespaced_pod_ephemeralcontainers) | **PUT** /api/v1/namespaces/{namespace}/pods/{name}/ephemeralcontainers | 
*CorevApi* | [**replace_core_v1_namespaced_pod_status**](docs/CorevApi.md#replace_core_v1_namespaced_pod_status) | **PUT** /api/v1/namespaces/{namespace}/pods/{name}/status | 
*CorevApi* | [**replace_core_v1_namespaced_pod_template**](docs/CorevApi.md#replace_core_v1_namespaced_pod_template) | **PUT** /api/v1/namespaces/{namespace}/podtemplates/{name} | 
*CorevApi* | [**replace_core_v1_namespaced_replication_controller**](docs/CorevApi.md#replace_core_v1_namespaced_replication_controller) | **PUT** /api/v1/namespaces/{namespace}/replicationcontrollers/{name} | 
*CorevApi* | [**replace_core_v1_namespaced_replication_controller_scale**](docs/CorevApi.md#replace_core_v1_namespaced_replication_controller_scale) | **PUT** /api/v1/namespaces/{namespace}/replicationcontrollers/{name}/scale | 
*CorevApi* | [**replace_core_v1_namespaced_replication_controller_status**](docs/CorevApi.md#replace_core_v1_namespaced_replication_controller_status) | **PUT** /api/v1/namespaces/{namespace}/replicationcontrollers/{name}/status | 
*CorevApi* | [**replace_core_v1_namespaced_resource_quota**](docs/CorevApi.md#replace_core_v1_namespaced_resource_quota) | **PUT** /api/v1/namespaces/{namespace}/resourcequotas/{name} | 
*CorevApi* | [**replace_core_v1_namespaced_resource_quota_status**](docs/CorevApi.md#replace_core_v1_namespaced_resource_quota_status) | **PUT** /api/v1/namespaces/{namespace}/resourcequotas/{name}/status | 
*CorevApi* | [**replace_core_v1_namespaced_secret**](docs/CorevApi.md#replace_core_v1_namespaced_secret) | **PUT** /api/v1/namespaces/{namespace}/secrets/{name} | 
*CorevApi* | [**replace_core_v1_namespaced_service**](docs/CorevApi.md#replace_core_v1_namespaced_service) | **PUT** /api/v1/namespaces/{namespace}/services/{name} | 
*CorevApi* | [**replace_core_v1_namespaced_service_account**](docs/CorevApi.md#replace_core_v1_namespaced_service_account) | **PUT** /api/v1/namespaces/{namespace}/serviceaccounts/{name} | 
*CorevApi* | [**replace_core_v1_namespaced_service_status**](docs/CorevApi.md#replace_core_v1_namespaced_service_status) | **PUT** /api/v1/namespaces/{namespace}/services/{name}/status | 
*CorevApi* | [**replace_core_v1_node**](docs/CorevApi.md#replace_core_v1_node) | **PUT** /api/v1/nodes/{name} | 
*CorevApi* | [**replace_core_v1_node_status**](docs/CorevApi.md#replace_core_v1_node_status) | **PUT** /api/v1/nodes/{name}/status | 
*CorevApi* | [**replace_core_v1_persistent_volume**](docs/CorevApi.md#replace_core_v1_persistent_volume) | **PUT** /api/v1/persistentvolumes/{name} | 
*CorevApi* | [**replace_core_v1_persistent_volume_status**](docs/CorevApi.md#replace_core_v1_persistent_volume_status) | **PUT** /api/v1/persistentvolumes/{name}/status | 
*CorevApi* | [**watch_core_v1_config_map_list_for_all_namespaces**](docs/CorevApi.md#watch_core_v1_config_map_list_for_all_namespaces) | **GET** /api/v1/watch/configmaps | 
*CorevApi* | [**watch_core_v1_endpoints_list_for_all_namespaces**](docs/CorevApi.md#watch_core_v1_endpoints_list_for_all_namespaces) | **GET** /api/v1/watch/endpoints | 
*CorevApi* | [**watch_core_v1_event_list_for_all_namespaces**](docs/CorevApi.md#watch_core_v1_event_list_for_all_namespaces) | **GET** /api/v1/watch/events | 
*CorevApi* | [**watch_core_v1_limit_range_list_for_all_namespaces**](docs/CorevApi.md#watch_core_v1_limit_range_list_for_all_namespaces) | **GET** /api/v1/watch/limitranges | 
*CorevApi* | [**watch_core_v1_namespace**](docs/CorevApi.md#watch_core_v1_namespace) | **GET** /api/v1/watch/namespaces/{name} | 
*CorevApi* | [**watch_core_v1_namespace_list**](docs/CorevApi.md#watch_core_v1_namespace_list) | **GET** /api/v1/watch/namespaces | 
*CorevApi* | [**watch_core_v1_namespaced_config_map**](docs/CorevApi.md#watch_core_v1_namespaced_config_map) | **GET** /api/v1/watch/namespaces/{namespace}/configmaps/{name} | 
*CorevApi* | [**watch_core_v1_namespaced_config_map_list**](docs/CorevApi.md#watch_core_v1_namespaced_config_map_list) | **GET** /api/v1/watch/namespaces/{namespace}/configmaps | 
*CorevApi* | [**watch_core_v1_namespaced_endpoints**](docs/CorevApi.md#watch_core_v1_namespaced_endpoints) | **GET** /api/v1/watch/namespaces/{namespace}/endpoints/{name} | 
*CorevApi* | [**watch_core_v1_namespaced_endpoints_list**](docs/CorevApi.md#watch_core_v1_namespaced_endpoints_list) | **GET** /api/v1/watch/namespaces/{namespace}/endpoints | 
*CorevApi* | [**watch_core_v1_namespaced_event**](docs/CorevApi.md#watch_core_v1_namespaced_event) | **GET** /api/v1/watch/namespaces/{namespace}/events/{name} | 
*CorevApi* | [**watch_core_v1_namespaced_event_list**](docs/CorevApi.md#watch_core_v1_namespaced_event_list) | **GET** /api/v1/watch/namespaces/{namespace}/events | 
*CorevApi* | [**watch_core_v1_namespaced_limit_range**](docs/CorevApi.md#watch_core_v1_namespaced_limit_range) | **GET** /api/v1/watch/namespaces/{namespace}/limitranges/{name} | 
*CorevApi* | [**watch_core_v1_namespaced_limit_range_list**](docs/CorevApi.md#watch_core_v1_namespaced_limit_range_list) | **GET** /api/v1/watch/namespaces/{namespace}/limitranges | 
*CorevApi* | [**watch_core_v1_namespaced_persistent_volume_claim**](docs/CorevApi.md#watch_core_v1_namespaced_persistent_volume_claim) | **GET** /api/v1/watch/namespaces/{namespace}/persistentvolumeclaims/{name} | 
*CorevApi* | [**watch_core_v1_namespaced_persistent_volume_claim_list**](docs/CorevApi.md#watch_core_v1_namespaced_persistent_volume_claim_list) | **GET** /api/v1/watch/namespaces/{namespace}/persistentvolumeclaims | 
*CorevApi* | [**watch_core_v1_namespaced_pod**](docs/CorevApi.md#watch_core_v1_namespaced_pod) | **GET** /api/v1/watch/namespaces/{namespace}/pods/{name} | 
*CorevApi* | [**watch_core_v1_namespaced_pod_list**](docs/CorevApi.md#watch_core_v1_namespaced_pod_list) | **GET** /api/v1/watch/namespaces/{namespace}/pods | 
*CorevApi* | [**watch_core_v1_namespaced_pod_template**](docs/CorevApi.md#watch_core_v1_namespaced_pod_template) | **GET** /api/v1/watch/namespaces/{namespace}/podtemplates/{name} | 
*CorevApi* | [**watch_core_v1_namespaced_pod_template_list**](docs/CorevApi.md#watch_core_v1_namespaced_pod_template_list) | **GET** /api/v1/watch/namespaces/{namespace}/podtemplates | 
*CorevApi* | [**watch_core_v1_namespaced_replication_controller**](docs/CorevApi.md#watch_core_v1_namespaced_replication_controller) | **GET** /api/v1/watch/namespaces/{namespace}/replicationcontrollers/{name} | 
*CorevApi* | [**watch_core_v1_namespaced_replication_controller_list**](docs/CorevApi.md#watch_core_v1_namespaced_replication_controller_list) | **GET** /api/v1/watch/namespaces/{namespace}/replicationcontrollers | 
*CorevApi* | [**watch_core_v1_namespaced_resource_quota**](docs/CorevApi.md#watch_core_v1_namespaced_resource_quota) | **GET** /api/v1/watch/namespaces/{namespace}/resourcequotas/{name} | 
*CorevApi* | [**watch_core_v1_namespaced_resource_quota_list**](docs/CorevApi.md#watch_core_v1_namespaced_resource_quota_list) | **GET** /api/v1/watch/namespaces/{namespace}/resourcequotas | 
*CorevApi* | [**watch_core_v1_namespaced_secret**](docs/CorevApi.md#watch_core_v1_namespaced_secret) | **GET** /api/v1/watch/namespaces/{namespace}/secrets/{name} | 
*CorevApi* | [**watch_core_v1_namespaced_secret_list**](docs/CorevApi.md#watch_core_v1_namespaced_secret_list) | **GET** /api/v1/watch/namespaces/{namespace}/secrets | 
*CorevApi* | [**watch_core_v1_namespaced_service**](docs/CorevApi.md#watch_core_v1_namespaced_service) | **GET** /api/v1/watch/namespaces/{namespace}/services/{name} | 
*CorevApi* | [**watch_core_v1_namespaced_service_account**](docs/CorevApi.md#watch_core_v1_namespaced_service_account) | **GET** /api/v1/watch/namespaces/{namespace}/serviceaccounts/{name} | 
*CorevApi* | [**watch_core_v1_namespaced_service_account_list**](docs/CorevApi.md#watch_core_v1_namespaced_service_account_list) | **GET** /api/v1/watch/namespaces/{namespace}/serviceaccounts | 
*CorevApi* | [**watch_core_v1_namespaced_service_list**](docs/CorevApi.md#watch_core_v1_namespaced_service_list) | **GET** /api/v1/watch/namespaces/{namespace}/services | 
*CorevApi* | [**watch_core_v1_node**](docs/CorevApi.md#watch_core_v1_node) | **GET** /api/v1/watch/nodes/{name} | 
*CorevApi* | [**watch_core_v1_node_list**](docs/CorevApi.md#watch_core_v1_node_list) | **GET** /api/v1/watch/nodes | 
*CorevApi* | [**watch_core_v1_persistent_volume**](docs/CorevApi.md#watch_core_v1_persistent_volume) | **GET** /api/v1/watch/persistentvolumes/{name} | 
*CorevApi* | [**watch_core_v1_persistent_volume_claim_list_for_all_namespaces**](docs/CorevApi.md#watch_core_v1_persistent_volume_claim_list_for_all_namespaces) | **GET** /api/v1/watch/persistentvolumeclaims | 
*CorevApi* | [**watch_core_v1_persistent_volume_list**](docs/CorevApi.md#watch_core_v1_persistent_volume_list) | **GET** /api/v1/watch/persistentvolumes | 
*CorevApi* | [**watch_core_v1_pod_list_for_all_namespaces**](docs/CorevApi.md#watch_core_v1_pod_list_for_all_namespaces) | **GET** /api/v1/watch/pods | 
*CorevApi* | [**watch_core_v1_pod_template_list_for_all_namespaces**](docs/CorevApi.md#watch_core_v1_pod_template_list_for_all_namespaces) | **GET** /api/v1/watch/podtemplates | 
*CorevApi* | [**watch_core_v1_replication_controller_list_for_all_namespaces**](docs/CorevApi.md#watch_core_v1_replication_controller_list_for_all_namespaces) | **GET** /api/v1/watch/replicationcontrollers | 
*CorevApi* | [**watch_core_v1_resource_quota_list_for_all_namespaces**](docs/CorevApi.md#watch_core_v1_resource_quota_list_for_all_namespaces) | **GET** /api/v1/watch/resourcequotas | 
*CorevApi* | [**watch_core_v1_secret_list_for_all_namespaces**](docs/CorevApi.md#watch_core_v1_secret_list_for_all_namespaces) | **GET** /api/v1/watch/secrets | 
*CorevApi* | [**watch_core_v1_service_account_list_for_all_namespaces**](docs/CorevApi.md#watch_core_v1_service_account_list_for_all_namespaces) | **GET** /api/v1/watch/serviceaccounts | 
*CorevApi* | [**watch_core_v1_service_list_for_all_namespaces**](docs/CorevApi.md#watch_core_v1_service_list_for_all_namespaces) | **GET** /api/v1/watch/services | 
*DiscoveryApi* | [**get_discovery_api_group**](docs/DiscoveryApi.md#get_discovery_api_group) | **GET** /apis/discovery.k8s.io/ | 
*DiscoveryvApi* | [**create_discovery_v1_namespaced_endpoint_slice**](docs/DiscoveryvApi.md#create_discovery_v1_namespaced_endpoint_slice) | **POST** /apis/discovery.k8s.io/v1/namespaces/{namespace}/endpointslices | 
*DiscoveryvApi* | [**delete_discovery_v1_collection_namespaced_endpoint_slice**](docs/DiscoveryvApi.md#delete_discovery_v1_collection_namespaced_endpoint_slice) | **DELETE** /apis/discovery.k8s.io/v1/namespaces/{namespace}/endpointslices | 
*DiscoveryvApi* | [**delete_discovery_v1_namespaced_endpoint_slice**](docs/DiscoveryvApi.md#delete_discovery_v1_namespaced_endpoint_slice) | **DELETE** /apis/discovery.k8s.io/v1/namespaces/{namespace}/endpointslices/{name} | 
*DiscoveryvApi* | [**get_discovery_v1_api_resources**](docs/DiscoveryvApi.md#get_discovery_v1_api_resources) | **GET** /apis/discovery.k8s.io/v1/ | 
*DiscoveryvApi* | [**list_discovery_v1_endpoint_slice_for_all_namespaces**](docs/DiscoveryvApi.md#list_discovery_v1_endpoint_slice_for_all_namespaces) | **GET** /apis/discovery.k8s.io/v1/endpointslices | 
*DiscoveryvApi* | [**list_discovery_v1_namespaced_endpoint_slice**](docs/DiscoveryvApi.md#list_discovery_v1_namespaced_endpoint_slice) | **GET** /apis/discovery.k8s.io/v1/namespaces/{namespace}/endpointslices | 
*DiscoveryvApi* | [**patch_discovery_v1_namespaced_endpoint_slice**](docs/DiscoveryvApi.md#patch_discovery_v1_namespaced_endpoint_slice) | **PATCH** /apis/discovery.k8s.io/v1/namespaces/{namespace}/endpointslices/{name} | 
*DiscoveryvApi* | [**read_discovery_v1_namespaced_endpoint_slice**](docs/DiscoveryvApi.md#read_discovery_v1_namespaced_endpoint_slice) | **GET** /apis/discovery.k8s.io/v1/namespaces/{namespace}/endpointslices/{name} | 
*DiscoveryvApi* | [**replace_discovery_v1_namespaced_endpoint_slice**](docs/DiscoveryvApi.md#replace_discovery_v1_namespaced_endpoint_slice) | **PUT** /apis/discovery.k8s.io/v1/namespaces/{namespace}/endpointslices/{name} | 
*DiscoveryvApi* | [**watch_discovery_v1_endpoint_slice_list_for_all_namespaces**](docs/DiscoveryvApi.md#watch_discovery_v1_endpoint_slice_list_for_all_namespaces) | **GET** /apis/discovery.k8s.io/v1/watch/endpointslices | 
*DiscoveryvApi* | [**watch_discovery_v1_namespaced_endpoint_slice**](docs/DiscoveryvApi.md#watch_discovery_v1_namespaced_endpoint_slice) | **GET** /apis/discovery.k8s.io/v1/watch/namespaces/{namespace}/endpointslices/{name} | 
*DiscoveryvApi* | [**watch_discovery_v1_namespaced_endpoint_slice_list**](docs/DiscoveryvApi.md#watch_discovery_v1_namespaced_endpoint_slice_list) | **GET** /apis/discovery.k8s.io/v1/watch/namespaces/{namespace}/endpointslices | 
*EventsApi* | [**get_events_api_group**](docs/EventsApi.md#get_events_api_group) | **GET** /apis/events.k8s.io/ | 
*EventsvApi* | [**create_events_v1_namespaced_event**](docs/EventsvApi.md#create_events_v1_namespaced_event) | **POST** /apis/events.k8s.io/v1/namespaces/{namespace}/events | 
*EventsvApi* | [**delete_events_v1_collection_namespaced_event**](docs/EventsvApi.md#delete_events_v1_collection_namespaced_event) | **DELETE** /apis/events.k8s.io/v1/namespaces/{namespace}/events | 
*EventsvApi* | [**delete_events_v1_namespaced_event**](docs/EventsvApi.md#delete_events_v1_namespaced_event) | **DELETE** /apis/events.k8s.io/v1/namespaces/{namespace}/events/{name} | 
*EventsvApi* | [**get_events_v1_api_resources**](docs/EventsvApi.md#get_events_v1_api_resources) | **GET** /apis/events.k8s.io/v1/ | 
*EventsvApi* | [**list_events_v1_event_for_all_namespaces**](docs/EventsvApi.md#list_events_v1_event_for_all_namespaces) | **GET** /apis/events.k8s.io/v1/events | 
*EventsvApi* | [**list_events_v1_namespaced_event**](docs/EventsvApi.md#list_events_v1_namespaced_event) | **GET** /apis/events.k8s.io/v1/namespaces/{namespace}/events | 
*EventsvApi* | [**patch_events_v1_namespaced_event**](docs/EventsvApi.md#patch_events_v1_namespaced_event) | **PATCH** /apis/events.k8s.io/v1/namespaces/{namespace}/events/{name} | 
*EventsvApi* | [**read_events_v1_namespaced_event**](docs/EventsvApi.md#read_events_v1_namespaced_event) | **GET** /apis/events.k8s.io/v1/namespaces/{namespace}/events/{name} | 
*EventsvApi* | [**replace_events_v1_namespaced_event**](docs/EventsvApi.md#replace_events_v1_namespaced_event) | **PUT** /apis/events.k8s.io/v1/namespaces/{namespace}/events/{name} | 
*EventsvApi* | [**watch_events_v1_event_list_for_all_namespaces**](docs/EventsvApi.md#watch_events_v1_event_list_for_all_namespaces) | **GET** /apis/events.k8s.io/v1/watch/events | 
*EventsvApi* | [**watch_events_v1_namespaced_event**](docs/EventsvApi.md#watch_events_v1_namespaced_event) | **GET** /apis/events.k8s.io/v1/watch/namespaces/{namespace}/events/{name} | 
*EventsvApi* | [**watch_events_v1_namespaced_event_list**](docs/EventsvApi.md#watch_events_v1_namespaced_event_list) | **GET** /apis/events.k8s.io/v1/watch/namespaces/{namespace}/events | 
*FlowcontrolApiserverApi* | [**get_flowcontrol_apiserver_api_group**](docs/FlowcontrolApiserverApi.md#get_flowcontrol_apiserver_api_group) | **GET** /apis/flowcontrol.apiserver.k8s.io/ | 
*FlowcontrolApiservervbetaApi* | [**create_flowcontrol_apiserver_v1beta2_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#create_flowcontrol_apiserver_v1beta2_flow_schema) | **POST** /apis/flowcontrol.apiserver.k8s.io/v1beta2/flowschemas | 
*FlowcontrolApiservervbetaApi* | [**create_flowcontrol_apiserver_v1beta2_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#create_flowcontrol_apiserver_v1beta2_priority_level_configuration) | **POST** /apis/flowcontrol.apiserver.k8s.io/v1beta2/prioritylevelconfigurations | 
*FlowcontrolApiservervbetaApi* | [**create_flowcontrol_apiserver_v1beta3_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#create_flowcontrol_apiserver_v1beta3_flow_schema) | **POST** /apis/flowcontrol.apiserver.k8s.io/v1beta3/flowschemas | 
*FlowcontrolApiservervbetaApi* | [**create_flowcontrol_apiserver_v1beta3_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#create_flowcontrol_apiserver_v1beta3_priority_level_configuration) | **POST** /apis/flowcontrol.apiserver.k8s.io/v1beta3/prioritylevelconfigurations | 
*FlowcontrolApiservervbetaApi* | [**delete_flowcontrol_apiserver_v1beta2_collection_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#delete_flowcontrol_apiserver_v1beta2_collection_flow_schema) | **DELETE** /apis/flowcontrol.apiserver.k8s.io/v1beta2/flowschemas | 
*FlowcontrolApiservervbetaApi* | [**delete_flowcontrol_apiserver_v1beta2_collection_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#delete_flowcontrol_apiserver_v1beta2_collection_priority_level_configuration) | **DELETE** /apis/flowcontrol.apiserver.k8s.io/v1beta2/prioritylevelconfigurations | 
*FlowcontrolApiservervbetaApi* | [**delete_flowcontrol_apiserver_v1beta2_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#delete_flowcontrol_apiserver_v1beta2_flow_schema) | **DELETE** /apis/flowcontrol.apiserver.k8s.io/v1beta2/flowschemas/{name} | 
*FlowcontrolApiservervbetaApi* | [**delete_flowcontrol_apiserver_v1beta2_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#delete_flowcontrol_apiserver_v1beta2_priority_level_configuration) | **DELETE** /apis/flowcontrol.apiserver.k8s.io/v1beta2/prioritylevelconfigurations/{name} | 
*FlowcontrolApiservervbetaApi* | [**delete_flowcontrol_apiserver_v1beta3_collection_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#delete_flowcontrol_apiserver_v1beta3_collection_flow_schema) | **DELETE** /apis/flowcontrol.apiserver.k8s.io/v1beta3/flowschemas | 
*FlowcontrolApiservervbetaApi* | [**delete_flowcontrol_apiserver_v1beta3_collection_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#delete_flowcontrol_apiserver_v1beta3_collection_priority_level_configuration) | **DELETE** /apis/flowcontrol.apiserver.k8s.io/v1beta3/prioritylevelconfigurations | 
*FlowcontrolApiservervbetaApi* | [**delete_flowcontrol_apiserver_v1beta3_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#delete_flowcontrol_apiserver_v1beta3_flow_schema) | **DELETE** /apis/flowcontrol.apiserver.k8s.io/v1beta3/flowschemas/{name} | 
*FlowcontrolApiservervbetaApi* | [**delete_flowcontrol_apiserver_v1beta3_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#delete_flowcontrol_apiserver_v1beta3_priority_level_configuration) | **DELETE** /apis/flowcontrol.apiserver.k8s.io/v1beta3/prioritylevelconfigurations/{name} | 
*FlowcontrolApiservervbetaApi* | [**get_flowcontrol_apiserver_v1beta2_api_resources**](docs/FlowcontrolApiservervbetaApi.md#get_flowcontrol_apiserver_v1beta2_api_resources) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta2/ | 
*FlowcontrolApiservervbetaApi* | [**get_flowcontrol_apiserver_v1beta3_api_resources**](docs/FlowcontrolApiservervbetaApi.md#get_flowcontrol_apiserver_v1beta3_api_resources) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta3/ | 
*FlowcontrolApiservervbetaApi* | [**list_flowcontrol_apiserver_v1beta2_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#list_flowcontrol_apiserver_v1beta2_flow_schema) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta2/flowschemas | 
*FlowcontrolApiservervbetaApi* | [**list_flowcontrol_apiserver_v1beta2_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#list_flowcontrol_apiserver_v1beta2_priority_level_configuration) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta2/prioritylevelconfigurations | 
*FlowcontrolApiservervbetaApi* | [**list_flowcontrol_apiserver_v1beta3_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#list_flowcontrol_apiserver_v1beta3_flow_schema) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta3/flowschemas | 
*FlowcontrolApiservervbetaApi* | [**list_flowcontrol_apiserver_v1beta3_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#list_flowcontrol_apiserver_v1beta3_priority_level_configuration) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta3/prioritylevelconfigurations | 
*FlowcontrolApiservervbetaApi* | [**patch_flowcontrol_apiserver_v1beta2_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#patch_flowcontrol_apiserver_v1beta2_flow_schema) | **PATCH** /apis/flowcontrol.apiserver.k8s.io/v1beta2/flowschemas/{name} | 
*FlowcontrolApiservervbetaApi* | [**patch_flowcontrol_apiserver_v1beta2_flow_schema_status**](docs/FlowcontrolApiservervbetaApi.md#patch_flowcontrol_apiserver_v1beta2_flow_schema_status) | **PATCH** /apis/flowcontrol.apiserver.k8s.io/v1beta2/flowschemas/{name}/status | 
*FlowcontrolApiservervbetaApi* | [**patch_flowcontrol_apiserver_v1beta2_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#patch_flowcontrol_apiserver_v1beta2_priority_level_configuration) | **PATCH** /apis/flowcontrol.apiserver.k8s.io/v1beta2/prioritylevelconfigurations/{name} | 
*FlowcontrolApiservervbetaApi* | [**patch_flowcontrol_apiserver_v1beta2_priority_level_configuration_status**](docs/FlowcontrolApiservervbetaApi.md#patch_flowcontrol_apiserver_v1beta2_priority_level_configuration_status) | **PATCH** /apis/flowcontrol.apiserver.k8s.io/v1beta2/prioritylevelconfigurations/{name}/status | 
*FlowcontrolApiservervbetaApi* | [**patch_flowcontrol_apiserver_v1beta3_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#patch_flowcontrol_apiserver_v1beta3_flow_schema) | **PATCH** /apis/flowcontrol.apiserver.k8s.io/v1beta3/flowschemas/{name} | 
*FlowcontrolApiservervbetaApi* | [**patch_flowcontrol_apiserver_v1beta3_flow_schema_status**](docs/FlowcontrolApiservervbetaApi.md#patch_flowcontrol_apiserver_v1beta3_flow_schema_status) | **PATCH** /apis/flowcontrol.apiserver.k8s.io/v1beta3/flowschemas/{name}/status | 
*FlowcontrolApiservervbetaApi* | [**patch_flowcontrol_apiserver_v1beta3_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#patch_flowcontrol_apiserver_v1beta3_priority_level_configuration) | **PATCH** /apis/flowcontrol.apiserver.k8s.io/v1beta3/prioritylevelconfigurations/{name} | 
*FlowcontrolApiservervbetaApi* | [**patch_flowcontrol_apiserver_v1beta3_priority_level_configuration_status**](docs/FlowcontrolApiservervbetaApi.md#patch_flowcontrol_apiserver_v1beta3_priority_level_configuration_status) | **PATCH** /apis/flowcontrol.apiserver.k8s.io/v1beta3/prioritylevelconfigurations/{name}/status | 
*FlowcontrolApiservervbetaApi* | [**read_flowcontrol_apiserver_v1beta2_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#read_flowcontrol_apiserver_v1beta2_flow_schema) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta2/flowschemas/{name} | 
*FlowcontrolApiservervbetaApi* | [**read_flowcontrol_apiserver_v1beta2_flow_schema_status**](docs/FlowcontrolApiservervbetaApi.md#read_flowcontrol_apiserver_v1beta2_flow_schema_status) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta2/flowschemas/{name}/status | 
*FlowcontrolApiservervbetaApi* | [**read_flowcontrol_apiserver_v1beta2_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#read_flowcontrol_apiserver_v1beta2_priority_level_configuration) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta2/prioritylevelconfigurations/{name} | 
*FlowcontrolApiservervbetaApi* | [**read_flowcontrol_apiserver_v1beta2_priority_level_configuration_status**](docs/FlowcontrolApiservervbetaApi.md#read_flowcontrol_apiserver_v1beta2_priority_level_configuration_status) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta2/prioritylevelconfigurations/{name}/status | 
*FlowcontrolApiservervbetaApi* | [**read_flowcontrol_apiserver_v1beta3_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#read_flowcontrol_apiserver_v1beta3_flow_schema) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta3/flowschemas/{name} | 
*FlowcontrolApiservervbetaApi* | [**read_flowcontrol_apiserver_v1beta3_flow_schema_status**](docs/FlowcontrolApiservervbetaApi.md#read_flowcontrol_apiserver_v1beta3_flow_schema_status) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta3/flowschemas/{name}/status | 
*FlowcontrolApiservervbetaApi* | [**read_flowcontrol_apiserver_v1beta3_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#read_flowcontrol_apiserver_v1beta3_priority_level_configuration) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta3/prioritylevelconfigurations/{name} | 
*FlowcontrolApiservervbetaApi* | [**read_flowcontrol_apiserver_v1beta3_priority_level_configuration_status**](docs/FlowcontrolApiservervbetaApi.md#read_flowcontrol_apiserver_v1beta3_priority_level_configuration_status) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta3/prioritylevelconfigurations/{name}/status | 
*FlowcontrolApiservervbetaApi* | [**replace_flowcontrol_apiserver_v1beta2_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#replace_flowcontrol_apiserver_v1beta2_flow_schema) | **PUT** /apis/flowcontrol.apiserver.k8s.io/v1beta2/flowschemas/{name} | 
*FlowcontrolApiservervbetaApi* | [**replace_flowcontrol_apiserver_v1beta2_flow_schema_status**](docs/FlowcontrolApiservervbetaApi.md#replace_flowcontrol_apiserver_v1beta2_flow_schema_status) | **PUT** /apis/flowcontrol.apiserver.k8s.io/v1beta2/flowschemas/{name}/status | 
*FlowcontrolApiservervbetaApi* | [**replace_flowcontrol_apiserver_v1beta2_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#replace_flowcontrol_apiserver_v1beta2_priority_level_configuration) | **PUT** /apis/flowcontrol.apiserver.k8s.io/v1beta2/prioritylevelconfigurations/{name} | 
*FlowcontrolApiservervbetaApi* | [**replace_flowcontrol_apiserver_v1beta2_priority_level_configuration_status**](docs/FlowcontrolApiservervbetaApi.md#replace_flowcontrol_apiserver_v1beta2_priority_level_configuration_status) | **PUT** /apis/flowcontrol.apiserver.k8s.io/v1beta2/prioritylevelconfigurations/{name}/status | 
*FlowcontrolApiservervbetaApi* | [**replace_flowcontrol_apiserver_v1beta3_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#replace_flowcontrol_apiserver_v1beta3_flow_schema) | **PUT** /apis/flowcontrol.apiserver.k8s.io/v1beta3/flowschemas/{name} | 
*FlowcontrolApiservervbetaApi* | [**replace_flowcontrol_apiserver_v1beta3_flow_schema_status**](docs/FlowcontrolApiservervbetaApi.md#replace_flowcontrol_apiserver_v1beta3_flow_schema_status) | **PUT** /apis/flowcontrol.apiserver.k8s.io/v1beta3/flowschemas/{name}/status | 
*FlowcontrolApiservervbetaApi* | [**replace_flowcontrol_apiserver_v1beta3_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#replace_flowcontrol_apiserver_v1beta3_priority_level_configuration) | **PUT** /apis/flowcontrol.apiserver.k8s.io/v1beta3/prioritylevelconfigurations/{name} | 
*FlowcontrolApiservervbetaApi* | [**replace_flowcontrol_apiserver_v1beta3_priority_level_configuration_status**](docs/FlowcontrolApiservervbetaApi.md#replace_flowcontrol_apiserver_v1beta3_priority_level_configuration_status) | **PUT** /apis/flowcontrol.apiserver.k8s.io/v1beta3/prioritylevelconfigurations/{name}/status | 
*FlowcontrolApiservervbetaApi* | [**watch_flowcontrol_apiserver_v1beta2_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#watch_flowcontrol_apiserver_v1beta2_flow_schema) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta2/watch/flowschemas/{name} | 
*FlowcontrolApiservervbetaApi* | [**watch_flowcontrol_apiserver_v1beta2_flow_schema_list**](docs/FlowcontrolApiservervbetaApi.md#watch_flowcontrol_apiserver_v1beta2_flow_schema_list) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta2/watch/flowschemas | 
*FlowcontrolApiservervbetaApi* | [**watch_flowcontrol_apiserver_v1beta2_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#watch_flowcontrol_apiserver_v1beta2_priority_level_configuration) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta2/watch/prioritylevelconfigurations/{name} | 
*FlowcontrolApiservervbetaApi* | [**watch_flowcontrol_apiserver_v1beta2_priority_level_configuration_list**](docs/FlowcontrolApiservervbetaApi.md#watch_flowcontrol_apiserver_v1beta2_priority_level_configuration_list) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta2/watch/prioritylevelconfigurations | 
*FlowcontrolApiservervbetaApi* | [**watch_flowcontrol_apiserver_v1beta3_flow_schema**](docs/FlowcontrolApiservervbetaApi.md#watch_flowcontrol_apiserver_v1beta3_flow_schema) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta3/watch/flowschemas/{name} | 
*FlowcontrolApiservervbetaApi* | [**watch_flowcontrol_apiserver_v1beta3_flow_schema_list**](docs/FlowcontrolApiservervbetaApi.md#watch_flowcontrol_apiserver_v1beta3_flow_schema_list) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta3/watch/flowschemas | 
*FlowcontrolApiservervbetaApi* | [**watch_flowcontrol_apiserver_v1beta3_priority_level_configuration**](docs/FlowcontrolApiservervbetaApi.md#watch_flowcontrol_apiserver_v1beta3_priority_level_configuration) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta3/watch/prioritylevelconfigurations/{name} | 
*FlowcontrolApiservervbetaApi* | [**watch_flowcontrol_apiserver_v1beta3_priority_level_configuration_list**](docs/FlowcontrolApiservervbetaApi.md#watch_flowcontrol_apiserver_v1beta3_priority_level_configuration_list) | **GET** /apis/flowcontrol.apiserver.k8s.io/v1beta3/watch/prioritylevelconfigurations | 
*InternalApiserverApi* | [**get_internal_apiserver_api_group**](docs/InternalApiserverApi.md#get_internal_apiserver_api_group) | **GET** /apis/internal.apiserver.k8s.io/ | 
*InternalApiservervalphaApi* | [**create_internal_apiserver_v1alpha1_storage_version**](docs/InternalApiservervalphaApi.md#create_internal_apiserver_v1alpha1_storage_version) | **POST** /apis/internal.apiserver.k8s.io/v1alpha1/storageversions | 
*InternalApiservervalphaApi* | [**delete_internal_apiserver_v1alpha1_collection_storage_version**](docs/InternalApiservervalphaApi.md#delete_internal_apiserver_v1alpha1_collection_storage_version) | **DELETE** /apis/internal.apiserver.k8s.io/v1alpha1/storageversions | 
*InternalApiservervalphaApi* | [**delete_internal_apiserver_v1alpha1_storage_version**](docs/InternalApiservervalphaApi.md#delete_internal_apiserver_v1alpha1_storage_version) | **DELETE** /apis/internal.apiserver.k8s.io/v1alpha1/storageversions/{name} | 
*InternalApiservervalphaApi* | [**get_internal_apiserver_v1alpha1_api_resources**](docs/InternalApiservervalphaApi.md#get_internal_apiserver_v1alpha1_api_resources) | **GET** /apis/internal.apiserver.k8s.io/v1alpha1/ | 
*InternalApiservervalphaApi* | [**list_internal_apiserver_v1alpha1_storage_version**](docs/InternalApiservervalphaApi.md#list_internal_apiserver_v1alpha1_storage_version) | **GET** /apis/internal.apiserver.k8s.io/v1alpha1/storageversions | 
*InternalApiservervalphaApi* | [**patch_internal_apiserver_v1alpha1_storage_version**](docs/InternalApiservervalphaApi.md#patch_internal_apiserver_v1alpha1_storage_version) | **PATCH** /apis/internal.apiserver.k8s.io/v1alpha1/storageversions/{name} | 
*InternalApiservervalphaApi* | [**patch_internal_apiserver_v1alpha1_storage_version_status**](docs/InternalApiservervalphaApi.md#patch_internal_apiserver_v1alpha1_storage_version_status) | **PATCH** /apis/internal.apiserver.k8s.io/v1alpha1/storageversions/{name}/status | 
*InternalApiservervalphaApi* | [**read_internal_apiserver_v1alpha1_storage_version**](docs/InternalApiservervalphaApi.md#read_internal_apiserver_v1alpha1_storage_version) | **GET** /apis/internal.apiserver.k8s.io/v1alpha1/storageversions/{name} | 
*InternalApiservervalphaApi* | [**read_internal_apiserver_v1alpha1_storage_version_status**](docs/InternalApiservervalphaApi.md#read_internal_apiserver_v1alpha1_storage_version_status) | **GET** /apis/internal.apiserver.k8s.io/v1alpha1/storageversions/{name}/status | 
*InternalApiservervalphaApi* | [**replace_internal_apiserver_v1alpha1_storage_version**](docs/InternalApiservervalphaApi.md#replace_internal_apiserver_v1alpha1_storage_version) | **PUT** /apis/internal.apiserver.k8s.io/v1alpha1/storageversions/{name} | 
*InternalApiservervalphaApi* | [**replace_internal_apiserver_v1alpha1_storage_version_status**](docs/InternalApiservervalphaApi.md#replace_internal_apiserver_v1alpha1_storage_version_status) | **PUT** /apis/internal.apiserver.k8s.io/v1alpha1/storageversions/{name}/status | 
*InternalApiservervalphaApi* | [**watch_internal_apiserver_v1alpha1_storage_version**](docs/InternalApiservervalphaApi.md#watch_internal_apiserver_v1alpha1_storage_version) | **GET** /apis/internal.apiserver.k8s.io/v1alpha1/watch/storageversions/{name} | 
*InternalApiservervalphaApi* | [**watch_internal_apiserver_v1alpha1_storage_version_list**](docs/InternalApiservervalphaApi.md#watch_internal_apiserver_v1alpha1_storage_version_list) | **GET** /apis/internal.apiserver.k8s.io/v1alpha1/watch/storageversions | 
*LogsApi* | [**log_file_handler**](docs/LogsApi.md#log_file_handler) | **GET** /logs/{logpath} | 
*LogsApi* | [**log_file_list_handler**](docs/LogsApi.md#log_file_list_handler) | **GET** /logs/ | 
*NetworkingApi* | [**get_networking_api_group**](docs/NetworkingApi.md#get_networking_api_group) | **GET** /apis/networking.k8s.io/ | 
*NetworkingvApi* | [**create_networking_v1_ingress_class**](docs/NetworkingvApi.md#create_networking_v1_ingress_class) | **POST** /apis/networking.k8s.io/v1/ingressclasses | 
*NetworkingvApi* | [**create_networking_v1_namespaced_ingress**](docs/NetworkingvApi.md#create_networking_v1_namespaced_ingress) | **POST** /apis/networking.k8s.io/v1/namespaces/{namespace}/ingresses | 
*NetworkingvApi* | [**create_networking_v1_namespaced_network_policy**](docs/NetworkingvApi.md#create_networking_v1_namespaced_network_policy) | **POST** /apis/networking.k8s.io/v1/namespaces/{namespace}/networkpolicies | 
*NetworkingvApi* | [**delete_networking_v1_collection_ingress_class**](docs/NetworkingvApi.md#delete_networking_v1_collection_ingress_class) | **DELETE** /apis/networking.k8s.io/v1/ingressclasses | 
*NetworkingvApi* | [**delete_networking_v1_collection_namespaced_ingress**](docs/NetworkingvApi.md#delete_networking_v1_collection_namespaced_ingress) | **DELETE** /apis/networking.k8s.io/v1/namespaces/{namespace}/ingresses | 
*NetworkingvApi* | [**delete_networking_v1_collection_namespaced_network_policy**](docs/NetworkingvApi.md#delete_networking_v1_collection_namespaced_network_policy) | **DELETE** /apis/networking.k8s.io/v1/namespaces/{namespace}/networkpolicies | 
*NetworkingvApi* | [**delete_networking_v1_ingress_class**](docs/NetworkingvApi.md#delete_networking_v1_ingress_class) | **DELETE** /apis/networking.k8s.io/v1/ingressclasses/{name} | 
*NetworkingvApi* | [**delete_networking_v1_namespaced_ingress**](docs/NetworkingvApi.md#delete_networking_v1_namespaced_ingress) | **DELETE** /apis/networking.k8s.io/v1/namespaces/{namespace}/ingresses/{name} | 
*NetworkingvApi* | [**delete_networking_v1_namespaced_network_policy**](docs/NetworkingvApi.md#delete_networking_v1_namespaced_network_policy) | **DELETE** /apis/networking.k8s.io/v1/namespaces/{namespace}/networkpolicies/{name} | 
*NetworkingvApi* | [**get_networking_v1_api_resources**](docs/NetworkingvApi.md#get_networking_v1_api_resources) | **GET** /apis/networking.k8s.io/v1/ | 
*NetworkingvApi* | [**list_networking_v1_ingress_class**](docs/NetworkingvApi.md#list_networking_v1_ingress_class) | **GET** /apis/networking.k8s.io/v1/ingressclasses | 
*NetworkingvApi* | [**list_networking_v1_ingress_for_all_namespaces**](docs/NetworkingvApi.md#list_networking_v1_ingress_for_all_namespaces) | **GET** /apis/networking.k8s.io/v1/ingresses | 
*NetworkingvApi* | [**list_networking_v1_namespaced_ingress**](docs/NetworkingvApi.md#list_networking_v1_namespaced_ingress) | **GET** /apis/networking.k8s.io/v1/namespaces/{namespace}/ingresses | 
*NetworkingvApi* | [**list_networking_v1_namespaced_network_policy**](docs/NetworkingvApi.md#list_networking_v1_namespaced_network_policy) | **GET** /apis/networking.k8s.io/v1/namespaces/{namespace}/networkpolicies | 
*NetworkingvApi* | [**list_networking_v1_network_policy_for_all_namespaces**](docs/NetworkingvApi.md#list_networking_v1_network_policy_for_all_namespaces) | **GET** /apis/networking.k8s.io/v1/networkpolicies | 
*NetworkingvApi* | [**patch_networking_v1_ingress_class**](docs/NetworkingvApi.md#patch_networking_v1_ingress_class) | **PATCH** /apis/networking.k8s.io/v1/ingressclasses/{name} | 
*NetworkingvApi* | [**patch_networking_v1_namespaced_ingress**](docs/NetworkingvApi.md#patch_networking_v1_namespaced_ingress) | **PATCH** /apis/networking.k8s.io/v1/namespaces/{namespace}/ingresses/{name} | 
*NetworkingvApi* | [**patch_networking_v1_namespaced_ingress_status**](docs/NetworkingvApi.md#patch_networking_v1_namespaced_ingress_status) | **PATCH** /apis/networking.k8s.io/v1/namespaces/{namespace}/ingresses/{name}/status | 
*NetworkingvApi* | [**patch_networking_v1_namespaced_network_policy**](docs/NetworkingvApi.md#patch_networking_v1_namespaced_network_policy) | **PATCH** /apis/networking.k8s.io/v1/namespaces/{namespace}/networkpolicies/{name} | 
*NetworkingvApi* | [**patch_networking_v1_namespaced_network_policy_status**](docs/NetworkingvApi.md#patch_networking_v1_namespaced_network_policy_status) | **PATCH** /apis/networking.k8s.io/v1/namespaces/{namespace}/networkpolicies/{name}/status | 
*NetworkingvApi* | [**read_networking_v1_ingress_class**](docs/NetworkingvApi.md#read_networking_v1_ingress_class) | **GET** /apis/networking.k8s.io/v1/ingressclasses/{name} | 
*NetworkingvApi* | [**read_networking_v1_namespaced_ingress**](docs/NetworkingvApi.md#read_networking_v1_namespaced_ingress) | **GET** /apis/networking.k8s.io/v1/namespaces/{namespace}/ingresses/{name} | 
*NetworkingvApi* | [**read_networking_v1_namespaced_ingress_status**](docs/NetworkingvApi.md#read_networking_v1_namespaced_ingress_status) | **GET** /apis/networking.k8s.io/v1/namespaces/{namespace}/ingresses/{name}/status | 
*NetworkingvApi* | [**read_networking_v1_namespaced_network_policy**](docs/NetworkingvApi.md#read_networking_v1_namespaced_network_policy) | **GET** /apis/networking.k8s.io/v1/namespaces/{namespace}/networkpolicies/{name} | 
*NetworkingvApi* | [**read_networking_v1_namespaced_network_policy_status**](docs/NetworkingvApi.md#read_networking_v1_namespaced_network_policy_status) | **GET** /apis/networking.k8s.io/v1/namespaces/{namespace}/networkpolicies/{name}/status | 
*NetworkingvApi* | [**replace_networking_v1_ingress_class**](docs/NetworkingvApi.md#replace_networking_v1_ingress_class) | **PUT** /apis/networking.k8s.io/v1/ingressclasses/{name} | 
*NetworkingvApi* | [**replace_networking_v1_namespaced_ingress**](docs/NetworkingvApi.md#replace_networking_v1_namespaced_ingress) | **PUT** /apis/networking.k8s.io/v1/namespaces/{namespace}/ingresses/{name} | 
*NetworkingvApi* | [**replace_networking_v1_namespaced_ingress_status**](docs/NetworkingvApi.md#replace_networking_v1_namespaced_ingress_status) | **PUT** /apis/networking.k8s.io/v1/namespaces/{namespace}/ingresses/{name}/status | 
*NetworkingvApi* | [**replace_networking_v1_namespaced_network_policy**](docs/NetworkingvApi.md#replace_networking_v1_namespaced_network_policy) | **PUT** /apis/networking.k8s.io/v1/namespaces/{namespace}/networkpolicies/{name} | 
*NetworkingvApi* | [**replace_networking_v1_namespaced_network_policy_status**](docs/NetworkingvApi.md#replace_networking_v1_namespaced_network_policy_status) | **PUT** /apis/networking.k8s.io/v1/namespaces/{namespace}/networkpolicies/{name}/status | 
*NetworkingvApi* | [**watch_networking_v1_ingress_class**](docs/NetworkingvApi.md#watch_networking_v1_ingress_class) | **GET** /apis/networking.k8s.io/v1/watch/ingressclasses/{name} | 
*NetworkingvApi* | [**watch_networking_v1_ingress_class_list**](docs/NetworkingvApi.md#watch_networking_v1_ingress_class_list) | **GET** /apis/networking.k8s.io/v1/watch/ingressclasses | 
*NetworkingvApi* | [**watch_networking_v1_ingress_list_for_all_namespaces**](docs/NetworkingvApi.md#watch_networking_v1_ingress_list_for_all_namespaces) | **GET** /apis/networking.k8s.io/v1/watch/ingresses | 
*NetworkingvApi* | [**watch_networking_v1_namespaced_ingress**](docs/NetworkingvApi.md#watch_networking_v1_namespaced_ingress) | **GET** /apis/networking.k8s.io/v1/watch/namespaces/{namespace}/ingresses/{name} | 
*NetworkingvApi* | [**watch_networking_v1_namespaced_ingress_list**](docs/NetworkingvApi.md#watch_networking_v1_namespaced_ingress_list) | **GET** /apis/networking.k8s.io/v1/watch/namespaces/{namespace}/ingresses | 
*NetworkingvApi* | [**watch_networking_v1_namespaced_network_policy**](docs/NetworkingvApi.md#watch_networking_v1_namespaced_network_policy) | **GET** /apis/networking.k8s.io/v1/watch/namespaces/{namespace}/networkpolicies/{name} | 
*NetworkingvApi* | [**watch_networking_v1_namespaced_network_policy_list**](docs/NetworkingvApi.md#watch_networking_v1_namespaced_network_policy_list) | **GET** /apis/networking.k8s.io/v1/watch/namespaces/{namespace}/networkpolicies | 
*NetworkingvApi* | [**watch_networking_v1_network_policy_list_for_all_namespaces**](docs/NetworkingvApi.md#watch_networking_v1_network_policy_list_for_all_namespaces) | **GET** /apis/networking.k8s.io/v1/watch/networkpolicies | 
*NetworkingvalphaApi* | [**create_networking_v1alpha1_cluster_cidr**](docs/NetworkingvalphaApi.md#create_networking_v1alpha1_cluster_cidr) | **POST** /apis/networking.k8s.io/v1alpha1/clustercidrs | 
*NetworkingvalphaApi* | [**delete_networking_v1alpha1_cluster_cidr**](docs/NetworkingvalphaApi.md#delete_networking_v1alpha1_cluster_cidr) | **DELETE** /apis/networking.k8s.io/v1alpha1/clustercidrs/{name} | 
*NetworkingvalphaApi* | [**delete_networking_v1alpha1_collection_cluster_cidr**](docs/NetworkingvalphaApi.md#delete_networking_v1alpha1_collection_cluster_cidr) | **DELETE** /apis/networking.k8s.io/v1alpha1/clustercidrs | 
*NetworkingvalphaApi* | [**get_networking_v1alpha1_api_resources**](docs/NetworkingvalphaApi.md#get_networking_v1alpha1_api_resources) | **GET** /apis/networking.k8s.io/v1alpha1/ | 
*NetworkingvalphaApi* | [**list_networking_v1alpha1_cluster_cidr**](docs/NetworkingvalphaApi.md#list_networking_v1alpha1_cluster_cidr) | **GET** /apis/networking.k8s.io/v1alpha1/clustercidrs | 
*NetworkingvalphaApi* | [**patch_networking_v1alpha1_cluster_cidr**](docs/NetworkingvalphaApi.md#patch_networking_v1alpha1_cluster_cidr) | **PATCH** /apis/networking.k8s.io/v1alpha1/clustercidrs/{name} | 
*NetworkingvalphaApi* | [**read_networking_v1alpha1_cluster_cidr**](docs/NetworkingvalphaApi.md#read_networking_v1alpha1_cluster_cidr) | **GET** /apis/networking.k8s.io/v1alpha1/clustercidrs/{name} | 
*NetworkingvalphaApi* | [**replace_networking_v1alpha1_cluster_cidr**](docs/NetworkingvalphaApi.md#replace_networking_v1alpha1_cluster_cidr) | **PUT** /apis/networking.k8s.io/v1alpha1/clustercidrs/{name} | 
*NetworkingvalphaApi* | [**watch_networking_v1alpha1_cluster_cidr**](docs/NetworkingvalphaApi.md#watch_networking_v1alpha1_cluster_cidr) | **GET** /apis/networking.k8s.io/v1alpha1/watch/clustercidrs/{name} | 
*NetworkingvalphaApi* | [**watch_networking_v1alpha1_cluster_cidr_list**](docs/NetworkingvalphaApi.md#watch_networking_v1alpha1_cluster_cidr_list) | **GET** /apis/networking.k8s.io/v1alpha1/watch/clustercidrs | 
*NodeApi* | [**get_node_api_group**](docs/NodeApi.md#get_node_api_group) | **GET** /apis/node.k8s.io/ | 
*NodevApi* | [**create_node_v1_runtime_class**](docs/NodevApi.md#create_node_v1_runtime_class) | **POST** /apis/node.k8s.io/v1/runtimeclasses | 
*NodevApi* | [**delete_node_v1_collection_runtime_class**](docs/NodevApi.md#delete_node_v1_collection_runtime_class) | **DELETE** /apis/node.k8s.io/v1/runtimeclasses | 
*NodevApi* | [**delete_node_v1_runtime_class**](docs/NodevApi.md#delete_node_v1_runtime_class) | **DELETE** /apis/node.k8s.io/v1/runtimeclasses/{name} | 
*NodevApi* | [**get_node_v1_api_resources**](docs/NodevApi.md#get_node_v1_api_resources) | **GET** /apis/node.k8s.io/v1/ | 
*NodevApi* | [**list_node_v1_runtime_class**](docs/NodevApi.md#list_node_v1_runtime_class) | **GET** /apis/node.k8s.io/v1/runtimeclasses | 
*NodevApi* | [**patch_node_v1_runtime_class**](docs/NodevApi.md#patch_node_v1_runtime_class) | **PATCH** /apis/node.k8s.io/v1/runtimeclasses/{name} | 
*NodevApi* | [**read_node_v1_runtime_class**](docs/NodevApi.md#read_node_v1_runtime_class) | **GET** /apis/node.k8s.io/v1/runtimeclasses/{name} | 
*NodevApi* | [**replace_node_v1_runtime_class**](docs/NodevApi.md#replace_node_v1_runtime_class) | **PUT** /apis/node.k8s.io/v1/runtimeclasses/{name} | 
*NodevApi* | [**watch_node_v1_runtime_class**](docs/NodevApi.md#watch_node_v1_runtime_class) | **GET** /apis/node.k8s.io/v1/watch/runtimeclasses/{name} | 
*NodevApi* | [**watch_node_v1_runtime_class_list**](docs/NodevApi.md#watch_node_v1_runtime_class_list) | **GET** /apis/node.k8s.io/v1/watch/runtimeclasses | 
*OpenidApi* | [**get_service_account_issuer_open_id_keyset**](docs/OpenidApi.md#get_service_account_issuer_open_id_keyset) | **GET** /openid/v1/jwks/ | 
*PolicyApi* | [**get_policy_api_group**](docs/PolicyApi.md#get_policy_api_group) | **GET** /apis/policy/ | 
*PolicyvApi* | [**create_policy_v1_namespaced_pod_disruption_budget**](docs/PolicyvApi.md#create_policy_v1_namespaced_pod_disruption_budget) | **POST** /apis/policy/v1/namespaces/{namespace}/poddisruptionbudgets | 
*PolicyvApi* | [**delete_policy_v1_collection_namespaced_pod_disruption_budget**](docs/PolicyvApi.md#delete_policy_v1_collection_namespaced_pod_disruption_budget) | **DELETE** /apis/policy/v1/namespaces/{namespace}/poddisruptionbudgets | 
*PolicyvApi* | [**delete_policy_v1_namespaced_pod_disruption_budget**](docs/PolicyvApi.md#delete_policy_v1_namespaced_pod_disruption_budget) | **DELETE** /apis/policy/v1/namespaces/{namespace}/poddisruptionbudgets/{name} | 
*PolicyvApi* | [**get_policy_v1_api_resources**](docs/PolicyvApi.md#get_policy_v1_api_resources) | **GET** /apis/policy/v1/ | 
*PolicyvApi* | [**list_policy_v1_namespaced_pod_disruption_budget**](docs/PolicyvApi.md#list_policy_v1_namespaced_pod_disruption_budget) | **GET** /apis/policy/v1/namespaces/{namespace}/poddisruptionbudgets | 
*PolicyvApi* | [**list_policy_v1_pod_disruption_budget_for_all_namespaces**](docs/PolicyvApi.md#list_policy_v1_pod_disruption_budget_for_all_namespaces) | **GET** /apis/policy/v1/poddisruptionbudgets | 
*PolicyvApi* | [**patch_policy_v1_namespaced_pod_disruption_budget**](docs/PolicyvApi.md#patch_policy_v1_namespaced_pod_disruption_budget) | **PATCH** /apis/policy/v1/namespaces/{namespace}/poddisruptionbudgets/{name} | 
*PolicyvApi* | [**patch_policy_v1_namespaced_pod_disruption_budget_status**](docs/PolicyvApi.md#patch_policy_v1_namespaced_pod_disruption_budget_status) | **PATCH** /apis/policy/v1/namespaces/{namespace}/poddisruptionbudgets/{name}/status | 
*PolicyvApi* | [**read_policy_v1_namespaced_pod_disruption_budget**](docs/PolicyvApi.md#read_policy_v1_namespaced_pod_disruption_budget) | **GET** /apis/policy/v1/namespaces/{namespace}/poddisruptionbudgets/{name} | 
*PolicyvApi* | [**read_policy_v1_namespaced_pod_disruption_budget_status**](docs/PolicyvApi.md#read_policy_v1_namespaced_pod_disruption_budget_status) | **GET** /apis/policy/v1/namespaces/{namespace}/poddisruptionbudgets/{name}/status | 
*PolicyvApi* | [**replace_policy_v1_namespaced_pod_disruption_budget**](docs/PolicyvApi.md#replace_policy_v1_namespaced_pod_disruption_budget) | **PUT** /apis/policy/v1/namespaces/{namespace}/poddisruptionbudgets/{name} | 
*PolicyvApi* | [**replace_policy_v1_namespaced_pod_disruption_budget_status**](docs/PolicyvApi.md#replace_policy_v1_namespaced_pod_disruption_budget_status) | **PUT** /apis/policy/v1/namespaces/{namespace}/poddisruptionbudgets/{name}/status | 
*PolicyvApi* | [**watch_policy_v1_namespaced_pod_disruption_budget**](docs/PolicyvApi.md#watch_policy_v1_namespaced_pod_disruption_budget) | **GET** /apis/policy/v1/watch/namespaces/{namespace}/poddisruptionbudgets/{name} | 
*PolicyvApi* | [**watch_policy_v1_namespaced_pod_disruption_budget_list**](docs/PolicyvApi.md#watch_policy_v1_namespaced_pod_disruption_budget_list) | **GET** /apis/policy/v1/watch/namespaces/{namespace}/poddisruptionbudgets | 
*PolicyvApi* | [**watch_policy_v1_pod_disruption_budget_list_for_all_namespaces**](docs/PolicyvApi.md#watch_policy_v1_pod_disruption_budget_list_for_all_namespaces) | **GET** /apis/policy/v1/watch/poddisruptionbudgets | 
*RbacAuthorizationApi* | [**get_rbac_authorization_api_group**](docs/RbacAuthorizationApi.md#get_rbac_authorization_api_group) | **GET** /apis/rbac.authorization.k8s.io/ | 
*RbacAuthorizationvApi* | [**create_rbac_authorization_v1_cluster_role**](docs/RbacAuthorizationvApi.md#create_rbac_authorization_v1_cluster_role) | **POST** /apis/rbac.authorization.k8s.io/v1/clusterroles | 
*RbacAuthorizationvApi* | [**create_rbac_authorization_v1_cluster_role_binding**](docs/RbacAuthorizationvApi.md#create_rbac_authorization_v1_cluster_role_binding) | **POST** /apis/rbac.authorization.k8s.io/v1/clusterrolebindings | 
*RbacAuthorizationvApi* | [**create_rbac_authorization_v1_namespaced_role**](docs/RbacAuthorizationvApi.md#create_rbac_authorization_v1_namespaced_role) | **POST** /apis/rbac.authorization.k8s.io/v1/namespaces/{namespace}/roles | 
*RbacAuthorizationvApi* | [**create_rbac_authorization_v1_namespaced_role_binding**](docs/RbacAuthorizationvApi.md#create_rbac_authorization_v1_namespaced_role_binding) | **POST** /apis/rbac.authorization.k8s.io/v1/namespaces/{namespace}/rolebindings | 
*RbacAuthorizationvApi* | [**delete_rbac_authorization_v1_cluster_role**](docs/RbacAuthorizationvApi.md#delete_rbac_authorization_v1_cluster_role) | **DELETE** /apis/rbac.authorization.k8s.io/v1/clusterroles/{name} | 
*RbacAuthorizationvApi* | [**delete_rbac_authorization_v1_cluster_role_binding**](docs/RbacAuthorizationvApi.md#delete_rbac_authorization_v1_cluster_role_binding) | **DELETE** /apis/rbac.authorization.k8s.io/v1/clusterrolebindings/{name} | 
*RbacAuthorizationvApi* | [**delete_rbac_authorization_v1_collection_cluster_role**](docs/RbacAuthorizationvApi.md#delete_rbac_authorization_v1_collection_cluster_role) | **DELETE** /apis/rbac.authorization.k8s.io/v1/clusterroles | 
*RbacAuthorizationvApi* | [**delete_rbac_authorization_v1_collection_cluster_role_binding**](docs/RbacAuthorizationvApi.md#delete_rbac_authorization_v1_collection_cluster_role_binding) | **DELETE** /apis/rbac.authorization.k8s.io/v1/clusterrolebindings | 
*RbacAuthorizationvApi* | [**delete_rbac_authorization_v1_collection_namespaced_role**](docs/RbacAuthorizationvApi.md#delete_rbac_authorization_v1_collection_namespaced_role) | **DELETE** /apis/rbac.authorization.k8s.io/v1/namespaces/{namespace}/roles | 
*RbacAuthorizationvApi* | [**delete_rbac_authorization_v1_collection_namespaced_role_binding**](docs/RbacAuthorizationvApi.md#delete_rbac_authorization_v1_collection_namespaced_role_binding) | **DELETE** /apis/rbac.authorization.k8s.io/v1/namespaces/{namespace}/rolebindings | 
*RbacAuthorizationvApi* | [**delete_rbac_authorization_v1_namespaced_role**](docs/RbacAuthorizationvApi.md#delete_rbac_authorization_v1_namespaced_role) | **DELETE** /apis/rbac.authorization.k8s.io/v1/namespaces/{namespace}/roles/{name} | 
*RbacAuthorizationvApi* | [**delete_rbac_authorization_v1_namespaced_role_binding**](docs/RbacAuthorizationvApi.md#delete_rbac_authorization_v1_namespaced_role_binding) | **DELETE** /apis/rbac.authorization.k8s.io/v1/namespaces/{namespace}/rolebindings/{name} | 
*RbacAuthorizationvApi* | [**get_rbac_authorization_v1_api_resources**](docs/RbacAuthorizationvApi.md#get_rbac_authorization_v1_api_resources) | **GET** /apis/rbac.authorization.k8s.io/v1/ | 
*RbacAuthorizationvApi* | [**list_rbac_authorization_v1_cluster_role**](docs/RbacAuthorizationvApi.md#list_rbac_authorization_v1_cluster_role) | **GET** /apis/rbac.authorization.k8s.io/v1/clusterroles | 
*RbacAuthorizationvApi* | [**list_rbac_authorization_v1_cluster_role_binding**](docs/RbacAuthorizationvApi.md#list_rbac_authorization_v1_cluster_role_binding) | **GET** /apis/rbac.authorization.k8s.io/v1/clusterrolebindings | 
*RbacAuthorizationvApi* | [**list_rbac_authorization_v1_namespaced_role**](docs/RbacAuthorizationvApi.md#list_rbac_authorization_v1_namespaced_role) | **GET** /apis/rbac.authorization.k8s.io/v1/namespaces/{namespace}/roles | 
*RbacAuthorizationvApi* | [**list_rbac_authorization_v1_namespaced_role_binding**](docs/RbacAuthorizationvApi.md#list_rbac_authorization_v1_namespaced_role_binding) | **GET** /apis/rbac.authorization.k8s.io/v1/namespaces/{namespace}/rolebindings | 
*RbacAuthorizationvApi* | [**list_rbac_authorization_v1_role_binding_for_all_namespaces**](docs/RbacAuthorizationvApi.md#list_rbac_authorization_v1_role_binding_for_all_namespaces) | **GET** /apis/rbac.authorization.k8s.io/v1/rolebindings | 
*RbacAuthorizationvApi* | [**list_rbac_authorization_v1_role_for_all_namespaces**](docs/RbacAuthorizationvApi.md#list_rbac_authorization_v1_role_for_all_namespaces) | **GET** /apis/rbac.authorization.k8s.io/v1/roles | 
*RbacAuthorizationvApi* | [**patch_rbac_authorization_v1_cluster_role**](docs/RbacAuthorizationvApi.md#patch_rbac_authorization_v1_cluster_role) | **PATCH** /apis/rbac.authorization.k8s.io/v1/clusterroles/{name} | 
*RbacAuthorizationvApi* | [**patch_rbac_authorization_v1_cluster_role_binding**](docs/RbacAuthorizationvApi.md#patch_rbac_authorization_v1_cluster_role_binding) | **PATCH** /apis/rbac.authorization.k8s.io/v1/clusterrolebindings/{name} | 
*RbacAuthorizationvApi* | [**patch_rbac_authorization_v1_namespaced_role**](docs/RbacAuthorizationvApi.md#patch_rbac_authorization_v1_namespaced_role) | **PATCH** /apis/rbac.authorization.k8s.io/v1/namespaces/{namespace}/roles/{name} | 
*RbacAuthorizationvApi* | [**patch_rbac_authorization_v1_namespaced_role_binding**](docs/RbacAuthorizationvApi.md#patch_rbac_authorization_v1_namespaced_role_binding) | **PATCH** /apis/rbac.authorization.k8s.io/v1/namespaces/{namespace}/rolebindings/{name} | 
*RbacAuthorizationvApi* | [**read_rbac_authorization_v1_cluster_role**](docs/RbacAuthorizationvApi.md#read_rbac_authorization_v1_cluster_role) | **GET** /apis/rbac.authorization.k8s.io/v1/clusterroles/{name} | 
*RbacAuthorizationvApi* | [**read_rbac_authorization_v1_cluster_role_binding**](docs/RbacAuthorizationvApi.md#read_rbac_authorization_v1_cluster_role_binding) | **GET** /apis/rbac.authorization.k8s.io/v1/clusterrolebindings/{name} | 
*RbacAuthorizationvApi* | [**read_rbac_authorization_v1_namespaced_role**](docs/RbacAuthorizationvApi.md#read_rbac_authorization_v1_namespaced_role) | **GET** /apis/rbac.authorization.k8s.io/v1/namespaces/{namespace}/roles/{name} | 
*RbacAuthorizationvApi* | [**read_rbac_authorization_v1_namespaced_role_binding**](docs/RbacAuthorizationvApi.md#read_rbac_authorization_v1_namespaced_role_binding) | **GET** /apis/rbac.authorization.k8s.io/v1/namespaces/{namespace}/rolebindings/{name} | 
*RbacAuthorizationvApi* | [**replace_rbac_authorization_v1_cluster_role**](docs/RbacAuthorizationvApi.md#replace_rbac_authorization_v1_cluster_role) | **PUT** /apis/rbac.authorization.k8s.io/v1/clusterroles/{name} | 
*RbacAuthorizationvApi* | [**replace_rbac_authorization_v1_cluster_role_binding**](docs/RbacAuthorizationvApi.md#replace_rbac_authorization_v1_cluster_role_binding) | **PUT** /apis/rbac.authorization.k8s.io/v1/clusterrolebindings/{name} | 
*RbacAuthorizationvApi* | [**replace_rbac_authorization_v1_namespaced_role**](docs/RbacAuthorizationvApi.md#replace_rbac_authorization_v1_namespaced_role) | **PUT** /apis/rbac.authorization.k8s.io/v1/namespaces/{namespace}/roles/{name} | 
*RbacAuthorizationvApi* | [**replace_rbac_authorization_v1_namespaced_role_binding**](docs/RbacAuthorizationvApi.md#replace_rbac_authorization_v1_namespaced_role_binding) | **PUT** /apis/rbac.authorization.k8s.io/v1/namespaces/{namespace}/rolebindings/{name} | 
*RbacAuthorizationvApi* | [**watch_rbac_authorization_v1_cluster_role**](docs/RbacAuthorizationvApi.md#watch_rbac_authorization_v1_cluster_role) | **GET** /apis/rbac.authorization.k8s.io/v1/watch/clusterroles/{name} | 
*RbacAuthorizationvApi* | [**watch_rbac_authorization_v1_cluster_role_binding**](docs/RbacAuthorizationvApi.md#watch_rbac_authorization_v1_cluster_role_binding) | **GET** /apis/rbac.authorization.k8s.io/v1/watch/clusterrolebindings/{name} | 
*RbacAuthorizationvApi* | [**watch_rbac_authorization_v1_cluster_role_binding_list**](docs/RbacAuthorizationvApi.md#watch_rbac_authorization_v1_cluster_role_binding_list) | **GET** /apis/rbac.authorization.k8s.io/v1/watch/clusterrolebindings | 
*RbacAuthorizationvApi* | [**watch_rbac_authorization_v1_cluster_role_list**](docs/RbacAuthorizationvApi.md#watch_rbac_authorization_v1_cluster_role_list) | **GET** /apis/rbac.authorization.k8s.io/v1/watch/clusterroles | 
*RbacAuthorizationvApi* | [**watch_rbac_authorization_v1_namespaced_role**](docs/RbacAuthorizationvApi.md#watch_rbac_authorization_v1_namespaced_role) | **GET** /apis/rbac.authorization.k8s.io/v1/watch/namespaces/{namespace}/roles/{name} | 
*RbacAuthorizationvApi* | [**watch_rbac_authorization_v1_namespaced_role_binding**](docs/RbacAuthorizationvApi.md#watch_rbac_authorization_v1_namespaced_role_binding) | **GET** /apis/rbac.authorization.k8s.io/v1/watch/namespaces/{namespace}/rolebindings/{name} | 
*RbacAuthorizationvApi* | [**watch_rbac_authorization_v1_namespaced_role_binding_list**](docs/RbacAuthorizationvApi.md#watch_rbac_authorization_v1_namespaced_role_binding_list) | **GET** /apis/rbac.authorization.k8s.io/v1/watch/namespaces/{namespace}/rolebindings | 
*RbacAuthorizationvApi* | [**watch_rbac_authorization_v1_namespaced_role_list**](docs/RbacAuthorizationvApi.md#watch_rbac_authorization_v1_namespaced_role_list) | **GET** /apis/rbac.authorization.k8s.io/v1/watch/namespaces/{namespace}/roles | 
*RbacAuthorizationvApi* | [**watch_rbac_authorization_v1_role_binding_list_for_all_namespaces**](docs/RbacAuthorizationvApi.md#watch_rbac_authorization_v1_role_binding_list_for_all_namespaces) | **GET** /apis/rbac.authorization.k8s.io/v1/watch/rolebindings | 
*RbacAuthorizationvApi* | [**watch_rbac_authorization_v1_role_list_for_all_namespaces**](docs/RbacAuthorizationvApi.md#watch_rbac_authorization_v1_role_list_for_all_namespaces) | **GET** /apis/rbac.authorization.k8s.io/v1/watch/roles | 
*ResourceApi* | [**get_resource_api_group**](docs/ResourceApi.md#get_resource_api_group) | **GET** /apis/resource.k8s.io/ | 
*ResourcevalphaApi* | [**create_resource_v1alpha1_namespaced_pod_scheduling**](docs/ResourcevalphaApi.md#create_resource_v1alpha1_namespaced_pod_scheduling) | **POST** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/podschedulings | 
*ResourcevalphaApi* | [**create_resource_v1alpha1_namespaced_resource_claim**](docs/ResourcevalphaApi.md#create_resource_v1alpha1_namespaced_resource_claim) | **POST** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaims | 
*ResourcevalphaApi* | [**create_resource_v1alpha1_namespaced_resource_claim_template**](docs/ResourcevalphaApi.md#create_resource_v1alpha1_namespaced_resource_claim_template) | **POST** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaimtemplates | 
*ResourcevalphaApi* | [**create_resource_v1alpha1_resource_class**](docs/ResourcevalphaApi.md#create_resource_v1alpha1_resource_class) | **POST** /apis/resource.k8s.io/v1alpha1/resourceclasses | 
*ResourcevalphaApi* | [**delete_resource_v1alpha1_collection_namespaced_pod_scheduling**](docs/ResourcevalphaApi.md#delete_resource_v1alpha1_collection_namespaced_pod_scheduling) | **DELETE** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/podschedulings | 
*ResourcevalphaApi* | [**delete_resource_v1alpha1_collection_namespaced_resource_claim**](docs/ResourcevalphaApi.md#delete_resource_v1alpha1_collection_namespaced_resource_claim) | **DELETE** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaims | 
*ResourcevalphaApi* | [**delete_resource_v1alpha1_collection_namespaced_resource_claim_template**](docs/ResourcevalphaApi.md#delete_resource_v1alpha1_collection_namespaced_resource_claim_template) | **DELETE** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaimtemplates | 
*ResourcevalphaApi* | [**delete_resource_v1alpha1_collection_resource_class**](docs/ResourcevalphaApi.md#delete_resource_v1alpha1_collection_resource_class) | **DELETE** /apis/resource.k8s.io/v1alpha1/resourceclasses | 
*ResourcevalphaApi* | [**delete_resource_v1alpha1_namespaced_pod_scheduling**](docs/ResourcevalphaApi.md#delete_resource_v1alpha1_namespaced_pod_scheduling) | **DELETE** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/podschedulings/{name} | 
*ResourcevalphaApi* | [**delete_resource_v1alpha1_namespaced_resource_claim**](docs/ResourcevalphaApi.md#delete_resource_v1alpha1_namespaced_resource_claim) | **DELETE** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaims/{name} | 
*ResourcevalphaApi* | [**delete_resource_v1alpha1_namespaced_resource_claim_template**](docs/ResourcevalphaApi.md#delete_resource_v1alpha1_namespaced_resource_claim_template) | **DELETE** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaimtemplates/{name} | 
*ResourcevalphaApi* | [**delete_resource_v1alpha1_resource_class**](docs/ResourcevalphaApi.md#delete_resource_v1alpha1_resource_class) | **DELETE** /apis/resource.k8s.io/v1alpha1/resourceclasses/{name} | 
*ResourcevalphaApi* | [**get_resource_v1alpha1_api_resources**](docs/ResourcevalphaApi.md#get_resource_v1alpha1_api_resources) | **GET** /apis/resource.k8s.io/v1alpha1/ | 
*ResourcevalphaApi* | [**list_resource_v1alpha1_namespaced_pod_scheduling**](docs/ResourcevalphaApi.md#list_resource_v1alpha1_namespaced_pod_scheduling) | **GET** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/podschedulings | 
*ResourcevalphaApi* | [**list_resource_v1alpha1_namespaced_resource_claim**](docs/ResourcevalphaApi.md#list_resource_v1alpha1_namespaced_resource_claim) | **GET** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaims | 
*ResourcevalphaApi* | [**list_resource_v1alpha1_namespaced_resource_claim_template**](docs/ResourcevalphaApi.md#list_resource_v1alpha1_namespaced_resource_claim_template) | **GET** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaimtemplates | 
*ResourcevalphaApi* | [**list_resource_v1alpha1_pod_scheduling_for_all_namespaces**](docs/ResourcevalphaApi.md#list_resource_v1alpha1_pod_scheduling_for_all_namespaces) | **GET** /apis/resource.k8s.io/v1alpha1/podschedulings | 
*ResourcevalphaApi* | [**list_resource_v1alpha1_resource_claim_for_all_namespaces**](docs/ResourcevalphaApi.md#list_resource_v1alpha1_resource_claim_for_all_namespaces) | **GET** /apis/resource.k8s.io/v1alpha1/resourceclaims | 
*ResourcevalphaApi* | [**list_resource_v1alpha1_resource_claim_template_for_all_namespaces**](docs/ResourcevalphaApi.md#list_resource_v1alpha1_resource_claim_template_for_all_namespaces) | **GET** /apis/resource.k8s.io/v1alpha1/resourceclaimtemplates | 
*ResourcevalphaApi* | [**list_resource_v1alpha1_resource_class**](docs/ResourcevalphaApi.md#list_resource_v1alpha1_resource_class) | **GET** /apis/resource.k8s.io/v1alpha1/resourceclasses | 
*ResourcevalphaApi* | [**patch_resource_v1alpha1_namespaced_pod_scheduling**](docs/ResourcevalphaApi.md#patch_resource_v1alpha1_namespaced_pod_scheduling) | **PATCH** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/podschedulings/{name} | 
*ResourcevalphaApi* | [**patch_resource_v1alpha1_namespaced_pod_scheduling_status**](docs/ResourcevalphaApi.md#patch_resource_v1alpha1_namespaced_pod_scheduling_status) | **PATCH** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/podschedulings/{name}/status | 
*ResourcevalphaApi* | [**patch_resource_v1alpha1_namespaced_resource_claim**](docs/ResourcevalphaApi.md#patch_resource_v1alpha1_namespaced_resource_claim) | **PATCH** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaims/{name} | 
*ResourcevalphaApi* | [**patch_resource_v1alpha1_namespaced_resource_claim_status**](docs/ResourcevalphaApi.md#patch_resource_v1alpha1_namespaced_resource_claim_status) | **PATCH** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaims/{name}/status | 
*ResourcevalphaApi* | [**patch_resource_v1alpha1_namespaced_resource_claim_template**](docs/ResourcevalphaApi.md#patch_resource_v1alpha1_namespaced_resource_claim_template) | **PATCH** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaimtemplates/{name} | 
*ResourcevalphaApi* | [**patch_resource_v1alpha1_resource_class**](docs/ResourcevalphaApi.md#patch_resource_v1alpha1_resource_class) | **PATCH** /apis/resource.k8s.io/v1alpha1/resourceclasses/{name} | 
*ResourcevalphaApi* | [**read_resource_v1alpha1_namespaced_pod_scheduling**](docs/ResourcevalphaApi.md#read_resource_v1alpha1_namespaced_pod_scheduling) | **GET** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/podschedulings/{name} | 
*ResourcevalphaApi* | [**read_resource_v1alpha1_namespaced_pod_scheduling_status**](docs/ResourcevalphaApi.md#read_resource_v1alpha1_namespaced_pod_scheduling_status) | **GET** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/podschedulings/{name}/status | 
*ResourcevalphaApi* | [**read_resource_v1alpha1_namespaced_resource_claim**](docs/ResourcevalphaApi.md#read_resource_v1alpha1_namespaced_resource_claim) | **GET** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaims/{name} | 
*ResourcevalphaApi* | [**read_resource_v1alpha1_namespaced_resource_claim_status**](docs/ResourcevalphaApi.md#read_resource_v1alpha1_namespaced_resource_claim_status) | **GET** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaims/{name}/status | 
*ResourcevalphaApi* | [**read_resource_v1alpha1_namespaced_resource_claim_template**](docs/ResourcevalphaApi.md#read_resource_v1alpha1_namespaced_resource_claim_template) | **GET** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaimtemplates/{name} | 
*ResourcevalphaApi* | [**read_resource_v1alpha1_resource_class**](docs/ResourcevalphaApi.md#read_resource_v1alpha1_resource_class) | **GET** /apis/resource.k8s.io/v1alpha1/resourceclasses/{name} | 
*ResourcevalphaApi* | [**replace_resource_v1alpha1_namespaced_pod_scheduling**](docs/ResourcevalphaApi.md#replace_resource_v1alpha1_namespaced_pod_scheduling) | **PUT** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/podschedulings/{name} | 
*ResourcevalphaApi* | [**replace_resource_v1alpha1_namespaced_pod_scheduling_status**](docs/ResourcevalphaApi.md#replace_resource_v1alpha1_namespaced_pod_scheduling_status) | **PUT** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/podschedulings/{name}/status | 
*ResourcevalphaApi* | [**replace_resource_v1alpha1_namespaced_resource_claim**](docs/ResourcevalphaApi.md#replace_resource_v1alpha1_namespaced_resource_claim) | **PUT** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaims/{name} | 
*ResourcevalphaApi* | [**replace_resource_v1alpha1_namespaced_resource_claim_status**](docs/ResourcevalphaApi.md#replace_resource_v1alpha1_namespaced_resource_claim_status) | **PUT** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaims/{name}/status | 
*ResourcevalphaApi* | [**replace_resource_v1alpha1_namespaced_resource_claim_template**](docs/ResourcevalphaApi.md#replace_resource_v1alpha1_namespaced_resource_claim_template) | **PUT** /apis/resource.k8s.io/v1alpha1/namespaces/{namespace}/resourceclaimtemplates/{name} | 
*ResourcevalphaApi* | [**replace_resource_v1alpha1_resource_class**](docs/ResourcevalphaApi.md#replace_resource_v1alpha1_resource_class) | **PUT** /apis/resource.k8s.io/v1alpha1/resourceclasses/{name} | 
*ResourcevalphaApi* | [**watch_resource_v1alpha1_namespaced_pod_scheduling**](docs/ResourcevalphaApi.md#watch_resource_v1alpha1_namespaced_pod_scheduling) | **GET** /apis/resource.k8s.io/v1alpha1/watch/namespaces/{namespace}/podschedulings/{name} | 
*ResourcevalphaApi* | [**watch_resource_v1alpha1_namespaced_pod_scheduling_list**](docs/ResourcevalphaApi.md#watch_resource_v1alpha1_namespaced_pod_scheduling_list) | **GET** /apis/resource.k8s.io/v1alpha1/watch/namespaces/{namespace}/podschedulings | 
*ResourcevalphaApi* | [**watch_resource_v1alpha1_namespaced_resource_claim**](docs/ResourcevalphaApi.md#watch_resource_v1alpha1_namespaced_resource_claim) | **GET** /apis/resource.k8s.io/v1alpha1/watch/namespaces/{namespace}/resourceclaims/{name} | 
*ResourcevalphaApi* | [**watch_resource_v1alpha1_namespaced_resource_claim_list**](docs/ResourcevalphaApi.md#watch_resource_v1alpha1_namespaced_resource_claim_list) | **GET** /apis/resource.k8s.io/v1alpha1/watch/namespaces/{namespace}/resourceclaims | 
*ResourcevalphaApi* | [**watch_resource_v1alpha1_namespaced_resource_claim_template**](docs/ResourcevalphaApi.md#watch_resource_v1alpha1_namespaced_resource_claim_template) | **GET** /apis/resource.k8s.io/v1alpha1/watch/namespaces/{namespace}/resourceclaimtemplates/{name} | 
*ResourcevalphaApi* | [**watch_resource_v1alpha1_namespaced_resource_claim_template_list**](docs/ResourcevalphaApi.md#watch_resource_v1alpha1_namespaced_resource_claim_template_list) | **GET** /apis/resource.k8s.io/v1alpha1/watch/namespaces/{namespace}/resourceclaimtemplates | 
*ResourcevalphaApi* | [**watch_resource_v1alpha1_pod_scheduling_list_for_all_namespaces**](docs/ResourcevalphaApi.md#watch_resource_v1alpha1_pod_scheduling_list_for_all_namespaces) | **GET** /apis/resource.k8s.io/v1alpha1/watch/podschedulings | 
*ResourcevalphaApi* | [**watch_resource_v1alpha1_resource_claim_list_for_all_namespaces**](docs/ResourcevalphaApi.md#watch_resource_v1alpha1_resource_claim_list_for_all_namespaces) | **GET** /apis/resource.k8s.io/v1alpha1/watch/resourceclaims | 
*ResourcevalphaApi* | [**watch_resource_v1alpha1_resource_claim_template_list_for_all_namespaces**](docs/ResourcevalphaApi.md#watch_resource_v1alpha1_resource_claim_template_list_for_all_namespaces) | **GET** /apis/resource.k8s.io/v1alpha1/watch/resourceclaimtemplates | 
*ResourcevalphaApi* | [**watch_resource_v1alpha1_resource_class**](docs/ResourcevalphaApi.md#watch_resource_v1alpha1_resource_class) | **GET** /apis/resource.k8s.io/v1alpha1/watch/resourceclasses/{name} | 
*ResourcevalphaApi* | [**watch_resource_v1alpha1_resource_class_list**](docs/ResourcevalphaApi.md#watch_resource_v1alpha1_resource_class_list) | **GET** /apis/resource.k8s.io/v1alpha1/watch/resourceclasses | 
*SchedulingApi* | [**get_scheduling_api_group**](docs/SchedulingApi.md#get_scheduling_api_group) | **GET** /apis/scheduling.k8s.io/ | 
*SchedulingvApi* | [**create_scheduling_v1_priority_class**](docs/SchedulingvApi.md#create_scheduling_v1_priority_class) | **POST** /apis/scheduling.k8s.io/v1/priorityclasses | 
*SchedulingvApi* | [**delete_scheduling_v1_collection_priority_class**](docs/SchedulingvApi.md#delete_scheduling_v1_collection_priority_class) | **DELETE** /apis/scheduling.k8s.io/v1/priorityclasses | 
*SchedulingvApi* | [**delete_scheduling_v1_priority_class**](docs/SchedulingvApi.md#delete_scheduling_v1_priority_class) | **DELETE** /apis/scheduling.k8s.io/v1/priorityclasses/{name} | 
*SchedulingvApi* | [**get_scheduling_v1_api_resources**](docs/SchedulingvApi.md#get_scheduling_v1_api_resources) | **GET** /apis/scheduling.k8s.io/v1/ | 
*SchedulingvApi* | [**list_scheduling_v1_priority_class**](docs/SchedulingvApi.md#list_scheduling_v1_priority_class) | **GET** /apis/scheduling.k8s.io/v1/priorityclasses | 
*SchedulingvApi* | [**patch_scheduling_v1_priority_class**](docs/SchedulingvApi.md#patch_scheduling_v1_priority_class) | **PATCH** /apis/scheduling.k8s.io/v1/priorityclasses/{name} | 
*SchedulingvApi* | [**read_scheduling_v1_priority_class**](docs/SchedulingvApi.md#read_scheduling_v1_priority_class) | **GET** /apis/scheduling.k8s.io/v1/priorityclasses/{name} | 
*SchedulingvApi* | [**replace_scheduling_v1_priority_class**](docs/SchedulingvApi.md#replace_scheduling_v1_priority_class) | **PUT** /apis/scheduling.k8s.io/v1/priorityclasses/{name} | 
*SchedulingvApi* | [**watch_scheduling_v1_priority_class**](docs/SchedulingvApi.md#watch_scheduling_v1_priority_class) | **GET** /apis/scheduling.k8s.io/v1/watch/priorityclasses/{name} | 
*SchedulingvApi* | [**watch_scheduling_v1_priority_class_list**](docs/SchedulingvApi.md#watch_scheduling_v1_priority_class_list) | **GET** /apis/scheduling.k8s.io/v1/watch/priorityclasses | 
*StorageApi* | [**get_storage_api_group**](docs/StorageApi.md#get_storage_api_group) | **GET** /apis/storage.k8s.io/ | 
*StoragevApi* | [**create_storage_v1_csi_driver**](docs/StoragevApi.md#create_storage_v1_csi_driver) | **POST** /apis/storage.k8s.io/v1/csidrivers | 
*StoragevApi* | [**create_storage_v1_csi_node**](docs/StoragevApi.md#create_storage_v1_csi_node) | **POST** /apis/storage.k8s.io/v1/csinodes | 
*StoragevApi* | [**create_storage_v1_namespaced_csi_storage_capacity**](docs/StoragevApi.md#create_storage_v1_namespaced_csi_storage_capacity) | **POST** /apis/storage.k8s.io/v1/namespaces/{namespace}/csistoragecapacities | 
*StoragevApi* | [**create_storage_v1_storage_class**](docs/StoragevApi.md#create_storage_v1_storage_class) | **POST** /apis/storage.k8s.io/v1/storageclasses | 
*StoragevApi* | [**create_storage_v1_volume_attachment**](docs/StoragevApi.md#create_storage_v1_volume_attachment) | **POST** /apis/storage.k8s.io/v1/volumeattachments | 
*StoragevApi* | [**delete_storage_v1_collection_csi_driver**](docs/StoragevApi.md#delete_storage_v1_collection_csi_driver) | **DELETE** /apis/storage.k8s.io/v1/csidrivers | 
*StoragevApi* | [**delete_storage_v1_collection_csi_node**](docs/StoragevApi.md#delete_storage_v1_collection_csi_node) | **DELETE** /apis/storage.k8s.io/v1/csinodes | 
*StoragevApi* | [**delete_storage_v1_collection_namespaced_csi_storage_capacity**](docs/StoragevApi.md#delete_storage_v1_collection_namespaced_csi_storage_capacity) | **DELETE** /apis/storage.k8s.io/v1/namespaces/{namespace}/csistoragecapacities | 
*StoragevApi* | [**delete_storage_v1_collection_storage_class**](docs/StoragevApi.md#delete_storage_v1_collection_storage_class) | **DELETE** /apis/storage.k8s.io/v1/storageclasses | 
*StoragevApi* | [**delete_storage_v1_collection_volume_attachment**](docs/StoragevApi.md#delete_storage_v1_collection_volume_attachment) | **DELETE** /apis/storage.k8s.io/v1/volumeattachments | 
*StoragevApi* | [**delete_storage_v1_csi_driver**](docs/StoragevApi.md#delete_storage_v1_csi_driver) | **DELETE** /apis/storage.k8s.io/v1/csidrivers/{name} | 
*StoragevApi* | [**delete_storage_v1_csi_node**](docs/StoragevApi.md#delete_storage_v1_csi_node) | **DELETE** /apis/storage.k8s.io/v1/csinodes/{name} | 
*StoragevApi* | [**delete_storage_v1_namespaced_csi_storage_capacity**](docs/StoragevApi.md#delete_storage_v1_namespaced_csi_storage_capacity) | **DELETE** /apis/storage.k8s.io/v1/namespaces/{namespace}/csistoragecapacities/{name} | 
*StoragevApi* | [**delete_storage_v1_storage_class**](docs/StoragevApi.md#delete_storage_v1_storage_class) | **DELETE** /apis/storage.k8s.io/v1/storageclasses/{name} | 
*StoragevApi* | [**delete_storage_v1_volume_attachment**](docs/StoragevApi.md#delete_storage_v1_volume_attachment) | **DELETE** /apis/storage.k8s.io/v1/volumeattachments/{name} | 
*StoragevApi* | [**get_storage_v1_api_resources**](docs/StoragevApi.md#get_storage_v1_api_resources) | **GET** /apis/storage.k8s.io/v1/ | 
*StoragevApi* | [**list_storage_v1_csi_driver**](docs/StoragevApi.md#list_storage_v1_csi_driver) | **GET** /apis/storage.k8s.io/v1/csidrivers | 
*StoragevApi* | [**list_storage_v1_csi_node**](docs/StoragevApi.md#list_storage_v1_csi_node) | **GET** /apis/storage.k8s.io/v1/csinodes | 
*StoragevApi* | [**list_storage_v1_csi_storage_capacity_for_all_namespaces**](docs/StoragevApi.md#list_storage_v1_csi_storage_capacity_for_all_namespaces) | **GET** /apis/storage.k8s.io/v1/csistoragecapacities | 
*StoragevApi* | [**list_storage_v1_namespaced_csi_storage_capacity**](docs/StoragevApi.md#list_storage_v1_namespaced_csi_storage_capacity) | **GET** /apis/storage.k8s.io/v1/namespaces/{namespace}/csistoragecapacities | 
*StoragevApi* | [**list_storage_v1_storage_class**](docs/StoragevApi.md#list_storage_v1_storage_class) | **GET** /apis/storage.k8s.io/v1/storageclasses | 
*StoragevApi* | [**list_storage_v1_volume_attachment**](docs/StoragevApi.md#list_storage_v1_volume_attachment) | **GET** /apis/storage.k8s.io/v1/volumeattachments | 
*StoragevApi* | [**patch_storage_v1_csi_driver**](docs/StoragevApi.md#patch_storage_v1_csi_driver) | **PATCH** /apis/storage.k8s.io/v1/csidrivers/{name} | 
*StoragevApi* | [**patch_storage_v1_csi_node**](docs/StoragevApi.md#patch_storage_v1_csi_node) | **PATCH** /apis/storage.k8s.io/v1/csinodes/{name} | 
*StoragevApi* | [**patch_storage_v1_namespaced_csi_storage_capacity**](docs/StoragevApi.md#patch_storage_v1_namespaced_csi_storage_capacity) | **PATCH** /apis/storage.k8s.io/v1/namespaces/{namespace}/csistoragecapacities/{name} | 
*StoragevApi* | [**patch_storage_v1_storage_class**](docs/StoragevApi.md#patch_storage_v1_storage_class) | **PATCH** /apis/storage.k8s.io/v1/storageclasses/{name} | 
*StoragevApi* | [**patch_storage_v1_volume_attachment**](docs/StoragevApi.md#patch_storage_v1_volume_attachment) | **PATCH** /apis/storage.k8s.io/v1/volumeattachments/{name} | 
*StoragevApi* | [**patch_storage_v1_volume_attachment_status**](docs/StoragevApi.md#patch_storage_v1_volume_attachment_status) | **PATCH** /apis/storage.k8s.io/v1/volumeattachments/{name}/status | 
*StoragevApi* | [**read_storage_v1_csi_driver**](docs/StoragevApi.md#read_storage_v1_csi_driver) | **GET** /apis/storage.k8s.io/v1/csidrivers/{name} | 
*StoragevApi* | [**read_storage_v1_csi_node**](docs/StoragevApi.md#read_storage_v1_csi_node) | **GET** /apis/storage.k8s.io/v1/csinodes/{name} | 
*StoragevApi* | [**read_storage_v1_namespaced_csi_storage_capacity**](docs/StoragevApi.md#read_storage_v1_namespaced_csi_storage_capacity) | **GET** /apis/storage.k8s.io/v1/namespaces/{namespace}/csistoragecapacities/{name} | 
*StoragevApi* | [**read_storage_v1_storage_class**](docs/StoragevApi.md#read_storage_v1_storage_class) | **GET** /apis/storage.k8s.io/v1/storageclasses/{name} | 
*StoragevApi* | [**read_storage_v1_volume_attachment**](docs/StoragevApi.md#read_storage_v1_volume_attachment) | **GET** /apis/storage.k8s.io/v1/volumeattachments/{name} | 
*StoragevApi* | [**read_storage_v1_volume_attachment_status**](docs/StoragevApi.md#read_storage_v1_volume_attachment_status) | **GET** /apis/storage.k8s.io/v1/volumeattachments/{name}/status | 
*StoragevApi* | [**replace_storage_v1_csi_driver**](docs/StoragevApi.md#replace_storage_v1_csi_driver) | **PUT** /apis/storage.k8s.io/v1/csidrivers/{name} | 
*StoragevApi* | [**replace_storage_v1_csi_node**](docs/StoragevApi.md#replace_storage_v1_csi_node) | **PUT** /apis/storage.k8s.io/v1/csinodes/{name} | 
*StoragevApi* | [**replace_storage_v1_namespaced_csi_storage_capacity**](docs/StoragevApi.md#replace_storage_v1_namespaced_csi_storage_capacity) | **PUT** /apis/storage.k8s.io/v1/namespaces/{namespace}/csistoragecapacities/{name} | 
*StoragevApi* | [**replace_storage_v1_storage_class**](docs/StoragevApi.md#replace_storage_v1_storage_class) | **PUT** /apis/storage.k8s.io/v1/storageclasses/{name} | 
*StoragevApi* | [**replace_storage_v1_volume_attachment**](docs/StoragevApi.md#replace_storage_v1_volume_attachment) | **PUT** /apis/storage.k8s.io/v1/volumeattachments/{name} | 
*StoragevApi* | [**replace_storage_v1_volume_attachment_status**](docs/StoragevApi.md#replace_storage_v1_volume_attachment_status) | **PUT** /apis/storage.k8s.io/v1/volumeattachments/{name}/status | 
*StoragevApi* | [**watch_storage_v1_csi_driver**](docs/StoragevApi.md#watch_storage_v1_csi_driver) | **GET** /apis/storage.k8s.io/v1/watch/csidrivers/{name} | 
*StoragevApi* | [**watch_storage_v1_csi_driver_list**](docs/StoragevApi.md#watch_storage_v1_csi_driver_list) | **GET** /apis/storage.k8s.io/v1/watch/csidrivers | 
*StoragevApi* | [**watch_storage_v1_csi_node**](docs/StoragevApi.md#watch_storage_v1_csi_node) | **GET** /apis/storage.k8s.io/v1/watch/csinodes/{name} | 
*StoragevApi* | [**watch_storage_v1_csi_node_list**](docs/StoragevApi.md#watch_storage_v1_csi_node_list) | **GET** /apis/storage.k8s.io/v1/watch/csinodes | 
*StoragevApi* | [**watch_storage_v1_csi_storage_capacity_list_for_all_namespaces**](docs/StoragevApi.md#watch_storage_v1_csi_storage_capacity_list_for_all_namespaces) | **GET** /apis/storage.k8s.io/v1/watch/csistoragecapacities | 
*StoragevApi* | [**watch_storage_v1_namespaced_csi_storage_capacity**](docs/StoragevApi.md#watch_storage_v1_namespaced_csi_storage_capacity) | **GET** /apis/storage.k8s.io/v1/watch/namespaces/{namespace}/csistoragecapacities/{name} | 
*StoragevApi* | [**watch_storage_v1_namespaced_csi_storage_capacity_list**](docs/StoragevApi.md#watch_storage_v1_namespaced_csi_storage_capacity_list) | **GET** /apis/storage.k8s.io/v1/watch/namespaces/{namespace}/csistoragecapacities | 
*StoragevApi* | [**watch_storage_v1_storage_class**](docs/StoragevApi.md#watch_storage_v1_storage_class) | **GET** /apis/storage.k8s.io/v1/watch/storageclasses/{name} | 
*StoragevApi* | [**watch_storage_v1_storage_class_list**](docs/StoragevApi.md#watch_storage_v1_storage_class_list) | **GET** /apis/storage.k8s.io/v1/watch/storageclasses | 
*StoragevApi* | [**watch_storage_v1_volume_attachment**](docs/StoragevApi.md#watch_storage_v1_volume_attachment) | **GET** /apis/storage.k8s.io/v1/watch/volumeattachments/{name} | 
*StoragevApi* | [**watch_storage_v1_volume_attachment_list**](docs/StoragevApi.md#watch_storage_v1_volume_attachment_list) | **GET** /apis/storage.k8s.io/v1/watch/volumeattachments | 
*StoragevbetaApi* | [**create_storage_v1beta1_namespaced_csi_storage_capacity**](docs/StoragevbetaApi.md#create_storage_v1beta1_namespaced_csi_storage_capacity) | **POST** /apis/storage.k8s.io/v1beta1/namespaces/{namespace}/csistoragecapacities | 
*StoragevbetaApi* | [**delete_storage_v1beta1_collection_namespaced_csi_storage_capacity**](docs/StoragevbetaApi.md#delete_storage_v1beta1_collection_namespaced_csi_storage_capacity) | **DELETE** /apis/storage.k8s.io/v1beta1/namespaces/{namespace}/csistoragecapacities | 
*StoragevbetaApi* | [**delete_storage_v1beta1_namespaced_csi_storage_capacity**](docs/StoragevbetaApi.md#delete_storage_v1beta1_namespaced_csi_storage_capacity) | **DELETE** /apis/storage.k8s.io/v1beta1/namespaces/{namespace}/csistoragecapacities/{name} | 
*StoragevbetaApi* | [**get_storage_v1beta1_api_resources**](docs/StoragevbetaApi.md#get_storage_v1beta1_api_resources) | **GET** /apis/storage.k8s.io/v1beta1/ | 
*StoragevbetaApi* | [**list_storage_v1beta1_csi_storage_capacity_for_all_namespaces**](docs/StoragevbetaApi.md#list_storage_v1beta1_csi_storage_capacity_for_all_namespaces) | **GET** /apis/storage.k8s.io/v1beta1/csistoragecapacities | 
*StoragevbetaApi* | [**list_storage_v1beta1_namespaced_csi_storage_capacity**](docs/StoragevbetaApi.md#list_storage_v1beta1_namespaced_csi_storage_capacity) | **GET** /apis/storage.k8s.io/v1beta1/namespaces/{namespace}/csistoragecapacities | 
*StoragevbetaApi* | [**patch_storage_v1beta1_namespaced_csi_storage_capacity**](docs/StoragevbetaApi.md#patch_storage_v1beta1_namespaced_csi_storage_capacity) | **PATCH** /apis/storage.k8s.io/v1beta1/namespaces/{namespace}/csistoragecapacities/{name} | 
*StoragevbetaApi* | [**read_storage_v1beta1_namespaced_csi_storage_capacity**](docs/StoragevbetaApi.md#read_storage_v1beta1_namespaced_csi_storage_capacity) | **GET** /apis/storage.k8s.io/v1beta1/namespaces/{namespace}/csistoragecapacities/{name} | 
*StoragevbetaApi* | [**replace_storage_v1beta1_namespaced_csi_storage_capacity**](docs/StoragevbetaApi.md#replace_storage_v1beta1_namespaced_csi_storage_capacity) | **PUT** /apis/storage.k8s.io/v1beta1/namespaces/{namespace}/csistoragecapacities/{name} | 
*StoragevbetaApi* | [**watch_storage_v1beta1_csi_storage_capacity_list_for_all_namespaces**](docs/StoragevbetaApi.md#watch_storage_v1beta1_csi_storage_capacity_list_for_all_namespaces) | **GET** /apis/storage.k8s.io/v1beta1/watch/csistoragecapacities | 
*StoragevbetaApi* | [**watch_storage_v1beta1_namespaced_csi_storage_capacity**](docs/StoragevbetaApi.md#watch_storage_v1beta1_namespaced_csi_storage_capacity) | **GET** /apis/storage.k8s.io/v1beta1/watch/namespaces/{namespace}/csistoragecapacities/{name} | 
*StoragevbetaApi* | [**watch_storage_v1beta1_namespaced_csi_storage_capacity_list**](docs/StoragevbetaApi.md#watch_storage_v1beta1_namespaced_csi_storage_capacity_list) | **GET** /apis/storage.k8s.io/v1beta1/watch/namespaces/{namespace}/csistoragecapacities | 
*VersionApi* | [**get_code_version**](docs/VersionApi.md#get_code_version) | **GET** /version/ | 
*WellKnownApi* | [**get_service_account_issuer_open_id_configuration**](docs/WellKnownApi.md#get_service_account_issuer_open_id_configuration) | **GET** /.well-known/openid-configuration/ | 


## Documentation For Models

 - [IoK8sApiAdmissionregistrationV1MutatingWebhook](docs/IoK8sApiAdmissionregistrationV1MutatingWebhook.md)
 - [IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration](docs/IoK8sApiAdmissionregistrationV1MutatingWebhookConfiguration.md)
 - [IoK8sApiAdmissionregistrationV1MutatingWebhookConfigurationList](docs/IoK8sApiAdmissionregistrationV1MutatingWebhookConfigurationList.md)
 - [IoK8sApiAdmissionregistrationV1RuleWithOperations](docs/IoK8sApiAdmissionregistrationV1RuleWithOperations.md)
 - [IoK8sApiAdmissionregistrationV1ServiceReference](docs/IoK8sApiAdmissionregistrationV1ServiceReference.md)
 - [IoK8sApiAdmissionregistrationV1ValidatingWebhook](docs/IoK8sApiAdmissionregistrationV1ValidatingWebhook.md)
 - [IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration](docs/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfiguration.md)
 - [IoK8sApiAdmissionregistrationV1ValidatingWebhookConfigurationList](docs/IoK8sApiAdmissionregistrationV1ValidatingWebhookConfigurationList.md)
 - [IoK8sApiAdmissionregistrationV1WebhookClientConfig](docs/IoK8sApiAdmissionregistrationV1WebhookClientConfig.md)
 - [IoK8sApiAdmissionregistrationV1alpha1MatchResources](docs/IoK8sApiAdmissionregistrationV1alpha1MatchResources.md)
 - [IoK8sApiAdmissionregistrationV1alpha1NamedRuleWithOperations](docs/IoK8sApiAdmissionregistrationV1alpha1NamedRuleWithOperations.md)
 - [IoK8sApiAdmissionregistrationV1alpha1ParamKind](docs/IoK8sApiAdmissionregistrationV1alpha1ParamKind.md)
 - [IoK8sApiAdmissionregistrationV1alpha1ParamRef](docs/IoK8sApiAdmissionregistrationV1alpha1ParamRef.md)
 - [IoK8sApiAdmissionregistrationV1alpha1ValidatingAdmissionPolicy](docs/IoK8sApiAdmissionregistrationV1alpha1ValidatingAdmissionPolicy.md)
 - [IoK8sApiAdmissionregistrationV1alpha1ValidatingAdmissionPolicyBinding](docs/IoK8sApiAdmissionregistrationV1alpha1ValidatingAdmissionPolicyBinding.md)
 - [IoK8sApiAdmissionregistrationV1alpha1ValidatingAdmissionPolicyBindingList](docs/IoK8sApiAdmissionregistrationV1alpha1ValidatingAdmissionPolicyBindingList.md)
 - [IoK8sApiAdmissionregistrationV1alpha1ValidatingAdmissionPolicyBindingSpec](docs/IoK8sApiAdmissionregistrationV1alpha1ValidatingAdmissionPolicyBindingSpec.md)
 - [IoK8sApiAdmissionregistrationV1alpha1ValidatingAdmissionPolicyList](docs/IoK8sApiAdmissionregistrationV1alpha1ValidatingAdmissionPolicyList.md)
 - [IoK8sApiAdmissionregistrationV1alpha1ValidatingAdmissionPolicySpec](docs/IoK8sApiAdmissionregistrationV1alpha1ValidatingAdmissionPolicySpec.md)
 - [IoK8sApiAdmissionregistrationV1alpha1Validation](docs/IoK8sApiAdmissionregistrationV1alpha1Validation.md)
 - [IoK8sApiApiserverinternalV1alpha1ServerStorageVersion](docs/IoK8sApiApiserverinternalV1alpha1ServerStorageVersion.md)
 - [IoK8sApiApiserverinternalV1alpha1StorageVersion](docs/IoK8sApiApiserverinternalV1alpha1StorageVersion.md)
 - [IoK8sApiApiserverinternalV1alpha1StorageVersionCondition](docs/IoK8sApiApiserverinternalV1alpha1StorageVersionCondition.md)
 - [IoK8sApiApiserverinternalV1alpha1StorageVersionList](docs/IoK8sApiApiserverinternalV1alpha1StorageVersionList.md)
 - [IoK8sApiApiserverinternalV1alpha1StorageVersionSpec](docs/IoK8sApiApiserverinternalV1alpha1StorageVersionSpec.md)
 - [IoK8sApiApiserverinternalV1alpha1StorageVersionStatus](docs/IoK8sApiApiserverinternalV1alpha1StorageVersionStatus.md)
 - [IoK8sApiAppsV1ControllerRevision](docs/IoK8sApiAppsV1ControllerRevision.md)
 - [IoK8sApiAppsV1ControllerRevisionList](docs/IoK8sApiAppsV1ControllerRevisionList.md)
 - [IoK8sApiAppsV1DaemonSet](docs/IoK8sApiAppsV1DaemonSet.md)
 - [IoK8sApiAppsV1DaemonSetCondition](docs/IoK8sApiAppsV1DaemonSetCondition.md)
 - [IoK8sApiAppsV1DaemonSetList](docs/IoK8sApiAppsV1DaemonSetList.md)
 - [IoK8sApiAppsV1DaemonSetSpec](docs/IoK8sApiAppsV1DaemonSetSpec.md)
 - [IoK8sApiAppsV1DaemonSetStatus](docs/IoK8sApiAppsV1DaemonSetStatus.md)
 - [IoK8sApiAppsV1DaemonSetUpdateStrategy](docs/IoK8sApiAppsV1DaemonSetUpdateStrategy.md)
 - [IoK8sApiAppsV1Deployment](docs/IoK8sApiAppsV1Deployment.md)
 - [IoK8sApiAppsV1DeploymentCondition](docs/IoK8sApiAppsV1DeploymentCondition.md)
 - [IoK8sApiAppsV1DeploymentList](docs/IoK8sApiAppsV1DeploymentList.md)
 - [IoK8sApiAppsV1DeploymentSpec](docs/IoK8sApiAppsV1DeploymentSpec.md)
 - [IoK8sApiAppsV1DeploymentStatus](docs/IoK8sApiAppsV1DeploymentStatus.md)
 - [IoK8sApiAppsV1DeploymentStrategy](docs/IoK8sApiAppsV1DeploymentStrategy.md)
 - [IoK8sApiAppsV1ReplicaSet](docs/IoK8sApiAppsV1ReplicaSet.md)
 - [IoK8sApiAppsV1ReplicaSetCondition](docs/IoK8sApiAppsV1ReplicaSetCondition.md)
 - [IoK8sApiAppsV1ReplicaSetList](docs/IoK8sApiAppsV1ReplicaSetList.md)
 - [IoK8sApiAppsV1ReplicaSetSpec](docs/IoK8sApiAppsV1ReplicaSetSpec.md)
 - [IoK8sApiAppsV1ReplicaSetStatus](docs/IoK8sApiAppsV1ReplicaSetStatus.md)
 - [IoK8sApiAppsV1RollingUpdateDaemonSet](docs/IoK8sApiAppsV1RollingUpdateDaemonSet.md)
 - [IoK8sApiAppsV1RollingUpdateDeployment](docs/IoK8sApiAppsV1RollingUpdateDeployment.md)
 - [IoK8sApiAppsV1RollingUpdateStatefulSetStrategy](docs/IoK8sApiAppsV1RollingUpdateStatefulSetStrategy.md)
 - [IoK8sApiAppsV1StatefulSet](docs/IoK8sApiAppsV1StatefulSet.md)
 - [IoK8sApiAppsV1StatefulSetCondition](docs/IoK8sApiAppsV1StatefulSetCondition.md)
 - [IoK8sApiAppsV1StatefulSetList](docs/IoK8sApiAppsV1StatefulSetList.md)
 - [IoK8sApiAppsV1StatefulSetOrdinals](docs/IoK8sApiAppsV1StatefulSetOrdinals.md)
 - [IoK8sApiAppsV1StatefulSetPersistentVolumeClaimRetentionPolicy](docs/IoK8sApiAppsV1StatefulSetPersistentVolumeClaimRetentionPolicy.md)
 - [IoK8sApiAppsV1StatefulSetSpec](docs/IoK8sApiAppsV1StatefulSetSpec.md)
 - [IoK8sApiAppsV1StatefulSetStatus](docs/IoK8sApiAppsV1StatefulSetStatus.md)
 - [IoK8sApiAppsV1StatefulSetUpdateStrategy](docs/IoK8sApiAppsV1StatefulSetUpdateStrategy.md)
 - [IoK8sApiAuthenticationV1BoundObjectReference](docs/IoK8sApiAuthenticationV1BoundObjectReference.md)
 - [IoK8sApiAuthenticationV1TokenRequest](docs/IoK8sApiAuthenticationV1TokenRequest.md)
 - [IoK8sApiAuthenticationV1TokenRequestSpec](docs/IoK8sApiAuthenticationV1TokenRequestSpec.md)
 - [IoK8sApiAuthenticationV1TokenRequestStatus](docs/IoK8sApiAuthenticationV1TokenRequestStatus.md)
 - [IoK8sApiAuthenticationV1TokenReview](docs/IoK8sApiAuthenticationV1TokenReview.md)
 - [IoK8sApiAuthenticationV1TokenReviewSpec](docs/IoK8sApiAuthenticationV1TokenReviewSpec.md)
 - [IoK8sApiAuthenticationV1TokenReviewStatus](docs/IoK8sApiAuthenticationV1TokenReviewStatus.md)
 - [IoK8sApiAuthenticationV1UserInfo](docs/IoK8sApiAuthenticationV1UserInfo.md)
 - [IoK8sApiAuthenticationV1alpha1SelfSubjectReview](docs/IoK8sApiAuthenticationV1alpha1SelfSubjectReview.md)
 - [IoK8sApiAuthenticationV1alpha1SelfSubjectReviewStatus](docs/IoK8sApiAuthenticationV1alpha1SelfSubjectReviewStatus.md)
 - [IoK8sApiAuthorizationV1LocalSubjectAccessReview](docs/IoK8sApiAuthorizationV1LocalSubjectAccessReview.md)
 - [IoK8sApiAuthorizationV1NonResourceAttributes](docs/IoK8sApiAuthorizationV1NonResourceAttributes.md)
 - [IoK8sApiAuthorizationV1NonResourceRule](docs/IoK8sApiAuthorizationV1NonResourceRule.md)
 - [IoK8sApiAuthorizationV1ResourceAttributes](docs/IoK8sApiAuthorizationV1ResourceAttributes.md)
 - [IoK8sApiAuthorizationV1ResourceRule](docs/IoK8sApiAuthorizationV1ResourceRule.md)
 - [IoK8sApiAuthorizationV1SelfSubjectAccessReview](docs/IoK8sApiAuthorizationV1SelfSubjectAccessReview.md)
 - [IoK8sApiAuthorizationV1SelfSubjectAccessReviewSpec](docs/IoK8sApiAuthorizationV1SelfSubjectAccessReviewSpec.md)
 - [IoK8sApiAuthorizationV1SelfSubjectRulesReview](docs/IoK8sApiAuthorizationV1SelfSubjectRulesReview.md)
 - [IoK8sApiAuthorizationV1SelfSubjectRulesReviewSpec](docs/IoK8sApiAuthorizationV1SelfSubjectRulesReviewSpec.md)
 - [IoK8sApiAuthorizationV1SubjectAccessReview](docs/IoK8sApiAuthorizationV1SubjectAccessReview.md)
 - [IoK8sApiAuthorizationV1SubjectAccessReviewSpec](docs/IoK8sApiAuthorizationV1SubjectAccessReviewSpec.md)
 - [IoK8sApiAuthorizationV1SubjectAccessReviewStatus](docs/IoK8sApiAuthorizationV1SubjectAccessReviewStatus.md)
 - [IoK8sApiAuthorizationV1SubjectRulesReviewStatus](docs/IoK8sApiAuthorizationV1SubjectRulesReviewStatus.md)
 - [IoK8sApiAutoscalingV1CrossVersionObjectReference](docs/IoK8sApiAutoscalingV1CrossVersionObjectReference.md)
 - [IoK8sApiAutoscalingV1HorizontalPodAutoscaler](docs/IoK8sApiAutoscalingV1HorizontalPodAutoscaler.md)
 - [IoK8sApiAutoscalingV1HorizontalPodAutoscalerList](docs/IoK8sApiAutoscalingV1HorizontalPodAutoscalerList.md)
 - [IoK8sApiAutoscalingV1HorizontalPodAutoscalerSpec](docs/IoK8sApiAutoscalingV1HorizontalPodAutoscalerSpec.md)
 - [IoK8sApiAutoscalingV1HorizontalPodAutoscalerStatus](docs/IoK8sApiAutoscalingV1HorizontalPodAutoscalerStatus.md)
 - [IoK8sApiAutoscalingV1Scale](docs/IoK8sApiAutoscalingV1Scale.md)
 - [IoK8sApiAutoscalingV1ScaleSpec](docs/IoK8sApiAutoscalingV1ScaleSpec.md)
 - [IoK8sApiAutoscalingV1ScaleStatus](docs/IoK8sApiAutoscalingV1ScaleStatus.md)
 - [IoK8sApiAutoscalingV2ContainerResourceMetricSource](docs/IoK8sApiAutoscalingV2ContainerResourceMetricSource.md)
 - [IoK8sApiAutoscalingV2ContainerResourceMetricStatus](docs/IoK8sApiAutoscalingV2ContainerResourceMetricStatus.md)
 - [IoK8sApiAutoscalingV2CrossVersionObjectReference](docs/IoK8sApiAutoscalingV2CrossVersionObjectReference.md)
 - [IoK8sApiAutoscalingV2ExternalMetricSource](docs/IoK8sApiAutoscalingV2ExternalMetricSource.md)
 - [IoK8sApiAutoscalingV2ExternalMetricStatus](docs/IoK8sApiAutoscalingV2ExternalMetricStatus.md)
 - [IoK8sApiAutoscalingV2HPAScalingPolicy](docs/IoK8sApiAutoscalingV2HPAScalingPolicy.md)
 - [IoK8sApiAutoscalingV2HPAScalingRules](docs/IoK8sApiAutoscalingV2HPAScalingRules.md)
 - [IoK8sApiAutoscalingV2HorizontalPodAutoscaler](docs/IoK8sApiAutoscalingV2HorizontalPodAutoscaler.md)
 - [IoK8sApiAutoscalingV2HorizontalPodAutoscalerBehavior](docs/IoK8sApiAutoscalingV2HorizontalPodAutoscalerBehavior.md)
 - [IoK8sApiAutoscalingV2HorizontalPodAutoscalerCondition](docs/IoK8sApiAutoscalingV2HorizontalPodAutoscalerCondition.md)
 - [IoK8sApiAutoscalingV2HorizontalPodAutoscalerList](docs/IoK8sApiAutoscalingV2HorizontalPodAutoscalerList.md)
 - [IoK8sApiAutoscalingV2HorizontalPodAutoscalerSpec](docs/IoK8sApiAutoscalingV2HorizontalPodAutoscalerSpec.md)
 - [IoK8sApiAutoscalingV2HorizontalPodAutoscalerStatus](docs/IoK8sApiAutoscalingV2HorizontalPodAutoscalerStatus.md)
 - [IoK8sApiAutoscalingV2MetricIdentifier](docs/IoK8sApiAutoscalingV2MetricIdentifier.md)
 - [IoK8sApiAutoscalingV2MetricSpec](docs/IoK8sApiAutoscalingV2MetricSpec.md)
 - [IoK8sApiAutoscalingV2MetricStatus](docs/IoK8sApiAutoscalingV2MetricStatus.md)
 - [IoK8sApiAutoscalingV2MetricTarget](docs/IoK8sApiAutoscalingV2MetricTarget.md)
 - [IoK8sApiAutoscalingV2MetricValueStatus](docs/IoK8sApiAutoscalingV2MetricValueStatus.md)
 - [IoK8sApiAutoscalingV2ObjectMetricSource](docs/IoK8sApiAutoscalingV2ObjectMetricSource.md)
 - [IoK8sApiAutoscalingV2ObjectMetricStatus](docs/IoK8sApiAutoscalingV2ObjectMetricStatus.md)
 - [IoK8sApiAutoscalingV2PodsMetricSource](docs/IoK8sApiAutoscalingV2PodsMetricSource.md)
 - [IoK8sApiAutoscalingV2PodsMetricStatus](docs/IoK8sApiAutoscalingV2PodsMetricStatus.md)
 - [IoK8sApiAutoscalingV2ResourceMetricSource](docs/IoK8sApiAutoscalingV2ResourceMetricSource.md)
 - [IoK8sApiAutoscalingV2ResourceMetricStatus](docs/IoK8sApiAutoscalingV2ResourceMetricStatus.md)
 - [IoK8sApiBatchV1CronJob](docs/IoK8sApiBatchV1CronJob.md)
 - [IoK8sApiBatchV1CronJobList](docs/IoK8sApiBatchV1CronJobList.md)
 - [IoK8sApiBatchV1CronJobSpec](docs/IoK8sApiBatchV1CronJobSpec.md)
 - [IoK8sApiBatchV1CronJobStatus](docs/IoK8sApiBatchV1CronJobStatus.md)
 - [IoK8sApiBatchV1Job](docs/IoK8sApiBatchV1Job.md)
 - [IoK8sApiBatchV1JobCondition](docs/IoK8sApiBatchV1JobCondition.md)
 - [IoK8sApiBatchV1JobList](docs/IoK8sApiBatchV1JobList.md)
 - [IoK8sApiBatchV1JobSpec](docs/IoK8sApiBatchV1JobSpec.md)
 - [IoK8sApiBatchV1JobStatus](docs/IoK8sApiBatchV1JobStatus.md)
 - [IoK8sApiBatchV1JobTemplateSpec](docs/IoK8sApiBatchV1JobTemplateSpec.md)
 - [IoK8sApiBatchV1PodFailurePolicy](docs/IoK8sApiBatchV1PodFailurePolicy.md)
 - [IoK8sApiBatchV1PodFailurePolicyOnExitCodesRequirement](docs/IoK8sApiBatchV1PodFailurePolicyOnExitCodesRequirement.md)
 - [IoK8sApiBatchV1PodFailurePolicyOnPodConditionsPattern](docs/IoK8sApiBatchV1PodFailurePolicyOnPodConditionsPattern.md)
 - [IoK8sApiBatchV1PodFailurePolicyRule](docs/IoK8sApiBatchV1PodFailurePolicyRule.md)
 - [IoK8sApiBatchV1UncountedTerminatedPods](docs/IoK8sApiBatchV1UncountedTerminatedPods.md)
 - [IoK8sApiCertificatesV1CertificateSigningRequest](docs/IoK8sApiCertificatesV1CertificateSigningRequest.md)
 - [IoK8sApiCertificatesV1CertificateSigningRequestCondition](docs/IoK8sApiCertificatesV1CertificateSigningRequestCondition.md)
 - [IoK8sApiCertificatesV1CertificateSigningRequestList](docs/IoK8sApiCertificatesV1CertificateSigningRequestList.md)
 - [IoK8sApiCertificatesV1CertificateSigningRequestSpec](docs/IoK8sApiCertificatesV1CertificateSigningRequestSpec.md)
 - [IoK8sApiCertificatesV1CertificateSigningRequestStatus](docs/IoK8sApiCertificatesV1CertificateSigningRequestStatus.md)
 - [IoK8sApiCoordinationV1Lease](docs/IoK8sApiCoordinationV1Lease.md)
 - [IoK8sApiCoordinationV1LeaseList](docs/IoK8sApiCoordinationV1LeaseList.md)
 - [IoK8sApiCoordinationV1LeaseSpec](docs/IoK8sApiCoordinationV1LeaseSpec.md)
 - [IoK8sApiCoreV1AWSElasticBlockStoreVolumeSource](docs/IoK8sApiCoreV1AWSElasticBlockStoreVolumeSource.md)
 - [IoK8sApiCoreV1Affinity](docs/IoK8sApiCoreV1Affinity.md)
 - [IoK8sApiCoreV1AttachedVolume](docs/IoK8sApiCoreV1AttachedVolume.md)
 - [IoK8sApiCoreV1AzureDiskVolumeSource](docs/IoK8sApiCoreV1AzureDiskVolumeSource.md)
 - [IoK8sApiCoreV1AzureFilePersistentVolumeSource](docs/IoK8sApiCoreV1AzureFilePersistentVolumeSource.md)
 - [IoK8sApiCoreV1AzureFileVolumeSource](docs/IoK8sApiCoreV1AzureFileVolumeSource.md)
 - [IoK8sApiCoreV1Binding](docs/IoK8sApiCoreV1Binding.md)
 - [IoK8sApiCoreV1CSIPersistentVolumeSource](docs/IoK8sApiCoreV1CSIPersistentVolumeSource.md)
 - [IoK8sApiCoreV1CSIVolumeSource](docs/IoK8sApiCoreV1CSIVolumeSource.md)
 - [IoK8sApiCoreV1Capabilities](docs/IoK8sApiCoreV1Capabilities.md)
 - [IoK8sApiCoreV1CephFSPersistentVolumeSource](docs/IoK8sApiCoreV1CephFSPersistentVolumeSource.md)
 - [IoK8sApiCoreV1CephFSVolumeSource](docs/IoK8sApiCoreV1CephFSVolumeSource.md)
 - [IoK8sApiCoreV1CinderPersistentVolumeSource](docs/IoK8sApiCoreV1CinderPersistentVolumeSource.md)
 - [IoK8sApiCoreV1CinderVolumeSource](docs/IoK8sApiCoreV1CinderVolumeSource.md)
 - [IoK8sApiCoreV1ClaimSource](docs/IoK8sApiCoreV1ClaimSource.md)
 - [IoK8sApiCoreV1ClientIPConfig](docs/IoK8sApiCoreV1ClientIPConfig.md)
 - [IoK8sApiCoreV1ComponentCondition](docs/IoK8sApiCoreV1ComponentCondition.md)
 - [IoK8sApiCoreV1ComponentStatus](docs/IoK8sApiCoreV1ComponentStatus.md)
 - [IoK8sApiCoreV1ComponentStatusList](docs/IoK8sApiCoreV1ComponentStatusList.md)
 - [IoK8sApiCoreV1ConfigMap](docs/IoK8sApiCoreV1ConfigMap.md)
 - [IoK8sApiCoreV1ConfigMapEnvSource](docs/IoK8sApiCoreV1ConfigMapEnvSource.md)
 - [IoK8sApiCoreV1ConfigMapKeySelector](docs/IoK8sApiCoreV1ConfigMapKeySelector.md)
 - [IoK8sApiCoreV1ConfigMapList](docs/IoK8sApiCoreV1ConfigMapList.md)
 - [IoK8sApiCoreV1ConfigMapNodeConfigSource](docs/IoK8sApiCoreV1ConfigMapNodeConfigSource.md)
 - [IoK8sApiCoreV1ConfigMapProjection](docs/IoK8sApiCoreV1ConfigMapProjection.md)
 - [IoK8sApiCoreV1ConfigMapVolumeSource](docs/IoK8sApiCoreV1ConfigMapVolumeSource.md)
 - [IoK8sApiCoreV1Container](docs/IoK8sApiCoreV1Container.md)
 - [IoK8sApiCoreV1ContainerImage](docs/IoK8sApiCoreV1ContainerImage.md)
 - [IoK8sApiCoreV1ContainerPort](docs/IoK8sApiCoreV1ContainerPort.md)
 - [IoK8sApiCoreV1ContainerState](docs/IoK8sApiCoreV1ContainerState.md)
 - [IoK8sApiCoreV1ContainerStateRunning](docs/IoK8sApiCoreV1ContainerStateRunning.md)
 - [IoK8sApiCoreV1ContainerStateTerminated](docs/IoK8sApiCoreV1ContainerStateTerminated.md)
 - [IoK8sApiCoreV1ContainerStateWaiting](docs/IoK8sApiCoreV1ContainerStateWaiting.md)
 - [IoK8sApiCoreV1ContainerStatus](docs/IoK8sApiCoreV1ContainerStatus.md)
 - [IoK8sApiCoreV1DaemonEndpoint](docs/IoK8sApiCoreV1DaemonEndpoint.md)
 - [IoK8sApiCoreV1DownwardAPIProjection](docs/IoK8sApiCoreV1DownwardAPIProjection.md)
 - [IoK8sApiCoreV1DownwardAPIVolumeFile](docs/IoK8sApiCoreV1DownwardAPIVolumeFile.md)
 - [IoK8sApiCoreV1DownwardAPIVolumeSource](docs/IoK8sApiCoreV1DownwardAPIVolumeSource.md)
 - [IoK8sApiCoreV1EmptyDirVolumeSource](docs/IoK8sApiCoreV1EmptyDirVolumeSource.md)
 - [IoK8sApiCoreV1EndpointAddress](docs/IoK8sApiCoreV1EndpointAddress.md)
 - [IoK8sApiCoreV1EndpointPort](docs/IoK8sApiCoreV1EndpointPort.md)
 - [IoK8sApiCoreV1EndpointSubset](docs/IoK8sApiCoreV1EndpointSubset.md)
 - [IoK8sApiCoreV1Endpoints](docs/IoK8sApiCoreV1Endpoints.md)
 - [IoK8sApiCoreV1EndpointsList](docs/IoK8sApiCoreV1EndpointsList.md)
 - [IoK8sApiCoreV1EnvFromSource](docs/IoK8sApiCoreV1EnvFromSource.md)
 - [IoK8sApiCoreV1EnvVar](docs/IoK8sApiCoreV1EnvVar.md)
 - [IoK8sApiCoreV1EnvVarSource](docs/IoK8sApiCoreV1EnvVarSource.md)
 - [IoK8sApiCoreV1EphemeralContainer](docs/IoK8sApiCoreV1EphemeralContainer.md)
 - [IoK8sApiCoreV1EphemeralVolumeSource](docs/IoK8sApiCoreV1EphemeralVolumeSource.md)
 - [IoK8sApiCoreV1Event](docs/IoK8sApiCoreV1Event.md)
 - [IoK8sApiCoreV1EventList](docs/IoK8sApiCoreV1EventList.md)
 - [IoK8sApiCoreV1EventSeries](docs/IoK8sApiCoreV1EventSeries.md)
 - [IoK8sApiCoreV1EventSource](docs/IoK8sApiCoreV1EventSource.md)
 - [IoK8sApiCoreV1ExecAction](docs/IoK8sApiCoreV1ExecAction.md)
 - [IoK8sApiCoreV1FCVolumeSource](docs/IoK8sApiCoreV1FCVolumeSource.md)
 - [IoK8sApiCoreV1FlexPersistentVolumeSource](docs/IoK8sApiCoreV1FlexPersistentVolumeSource.md)
 - [IoK8sApiCoreV1FlexVolumeSource](docs/IoK8sApiCoreV1FlexVolumeSource.md)
 - [IoK8sApiCoreV1FlockerVolumeSource](docs/IoK8sApiCoreV1FlockerVolumeSource.md)
 - [IoK8sApiCoreV1GCEPersistentDiskVolumeSource](docs/IoK8sApiCoreV1GCEPersistentDiskVolumeSource.md)
 - [IoK8sApiCoreV1GRPCAction](docs/IoK8sApiCoreV1GRPCAction.md)
 - [IoK8sApiCoreV1GitRepoVolumeSource](docs/IoK8sApiCoreV1GitRepoVolumeSource.md)
 - [IoK8sApiCoreV1GlusterfsPersistentVolumeSource](docs/IoK8sApiCoreV1GlusterfsPersistentVolumeSource.md)
 - [IoK8sApiCoreV1GlusterfsVolumeSource](docs/IoK8sApiCoreV1GlusterfsVolumeSource.md)
 - [IoK8sApiCoreV1HTTPGetAction](docs/IoK8sApiCoreV1HTTPGetAction.md)
 - [IoK8sApiCoreV1HTTPHeader](docs/IoK8sApiCoreV1HTTPHeader.md)
 - [IoK8sApiCoreV1HostAlias](docs/IoK8sApiCoreV1HostAlias.md)
 - [IoK8sApiCoreV1HostPathVolumeSource](docs/IoK8sApiCoreV1HostPathVolumeSource.md)
 - [IoK8sApiCoreV1ISCSIPersistentVolumeSource](docs/IoK8sApiCoreV1ISCSIPersistentVolumeSource.md)
 - [IoK8sApiCoreV1ISCSIVolumeSource](docs/IoK8sApiCoreV1ISCSIVolumeSource.md)
 - [IoK8sApiCoreV1KeyToPath](docs/IoK8sApiCoreV1KeyToPath.md)
 - [IoK8sApiCoreV1Lifecycle](docs/IoK8sApiCoreV1Lifecycle.md)
 - [IoK8sApiCoreV1LifecycleHandler](docs/IoK8sApiCoreV1LifecycleHandler.md)
 - [IoK8sApiCoreV1LimitRange](docs/IoK8sApiCoreV1LimitRange.md)
 - [IoK8sApiCoreV1LimitRangeItem](docs/IoK8sApiCoreV1LimitRangeItem.md)
 - [IoK8sApiCoreV1LimitRangeList](docs/IoK8sApiCoreV1LimitRangeList.md)
 - [IoK8sApiCoreV1LimitRangeSpec](docs/IoK8sApiCoreV1LimitRangeSpec.md)
 - [IoK8sApiCoreV1LoadBalancerIngress](docs/IoK8sApiCoreV1LoadBalancerIngress.md)
 - [IoK8sApiCoreV1LoadBalancerStatus](docs/IoK8sApiCoreV1LoadBalancerStatus.md)
 - [IoK8sApiCoreV1LocalObjectReference](docs/IoK8sApiCoreV1LocalObjectReference.md)
 - [IoK8sApiCoreV1LocalVolumeSource](docs/IoK8sApiCoreV1LocalVolumeSource.md)
 - [IoK8sApiCoreV1NFSVolumeSource](docs/IoK8sApiCoreV1NFSVolumeSource.md)
 - [IoK8sApiCoreV1Namespace](docs/IoK8sApiCoreV1Namespace.md)
 - [IoK8sApiCoreV1NamespaceCondition](docs/IoK8sApiCoreV1NamespaceCondition.md)
 - [IoK8sApiCoreV1NamespaceList](docs/IoK8sApiCoreV1NamespaceList.md)
 - [IoK8sApiCoreV1NamespaceSpec](docs/IoK8sApiCoreV1NamespaceSpec.md)
 - [IoK8sApiCoreV1NamespaceStatus](docs/IoK8sApiCoreV1NamespaceStatus.md)
 - [IoK8sApiCoreV1Node](docs/IoK8sApiCoreV1Node.md)
 - [IoK8sApiCoreV1NodeAddress](docs/IoK8sApiCoreV1NodeAddress.md)
 - [IoK8sApiCoreV1NodeAffinity](docs/IoK8sApiCoreV1NodeAffinity.md)
 - [IoK8sApiCoreV1NodeCondition](docs/IoK8sApiCoreV1NodeCondition.md)
 - [IoK8sApiCoreV1NodeConfigSource](docs/IoK8sApiCoreV1NodeConfigSource.md)
 - [IoK8sApiCoreV1NodeConfigStatus](docs/IoK8sApiCoreV1NodeConfigStatus.md)
 - [IoK8sApiCoreV1NodeDaemonEndpoints](docs/IoK8sApiCoreV1NodeDaemonEndpoints.md)
 - [IoK8sApiCoreV1NodeList](docs/IoK8sApiCoreV1NodeList.md)
 - [IoK8sApiCoreV1NodeSelector](docs/IoK8sApiCoreV1NodeSelector.md)
 - [IoK8sApiCoreV1NodeSelectorRequirement](docs/IoK8sApiCoreV1NodeSelectorRequirement.md)
 - [IoK8sApiCoreV1NodeSelectorTerm](docs/IoK8sApiCoreV1NodeSelectorTerm.md)
 - [IoK8sApiCoreV1NodeSpec](docs/IoK8sApiCoreV1NodeSpec.md)
 - [IoK8sApiCoreV1NodeStatus](docs/IoK8sApiCoreV1NodeStatus.md)
 - [IoK8sApiCoreV1NodeSystemInfo](docs/IoK8sApiCoreV1NodeSystemInfo.md)
 - [IoK8sApiCoreV1ObjectFieldSelector](docs/IoK8sApiCoreV1ObjectFieldSelector.md)
 - [IoK8sApiCoreV1ObjectReference](docs/IoK8sApiCoreV1ObjectReference.md)
 - [IoK8sApiCoreV1PersistentVolume](docs/IoK8sApiCoreV1PersistentVolume.md)
 - [IoK8sApiCoreV1PersistentVolumeClaim](docs/IoK8sApiCoreV1PersistentVolumeClaim.md)
 - [IoK8sApiCoreV1PersistentVolumeClaimCondition](docs/IoK8sApiCoreV1PersistentVolumeClaimCondition.md)
 - [IoK8sApiCoreV1PersistentVolumeClaimList](docs/IoK8sApiCoreV1PersistentVolumeClaimList.md)
 - [IoK8sApiCoreV1PersistentVolumeClaimSpec](docs/IoK8sApiCoreV1PersistentVolumeClaimSpec.md)
 - [IoK8sApiCoreV1PersistentVolumeClaimStatus](docs/IoK8sApiCoreV1PersistentVolumeClaimStatus.md)
 - [IoK8sApiCoreV1PersistentVolumeClaimTemplate](docs/IoK8sApiCoreV1PersistentVolumeClaimTemplate.md)
 - [IoK8sApiCoreV1PersistentVolumeClaimVolumeSource](docs/IoK8sApiCoreV1PersistentVolumeClaimVolumeSource.md)
 - [IoK8sApiCoreV1PersistentVolumeList](docs/IoK8sApiCoreV1PersistentVolumeList.md)
 - [IoK8sApiCoreV1PersistentVolumeSpec](docs/IoK8sApiCoreV1PersistentVolumeSpec.md)
 - [IoK8sApiCoreV1PersistentVolumeStatus](docs/IoK8sApiCoreV1PersistentVolumeStatus.md)
 - [IoK8sApiCoreV1PhotonPersistentDiskVolumeSource](docs/IoK8sApiCoreV1PhotonPersistentDiskVolumeSource.md)
 - [IoK8sApiCoreV1Pod](docs/IoK8sApiCoreV1Pod.md)
 - [IoK8sApiCoreV1PodAffinity](docs/IoK8sApiCoreV1PodAffinity.md)
 - [IoK8sApiCoreV1PodAffinityTerm](docs/IoK8sApiCoreV1PodAffinityTerm.md)
 - [IoK8sApiCoreV1PodAntiAffinity](docs/IoK8sApiCoreV1PodAntiAffinity.md)
 - [IoK8sApiCoreV1PodCondition](docs/IoK8sApiCoreV1PodCondition.md)
 - [IoK8sApiCoreV1PodDNSConfig](docs/IoK8sApiCoreV1PodDNSConfig.md)
 - [IoK8sApiCoreV1PodDNSConfigOption](docs/IoK8sApiCoreV1PodDNSConfigOption.md)
 - [IoK8sApiCoreV1PodIP](docs/IoK8sApiCoreV1PodIP.md)
 - [IoK8sApiCoreV1PodList](docs/IoK8sApiCoreV1PodList.md)
 - [IoK8sApiCoreV1PodOS](docs/IoK8sApiCoreV1PodOS.md)
 - [IoK8sApiCoreV1PodReadinessGate](docs/IoK8sApiCoreV1PodReadinessGate.md)
 - [IoK8sApiCoreV1PodResourceClaim](docs/IoK8sApiCoreV1PodResourceClaim.md)
 - [IoK8sApiCoreV1PodSchedulingGate](docs/IoK8sApiCoreV1PodSchedulingGate.md)
 - [IoK8sApiCoreV1PodSecurityContext](docs/IoK8sApiCoreV1PodSecurityContext.md)
 - [IoK8sApiCoreV1PodSpec](docs/IoK8sApiCoreV1PodSpec.md)
 - [IoK8sApiCoreV1PodStatus](docs/IoK8sApiCoreV1PodStatus.md)
 - [IoK8sApiCoreV1PodTemplate](docs/IoK8sApiCoreV1PodTemplate.md)
 - [IoK8sApiCoreV1PodTemplateList](docs/IoK8sApiCoreV1PodTemplateList.md)
 - [IoK8sApiCoreV1PodTemplateSpec](docs/IoK8sApiCoreV1PodTemplateSpec.md)
 - [IoK8sApiCoreV1PortStatus](docs/IoK8sApiCoreV1PortStatus.md)
 - [IoK8sApiCoreV1PortworxVolumeSource](docs/IoK8sApiCoreV1PortworxVolumeSource.md)
 - [IoK8sApiCoreV1PreferredSchedulingTerm](docs/IoK8sApiCoreV1PreferredSchedulingTerm.md)
 - [IoK8sApiCoreV1Probe](docs/IoK8sApiCoreV1Probe.md)
 - [IoK8sApiCoreV1ProjectedVolumeSource](docs/IoK8sApiCoreV1ProjectedVolumeSource.md)
 - [IoK8sApiCoreV1QuobyteVolumeSource](docs/IoK8sApiCoreV1QuobyteVolumeSource.md)
 - [IoK8sApiCoreV1RBDPersistentVolumeSource](docs/IoK8sApiCoreV1RBDPersistentVolumeSource.md)
 - [IoK8sApiCoreV1RBDVolumeSource](docs/IoK8sApiCoreV1RBDVolumeSource.md)
 - [IoK8sApiCoreV1ReplicationController](docs/IoK8sApiCoreV1ReplicationController.md)
 - [IoK8sApiCoreV1ReplicationControllerCondition](docs/IoK8sApiCoreV1ReplicationControllerCondition.md)
 - [IoK8sApiCoreV1ReplicationControllerList](docs/IoK8sApiCoreV1ReplicationControllerList.md)
 - [IoK8sApiCoreV1ReplicationControllerSpec](docs/IoK8sApiCoreV1ReplicationControllerSpec.md)
 - [IoK8sApiCoreV1ReplicationControllerStatus](docs/IoK8sApiCoreV1ReplicationControllerStatus.md)
 - [IoK8sApiCoreV1ResourceClaim](docs/IoK8sApiCoreV1ResourceClaim.md)
 - [IoK8sApiCoreV1ResourceFieldSelector](docs/IoK8sApiCoreV1ResourceFieldSelector.md)
 - [IoK8sApiCoreV1ResourceQuota](docs/IoK8sApiCoreV1ResourceQuota.md)
 - [IoK8sApiCoreV1ResourceQuotaList](docs/IoK8sApiCoreV1ResourceQuotaList.md)
 - [IoK8sApiCoreV1ResourceQuotaSpec](docs/IoK8sApiCoreV1ResourceQuotaSpec.md)
 - [IoK8sApiCoreV1ResourceQuotaStatus](docs/IoK8sApiCoreV1ResourceQuotaStatus.md)
 - [IoK8sApiCoreV1ResourceRequirements](docs/IoK8sApiCoreV1ResourceRequirements.md)
 - [IoK8sApiCoreV1SELinuxOptions](docs/IoK8sApiCoreV1SELinuxOptions.md)
 - [IoK8sApiCoreV1ScaleIOPersistentVolumeSource](docs/IoK8sApiCoreV1ScaleIOPersistentVolumeSource.md)
 - [IoK8sApiCoreV1ScaleIOVolumeSource](docs/IoK8sApiCoreV1ScaleIOVolumeSource.md)
 - [IoK8sApiCoreV1ScopeSelector](docs/IoK8sApiCoreV1ScopeSelector.md)
 - [IoK8sApiCoreV1ScopedResourceSelectorRequirement](docs/IoK8sApiCoreV1ScopedResourceSelectorRequirement.md)
 - [IoK8sApiCoreV1SeccompProfile](docs/IoK8sApiCoreV1SeccompProfile.md)
 - [IoK8sApiCoreV1Secret](docs/IoK8sApiCoreV1Secret.md)
 - [IoK8sApiCoreV1SecretEnvSource](docs/IoK8sApiCoreV1SecretEnvSource.md)
 - [IoK8sApiCoreV1SecretKeySelector](docs/IoK8sApiCoreV1SecretKeySelector.md)
 - [IoK8sApiCoreV1SecretList](docs/IoK8sApiCoreV1SecretList.md)
 - [IoK8sApiCoreV1SecretProjection](docs/IoK8sApiCoreV1SecretProjection.md)
 - [IoK8sApiCoreV1SecretReference](docs/IoK8sApiCoreV1SecretReference.md)
 - [IoK8sApiCoreV1SecretVolumeSource](docs/IoK8sApiCoreV1SecretVolumeSource.md)
 - [IoK8sApiCoreV1SecurityContext](docs/IoK8sApiCoreV1SecurityContext.md)
 - [IoK8sApiCoreV1Service](docs/IoK8sApiCoreV1Service.md)
 - [IoK8sApiCoreV1ServiceAccount](docs/IoK8sApiCoreV1ServiceAccount.md)
 - [IoK8sApiCoreV1ServiceAccountList](docs/IoK8sApiCoreV1ServiceAccountList.md)
 - [IoK8sApiCoreV1ServiceAccountTokenProjection](docs/IoK8sApiCoreV1ServiceAccountTokenProjection.md)
 - [IoK8sApiCoreV1ServiceList](docs/IoK8sApiCoreV1ServiceList.md)
 - [IoK8sApiCoreV1ServicePort](docs/IoK8sApiCoreV1ServicePort.md)
 - [IoK8sApiCoreV1ServiceSpec](docs/IoK8sApiCoreV1ServiceSpec.md)
 - [IoK8sApiCoreV1ServiceStatus](docs/IoK8sApiCoreV1ServiceStatus.md)
 - [IoK8sApiCoreV1SessionAffinityConfig](docs/IoK8sApiCoreV1SessionAffinityConfig.md)
 - [IoK8sApiCoreV1StorageOSPersistentVolumeSource](docs/IoK8sApiCoreV1StorageOSPersistentVolumeSource.md)
 - [IoK8sApiCoreV1StorageOSVolumeSource](docs/IoK8sApiCoreV1StorageOSVolumeSource.md)
 - [IoK8sApiCoreV1Sysctl](docs/IoK8sApiCoreV1Sysctl.md)
 - [IoK8sApiCoreV1TCPSocketAction](docs/IoK8sApiCoreV1TCPSocketAction.md)
 - [IoK8sApiCoreV1Taint](docs/IoK8sApiCoreV1Taint.md)
 - [IoK8sApiCoreV1Toleration](docs/IoK8sApiCoreV1Toleration.md)
 - [IoK8sApiCoreV1TopologySelectorLabelRequirement](docs/IoK8sApiCoreV1TopologySelectorLabelRequirement.md)
 - [IoK8sApiCoreV1TopologySelectorTerm](docs/IoK8sApiCoreV1TopologySelectorTerm.md)
 - [IoK8sApiCoreV1TopologySpreadConstraint](docs/IoK8sApiCoreV1TopologySpreadConstraint.md)
 - [IoK8sApiCoreV1TypedLocalObjectReference](docs/IoK8sApiCoreV1TypedLocalObjectReference.md)
 - [IoK8sApiCoreV1TypedObjectReference](docs/IoK8sApiCoreV1TypedObjectReference.md)
 - [IoK8sApiCoreV1Volume](docs/IoK8sApiCoreV1Volume.md)
 - [IoK8sApiCoreV1VolumeDevice](docs/IoK8sApiCoreV1VolumeDevice.md)
 - [IoK8sApiCoreV1VolumeMount](docs/IoK8sApiCoreV1VolumeMount.md)
 - [IoK8sApiCoreV1VolumeNodeAffinity](docs/IoK8sApiCoreV1VolumeNodeAffinity.md)
 - [IoK8sApiCoreV1VolumeProjection](docs/IoK8sApiCoreV1VolumeProjection.md)
 - [IoK8sApiCoreV1VsphereVirtualDiskVolumeSource](docs/IoK8sApiCoreV1VsphereVirtualDiskVolumeSource.md)
 - [IoK8sApiCoreV1WeightedPodAffinityTerm](docs/IoK8sApiCoreV1WeightedPodAffinityTerm.md)
 - [IoK8sApiCoreV1WindowsSecurityContextOptions](docs/IoK8sApiCoreV1WindowsSecurityContextOptions.md)
 - [IoK8sApiDiscoveryV1Endpoint](docs/IoK8sApiDiscoveryV1Endpoint.md)
 - [IoK8sApiDiscoveryV1EndpointConditions](docs/IoK8sApiDiscoveryV1EndpointConditions.md)
 - [IoK8sApiDiscoveryV1EndpointHints](docs/IoK8sApiDiscoveryV1EndpointHints.md)
 - [IoK8sApiDiscoveryV1EndpointPort](docs/IoK8sApiDiscoveryV1EndpointPort.md)
 - [IoK8sApiDiscoveryV1EndpointSlice](docs/IoK8sApiDiscoveryV1EndpointSlice.md)
 - [IoK8sApiDiscoveryV1EndpointSliceList](docs/IoK8sApiDiscoveryV1EndpointSliceList.md)
 - [IoK8sApiDiscoveryV1ForZone](docs/IoK8sApiDiscoveryV1ForZone.md)
 - [IoK8sApiEventsV1Event](docs/IoK8sApiEventsV1Event.md)
 - [IoK8sApiEventsV1EventList](docs/IoK8sApiEventsV1EventList.md)
 - [IoK8sApiEventsV1EventSeries](docs/IoK8sApiEventsV1EventSeries.md)
 - [IoK8sApiFlowcontrolV1beta2FlowDistinguisherMethod](docs/IoK8sApiFlowcontrolV1beta2FlowDistinguisherMethod.md)
 - [IoK8sApiFlowcontrolV1beta2FlowSchema](docs/IoK8sApiFlowcontrolV1beta2FlowSchema.md)
 - [IoK8sApiFlowcontrolV1beta2FlowSchemaCondition](docs/IoK8sApiFlowcontrolV1beta2FlowSchemaCondition.md)
 - [IoK8sApiFlowcontrolV1beta2FlowSchemaList](docs/IoK8sApiFlowcontrolV1beta2FlowSchemaList.md)
 - [IoK8sApiFlowcontrolV1beta2FlowSchemaSpec](docs/IoK8sApiFlowcontrolV1beta2FlowSchemaSpec.md)
 - [IoK8sApiFlowcontrolV1beta2FlowSchemaStatus](docs/IoK8sApiFlowcontrolV1beta2FlowSchemaStatus.md)
 - [IoK8sApiFlowcontrolV1beta2GroupSubject](docs/IoK8sApiFlowcontrolV1beta2GroupSubject.md)
 - [IoK8sApiFlowcontrolV1beta2LimitResponse](docs/IoK8sApiFlowcontrolV1beta2LimitResponse.md)
 - [IoK8sApiFlowcontrolV1beta2LimitedPriorityLevelConfiguration](docs/IoK8sApiFlowcontrolV1beta2LimitedPriorityLevelConfiguration.md)
 - [IoK8sApiFlowcontrolV1beta2NonResourcePolicyRule](docs/IoK8sApiFlowcontrolV1beta2NonResourcePolicyRule.md)
 - [IoK8sApiFlowcontrolV1beta2PolicyRulesWithSubjects](docs/IoK8sApiFlowcontrolV1beta2PolicyRulesWithSubjects.md)
 - [IoK8sApiFlowcontrolV1beta2PriorityLevelConfiguration](docs/IoK8sApiFlowcontrolV1beta2PriorityLevelConfiguration.md)
 - [IoK8sApiFlowcontrolV1beta2PriorityLevelConfigurationCondition](docs/IoK8sApiFlowcontrolV1beta2PriorityLevelConfigurationCondition.md)
 - [IoK8sApiFlowcontrolV1beta2PriorityLevelConfigurationList](docs/IoK8sApiFlowcontrolV1beta2PriorityLevelConfigurationList.md)
 - [IoK8sApiFlowcontrolV1beta2PriorityLevelConfigurationReference](docs/IoK8sApiFlowcontrolV1beta2PriorityLevelConfigurationReference.md)
 - [IoK8sApiFlowcontrolV1beta2PriorityLevelConfigurationSpec](docs/IoK8sApiFlowcontrolV1beta2PriorityLevelConfigurationSpec.md)
 - [IoK8sApiFlowcontrolV1beta2PriorityLevelConfigurationStatus](docs/IoK8sApiFlowcontrolV1beta2PriorityLevelConfigurationStatus.md)
 - [IoK8sApiFlowcontrolV1beta2QueuingConfiguration](docs/IoK8sApiFlowcontrolV1beta2QueuingConfiguration.md)
 - [IoK8sApiFlowcontrolV1beta2ResourcePolicyRule](docs/IoK8sApiFlowcontrolV1beta2ResourcePolicyRule.md)
 - [IoK8sApiFlowcontrolV1beta2ServiceAccountSubject](docs/IoK8sApiFlowcontrolV1beta2ServiceAccountSubject.md)
 - [IoK8sApiFlowcontrolV1beta2Subject](docs/IoK8sApiFlowcontrolV1beta2Subject.md)
 - [IoK8sApiFlowcontrolV1beta2UserSubject](docs/IoK8sApiFlowcontrolV1beta2UserSubject.md)
 - [IoK8sApiFlowcontrolV1beta3FlowDistinguisherMethod](docs/IoK8sApiFlowcontrolV1beta3FlowDistinguisherMethod.md)
 - [IoK8sApiFlowcontrolV1beta3FlowSchema](docs/IoK8sApiFlowcontrolV1beta3FlowSchema.md)
 - [IoK8sApiFlowcontrolV1beta3FlowSchemaCondition](docs/IoK8sApiFlowcontrolV1beta3FlowSchemaCondition.md)
 - [IoK8sApiFlowcontrolV1beta3FlowSchemaList](docs/IoK8sApiFlowcontrolV1beta3FlowSchemaList.md)
 - [IoK8sApiFlowcontrolV1beta3FlowSchemaSpec](docs/IoK8sApiFlowcontrolV1beta3FlowSchemaSpec.md)
 - [IoK8sApiFlowcontrolV1beta3FlowSchemaStatus](docs/IoK8sApiFlowcontrolV1beta3FlowSchemaStatus.md)
 - [IoK8sApiFlowcontrolV1beta3GroupSubject](docs/IoK8sApiFlowcontrolV1beta3GroupSubject.md)
 - [IoK8sApiFlowcontrolV1beta3LimitResponse](docs/IoK8sApiFlowcontrolV1beta3LimitResponse.md)
 - [IoK8sApiFlowcontrolV1beta3LimitedPriorityLevelConfiguration](docs/IoK8sApiFlowcontrolV1beta3LimitedPriorityLevelConfiguration.md)
 - [IoK8sApiFlowcontrolV1beta3NonResourcePolicyRule](docs/IoK8sApiFlowcontrolV1beta3NonResourcePolicyRule.md)
 - [IoK8sApiFlowcontrolV1beta3PolicyRulesWithSubjects](docs/IoK8sApiFlowcontrolV1beta3PolicyRulesWithSubjects.md)
 - [IoK8sApiFlowcontrolV1beta3PriorityLevelConfiguration](docs/IoK8sApiFlowcontrolV1beta3PriorityLevelConfiguration.md)
 - [IoK8sApiFlowcontrolV1beta3PriorityLevelConfigurationCondition](docs/IoK8sApiFlowcontrolV1beta3PriorityLevelConfigurationCondition.md)
 - [IoK8sApiFlowcontrolV1beta3PriorityLevelConfigurationList](docs/IoK8sApiFlowcontrolV1beta3PriorityLevelConfigurationList.md)
 - [IoK8sApiFlowcontrolV1beta3PriorityLevelConfigurationReference](docs/IoK8sApiFlowcontrolV1beta3PriorityLevelConfigurationReference.md)
 - [IoK8sApiFlowcontrolV1beta3PriorityLevelConfigurationSpec](docs/IoK8sApiFlowcontrolV1beta3PriorityLevelConfigurationSpec.md)
 - [IoK8sApiFlowcontrolV1beta3PriorityLevelConfigurationStatus](docs/IoK8sApiFlowcontrolV1beta3PriorityLevelConfigurationStatus.md)
 - [IoK8sApiFlowcontrolV1beta3QueuingConfiguration](docs/IoK8sApiFlowcontrolV1beta3QueuingConfiguration.md)
 - [IoK8sApiFlowcontrolV1beta3ResourcePolicyRule](docs/IoK8sApiFlowcontrolV1beta3ResourcePolicyRule.md)
 - [IoK8sApiFlowcontrolV1beta3ServiceAccountSubject](docs/IoK8sApiFlowcontrolV1beta3ServiceAccountSubject.md)
 - [IoK8sApiFlowcontrolV1beta3Subject](docs/IoK8sApiFlowcontrolV1beta3Subject.md)
 - [IoK8sApiFlowcontrolV1beta3UserSubject](docs/IoK8sApiFlowcontrolV1beta3UserSubject.md)
 - [IoK8sApiNetworkingV1HTTPIngressPath](docs/IoK8sApiNetworkingV1HTTPIngressPath.md)
 - [IoK8sApiNetworkingV1HTTPIngressRuleValue](docs/IoK8sApiNetworkingV1HTTPIngressRuleValue.md)
 - [IoK8sApiNetworkingV1IPBlock](docs/IoK8sApiNetworkingV1IPBlock.md)
 - [IoK8sApiNetworkingV1Ingress](docs/IoK8sApiNetworkingV1Ingress.md)
 - [IoK8sApiNetworkingV1IngressBackend](docs/IoK8sApiNetworkingV1IngressBackend.md)
 - [IoK8sApiNetworkingV1IngressClass](docs/IoK8sApiNetworkingV1IngressClass.md)
 - [IoK8sApiNetworkingV1IngressClassList](docs/IoK8sApiNetworkingV1IngressClassList.md)
 - [IoK8sApiNetworkingV1IngressClassParametersReference](docs/IoK8sApiNetworkingV1IngressClassParametersReference.md)
 - [IoK8sApiNetworkingV1IngressClassSpec](docs/IoK8sApiNetworkingV1IngressClassSpec.md)
 - [IoK8sApiNetworkingV1IngressList](docs/IoK8sApiNetworkingV1IngressList.md)
 - [IoK8sApiNetworkingV1IngressLoadBalancerIngress](docs/IoK8sApiNetworkingV1IngressLoadBalancerIngress.md)
 - [IoK8sApiNetworkingV1IngressLoadBalancerStatus](docs/IoK8sApiNetworkingV1IngressLoadBalancerStatus.md)
 - [IoK8sApiNetworkingV1IngressPortStatus](docs/IoK8sApiNetworkingV1IngressPortStatus.md)
 - [IoK8sApiNetworkingV1IngressRule](docs/IoK8sApiNetworkingV1IngressRule.md)
 - [IoK8sApiNetworkingV1IngressServiceBackend](docs/IoK8sApiNetworkingV1IngressServiceBackend.md)
 - [IoK8sApiNetworkingV1IngressSpec](docs/IoK8sApiNetworkingV1IngressSpec.md)
 - [IoK8sApiNetworkingV1IngressStatus](docs/IoK8sApiNetworkingV1IngressStatus.md)
 - [IoK8sApiNetworkingV1IngressTLS](docs/IoK8sApiNetworkingV1IngressTLS.md)
 - [IoK8sApiNetworkingV1NetworkPolicy](docs/IoK8sApiNetworkingV1NetworkPolicy.md)
 - [IoK8sApiNetworkingV1NetworkPolicyEgressRule](docs/IoK8sApiNetworkingV1NetworkPolicyEgressRule.md)
 - [IoK8sApiNetworkingV1NetworkPolicyIngressRule](docs/IoK8sApiNetworkingV1NetworkPolicyIngressRule.md)
 - [IoK8sApiNetworkingV1NetworkPolicyList](docs/IoK8sApiNetworkingV1NetworkPolicyList.md)
 - [IoK8sApiNetworkingV1NetworkPolicyPeer](docs/IoK8sApiNetworkingV1NetworkPolicyPeer.md)
 - [IoK8sApiNetworkingV1NetworkPolicyPort](docs/IoK8sApiNetworkingV1NetworkPolicyPort.md)
 - [IoK8sApiNetworkingV1NetworkPolicySpec](docs/IoK8sApiNetworkingV1NetworkPolicySpec.md)
 - [IoK8sApiNetworkingV1NetworkPolicyStatus](docs/IoK8sApiNetworkingV1NetworkPolicyStatus.md)
 - [IoK8sApiNetworkingV1ServiceBackendPort](docs/IoK8sApiNetworkingV1ServiceBackendPort.md)
 - [IoK8sApiNetworkingV1alpha1ClusterCIDR](docs/IoK8sApiNetworkingV1alpha1ClusterCIDR.md)
 - [IoK8sApiNetworkingV1alpha1ClusterCIDRList](docs/IoK8sApiNetworkingV1alpha1ClusterCIDRList.md)
 - [IoK8sApiNetworkingV1alpha1ClusterCIDRSpec](docs/IoK8sApiNetworkingV1alpha1ClusterCIDRSpec.md)
 - [IoK8sApiNodeV1Overhead](docs/IoK8sApiNodeV1Overhead.md)
 - [IoK8sApiNodeV1RuntimeClass](docs/IoK8sApiNodeV1RuntimeClass.md)
 - [IoK8sApiNodeV1RuntimeClassList](docs/IoK8sApiNodeV1RuntimeClassList.md)
 - [IoK8sApiNodeV1Scheduling](docs/IoK8sApiNodeV1Scheduling.md)
 - [IoK8sApiPolicyV1Eviction](docs/IoK8sApiPolicyV1Eviction.md)
 - [IoK8sApiPolicyV1PodDisruptionBudget](docs/IoK8sApiPolicyV1PodDisruptionBudget.md)
 - [IoK8sApiPolicyV1PodDisruptionBudgetList](docs/IoK8sApiPolicyV1PodDisruptionBudgetList.md)
 - [IoK8sApiPolicyV1PodDisruptionBudgetSpec](docs/IoK8sApiPolicyV1PodDisruptionBudgetSpec.md)
 - [IoK8sApiPolicyV1PodDisruptionBudgetStatus](docs/IoK8sApiPolicyV1PodDisruptionBudgetStatus.md)
 - [IoK8sApiRbacV1AggregationRule](docs/IoK8sApiRbacV1AggregationRule.md)
 - [IoK8sApiRbacV1ClusterRole](docs/IoK8sApiRbacV1ClusterRole.md)
 - [IoK8sApiRbacV1ClusterRoleBinding](docs/IoK8sApiRbacV1ClusterRoleBinding.md)
 - [IoK8sApiRbacV1ClusterRoleBindingList](docs/IoK8sApiRbacV1ClusterRoleBindingList.md)
 - [IoK8sApiRbacV1ClusterRoleList](docs/IoK8sApiRbacV1ClusterRoleList.md)
 - [IoK8sApiRbacV1PolicyRule](docs/IoK8sApiRbacV1PolicyRule.md)
 - [IoK8sApiRbacV1Role](docs/IoK8sApiRbacV1Role.md)
 - [IoK8sApiRbacV1RoleBinding](docs/IoK8sApiRbacV1RoleBinding.md)
 - [IoK8sApiRbacV1RoleBindingList](docs/IoK8sApiRbacV1RoleBindingList.md)
 - [IoK8sApiRbacV1RoleList](docs/IoK8sApiRbacV1RoleList.md)
 - [IoK8sApiRbacV1RoleRef](docs/IoK8sApiRbacV1RoleRef.md)
 - [IoK8sApiRbacV1Subject](docs/IoK8sApiRbacV1Subject.md)
 - [IoK8sApiResourceV1alpha1AllocationResult](docs/IoK8sApiResourceV1alpha1AllocationResult.md)
 - [IoK8sApiResourceV1alpha1PodScheduling](docs/IoK8sApiResourceV1alpha1PodScheduling.md)
 - [IoK8sApiResourceV1alpha1PodSchedulingList](docs/IoK8sApiResourceV1alpha1PodSchedulingList.md)
 - [IoK8sApiResourceV1alpha1PodSchedulingSpec](docs/IoK8sApiResourceV1alpha1PodSchedulingSpec.md)
 - [IoK8sApiResourceV1alpha1PodSchedulingStatus](docs/IoK8sApiResourceV1alpha1PodSchedulingStatus.md)
 - [IoK8sApiResourceV1alpha1ResourceClaim](docs/IoK8sApiResourceV1alpha1ResourceClaim.md)
 - [IoK8sApiResourceV1alpha1ResourceClaimConsumerReference](docs/IoK8sApiResourceV1alpha1ResourceClaimConsumerReference.md)
 - [IoK8sApiResourceV1alpha1ResourceClaimList](docs/IoK8sApiResourceV1alpha1ResourceClaimList.md)
 - [IoK8sApiResourceV1alpha1ResourceClaimParametersReference](docs/IoK8sApiResourceV1alpha1ResourceClaimParametersReference.md)
 - [IoK8sApiResourceV1alpha1ResourceClaimSchedulingStatus](docs/IoK8sApiResourceV1alpha1ResourceClaimSchedulingStatus.md)
 - [IoK8sApiResourceV1alpha1ResourceClaimSpec](docs/IoK8sApiResourceV1alpha1ResourceClaimSpec.md)
 - [IoK8sApiResourceV1alpha1ResourceClaimStatus](docs/IoK8sApiResourceV1alpha1ResourceClaimStatus.md)
 - [IoK8sApiResourceV1alpha1ResourceClaimTemplate](docs/IoK8sApiResourceV1alpha1ResourceClaimTemplate.md)
 - [IoK8sApiResourceV1alpha1ResourceClaimTemplateList](docs/IoK8sApiResourceV1alpha1ResourceClaimTemplateList.md)
 - [IoK8sApiResourceV1alpha1ResourceClaimTemplateSpec](docs/IoK8sApiResourceV1alpha1ResourceClaimTemplateSpec.md)
 - [IoK8sApiResourceV1alpha1ResourceClass](docs/IoK8sApiResourceV1alpha1ResourceClass.md)
 - [IoK8sApiResourceV1alpha1ResourceClassList](docs/IoK8sApiResourceV1alpha1ResourceClassList.md)
 - [IoK8sApiResourceV1alpha1ResourceClassParametersReference](docs/IoK8sApiResourceV1alpha1ResourceClassParametersReference.md)
 - [IoK8sApiSchedulingV1PriorityClass](docs/IoK8sApiSchedulingV1PriorityClass.md)
 - [IoK8sApiSchedulingV1PriorityClassList](docs/IoK8sApiSchedulingV1PriorityClassList.md)
 - [IoK8sApiStorageV1CSIDriver](docs/IoK8sApiStorageV1CSIDriver.md)
 - [IoK8sApiStorageV1CSIDriverList](docs/IoK8sApiStorageV1CSIDriverList.md)
 - [IoK8sApiStorageV1CSIDriverSpec](docs/IoK8sApiStorageV1CSIDriverSpec.md)
 - [IoK8sApiStorageV1CSINode](docs/IoK8sApiStorageV1CSINode.md)
 - [IoK8sApiStorageV1CSINodeDriver](docs/IoK8sApiStorageV1CSINodeDriver.md)
 - [IoK8sApiStorageV1CSINodeList](docs/IoK8sApiStorageV1CSINodeList.md)
 - [IoK8sApiStorageV1CSINodeSpec](docs/IoK8sApiStorageV1CSINodeSpec.md)
 - [IoK8sApiStorageV1CSIStorageCapacity](docs/IoK8sApiStorageV1CSIStorageCapacity.md)
 - [IoK8sApiStorageV1CSIStorageCapacityList](docs/IoK8sApiStorageV1CSIStorageCapacityList.md)
 - [IoK8sApiStorageV1StorageClass](docs/IoK8sApiStorageV1StorageClass.md)
 - [IoK8sApiStorageV1StorageClassList](docs/IoK8sApiStorageV1StorageClassList.md)
 - [IoK8sApiStorageV1TokenRequest](docs/IoK8sApiStorageV1TokenRequest.md)
 - [IoK8sApiStorageV1VolumeAttachment](docs/IoK8sApiStorageV1VolumeAttachment.md)
 - [IoK8sApiStorageV1VolumeAttachmentList](docs/IoK8sApiStorageV1VolumeAttachmentList.md)
 - [IoK8sApiStorageV1VolumeAttachmentSource](docs/IoK8sApiStorageV1VolumeAttachmentSource.md)
 - [IoK8sApiStorageV1VolumeAttachmentSpec](docs/IoK8sApiStorageV1VolumeAttachmentSpec.md)
 - [IoK8sApiStorageV1VolumeAttachmentStatus](docs/IoK8sApiStorageV1VolumeAttachmentStatus.md)
 - [IoK8sApiStorageV1VolumeError](docs/IoK8sApiStorageV1VolumeError.md)
 - [IoK8sApiStorageV1VolumeNodeResources](docs/IoK8sApiStorageV1VolumeNodeResources.md)
 - [IoK8sApiStorageV1beta1CSIStorageCapacity](docs/IoK8sApiStorageV1beta1CSIStorageCapacity.md)
 - [IoK8sApiStorageV1beta1CSIStorageCapacityList](docs/IoK8sApiStorageV1beta1CSIStorageCapacityList.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceColumnDefinition](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceColumnDefinition.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceConversion](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceConversion.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceDefinition](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceDefinition.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceDefinitionCondition](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceDefinitionCondition.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceDefinitionList](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceDefinitionList.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceDefinitionNames](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceDefinitionNames.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceDefinitionSpec](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceDefinitionSpec.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceDefinitionStatus](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceDefinitionStatus.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceDefinitionVersion](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceDefinitionVersion.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceSubresourceScale](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceSubresourceScale.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceSubresourceStatus](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceSubresourceStatus.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceSubresources](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceSubresources.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceValidation](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1CustomResourceValidation.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1ExternalDocumentation](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1ExternalDocumentation.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1JSONSchemaProps](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1JSONSchemaProps.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1ServiceReference](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1ServiceReference.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1ValidationRule](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1ValidationRule.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1WebhookClientConfig](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1WebhookClientConfig.md)
 - [IoK8sApiextensionsApiserverPkgApisApiextensionsV1WebhookConversion](docs/IoK8sApiextensionsApiserverPkgApisApiextensionsV1WebhookConversion.md)
 - [IoK8sApimachineryPkgApiResourceQuantity](docs/IoK8sApimachineryPkgApiResourceQuantity.md)
 - [IoK8sApimachineryPkgApisMetaV1APIGroup](docs/IoK8sApimachineryPkgApisMetaV1APIGroup.md)
 - [IoK8sApimachineryPkgApisMetaV1APIGroupList](docs/IoK8sApimachineryPkgApisMetaV1APIGroupList.md)
 - [IoK8sApimachineryPkgApisMetaV1APIResource](docs/IoK8sApimachineryPkgApisMetaV1APIResource.md)
 - [IoK8sApimachineryPkgApisMetaV1APIResourceList](docs/IoK8sApimachineryPkgApisMetaV1APIResourceList.md)
 - [IoK8sApimachineryPkgApisMetaV1APIVersions](docs/IoK8sApimachineryPkgApisMetaV1APIVersions.md)
 - [IoK8sApimachineryPkgApisMetaV1Condition](docs/IoK8sApimachineryPkgApisMetaV1Condition.md)
 - [IoK8sApimachineryPkgApisMetaV1DeleteOptions](docs/IoK8sApimachineryPkgApisMetaV1DeleteOptions.md)
 - [IoK8sApimachineryPkgApisMetaV1FieldsV1](docs/IoK8sApimachineryPkgApisMetaV1FieldsV1.md)
 - [IoK8sApimachineryPkgApisMetaV1GroupVersionForDiscovery](docs/IoK8sApimachineryPkgApisMetaV1GroupVersionForDiscovery.md)
 - [IoK8sApimachineryPkgApisMetaV1LabelSelector](docs/IoK8sApimachineryPkgApisMetaV1LabelSelector.md)
 - [IoK8sApimachineryPkgApisMetaV1LabelSelectorRequirement](docs/IoK8sApimachineryPkgApisMetaV1LabelSelectorRequirement.md)
 - [IoK8sApimachineryPkgApisMetaV1ListMeta](docs/IoK8sApimachineryPkgApisMetaV1ListMeta.md)
 - [IoK8sApimachineryPkgApisMetaV1ManagedFieldsEntry](docs/IoK8sApimachineryPkgApisMetaV1ManagedFieldsEntry.md)
 - [IoK8sApimachineryPkgApisMetaV1MicroTime](docs/IoK8sApimachineryPkgApisMetaV1MicroTime.md)
 - [IoK8sApimachineryPkgApisMetaV1ObjectMeta](docs/IoK8sApimachineryPkgApisMetaV1ObjectMeta.md)
 - [IoK8sApimachineryPkgApisMetaV1OwnerReference](docs/IoK8sApimachineryPkgApisMetaV1OwnerReference.md)
 - [IoK8sApimachineryPkgApisMetaV1Patch](docs/IoK8sApimachineryPkgApisMetaV1Patch.md)
 - [IoK8sApimachineryPkgApisMetaV1Preconditions](docs/IoK8sApimachineryPkgApisMetaV1Preconditions.md)
 - [IoK8sApimachineryPkgApisMetaV1ServerAddressByClientCIDR](docs/IoK8sApimachineryPkgApisMetaV1ServerAddressByClientCIDR.md)
 - [IoK8sApimachineryPkgApisMetaV1Status](docs/IoK8sApimachineryPkgApisMetaV1Status.md)
 - [IoK8sApimachineryPkgApisMetaV1StatusCause](docs/IoK8sApimachineryPkgApisMetaV1StatusCause.md)
 - [IoK8sApimachineryPkgApisMetaV1StatusDetails](docs/IoK8sApimachineryPkgApisMetaV1StatusDetails.md)
 - [IoK8sApimachineryPkgApisMetaV1Time](docs/IoK8sApimachineryPkgApisMetaV1Time.md)
 - [IoK8sApimachineryPkgApisMetaV1WatchEvent](docs/IoK8sApimachineryPkgApisMetaV1WatchEvent.md)
 - [IoK8sApimachineryPkgRuntimeRawExtension](docs/IoK8sApimachineryPkgRuntimeRawExtension.md)
 - [IoK8sApimachineryPkgUtilIntstrIntOrString](docs/IoK8sApimachineryPkgUtilIntstrIntOrString.md)
 - [IoK8sApimachineryPkgVersionInfo](docs/IoK8sApimachineryPkgVersionInfo.md)
 - [IoK8sKubeAggregatorPkgApisApiregistrationV1APIService](docs/IoK8sKubeAggregatorPkgApisApiregistrationV1APIService.md)
 - [IoK8sKubeAggregatorPkgApisApiregistrationV1APIServiceCondition](docs/IoK8sKubeAggregatorPkgApisApiregistrationV1APIServiceCondition.md)
 - [IoK8sKubeAggregatorPkgApisApiregistrationV1APIServiceList](docs/IoK8sKubeAggregatorPkgApisApiregistrationV1APIServiceList.md)
 - [IoK8sKubeAggregatorPkgApisApiregistrationV1APIServiceSpec](docs/IoK8sKubeAggregatorPkgApisApiregistrationV1APIServiceSpec.md)
 - [IoK8sKubeAggregatorPkgApisApiregistrationV1APIServiceStatus](docs/IoK8sKubeAggregatorPkgApisApiregistrationV1APIServiceStatus.md)
 - [IoK8sKubeAggregatorPkgApisApiregistrationV1ServiceReference](docs/IoK8sKubeAggregatorPkgApisApiregistrationV1ServiceReference.md)


## Documentation For Authorization


## BearerToken

- **Type**: API key
- **API key parameter name**: authorization
- **Location**: HTTP header
