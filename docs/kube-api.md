## Resource categories

**Workloads** are objects used to manage and run containers in the cluster.  
**Discovery and LB** resources are objects that bind worloads into an externally accessible, load-balanced service.  
**Config and Storage** resources inject initialization data into applications, and persist data external to containers.  
**Cluster** resources define fundamental configuration.  
**Metadata** objects configure other resources within the cluster.  

## Resource objects

**Resource ObjectMeta**  
Metadata about the resource (name, type, api version, annotations and labels).  

**ResourceSpec**  
It is defined by the user when creating or updating an object, and describes the desired state of system.  

**ResourceStatus**  
It reports the current state of the system.

## Resource operations

### Create
It will create the resource in the storage backend. After this, the system will apply the desired state.

### Update
It provides two options: **Replace** and **Patch**.  

**Replace:** Resource will be updated replacing the existing spec with the provided one. *ResourceStatus* will be ignored by the system. To update this, specific status update operation must be called.  
Note: Replacing a resource object may not propagate immediately. For instance, replacing a ***ConfigMap*** or ***Secret*** will require the pods being restarted.  
**Patch:** It applies a change to a specific field. When patching complex types, arrays and maps, its application is defined on per-field basis, and it may replace current value or merge changes into it.

### Read
**Get**, **List** and **Watch**  

**Get:** It retrieves a specific resource object by name.  
**List:** It retrieves all resource objects of a specific type within a namespace, and the results can be restricted with a selector query  
**Watch:** It streams results for an object as it is updated.





## API Groups

> admissionregistration.k8s.io ***v1, v1alpha1***

> apiextensions.k8s.io ***v1***

> apiregistration.k8s.io ***v1***

> app ***v1***

> authentication.k8s.io ***v1, v1alpha1***

> authorization.k8s.io ***v1***

> autoscaling ***v2, v1***

> batch ***v1***

> certificates.k8s.io ***v1***

> coordination.k8s.io ***v1***

> core ***v1***

> discovery.k8s.io ***v1***

> events.k8s.io ***v1***

> flowcontrol.apiserver.k8s.io ***v1beta3, v1beta2***

> internal.apiserver.k8s.io ***v1alpha1***

> networking.k8s.io ***v1, v1alpha1***

> node.k8s.io ***v1***

> policy ***v1***

> rbac.authorization.k8s.io ***v1***

> resource.k8s.io ***v1alpha1***

> scheduling.k8s.io ***v1***

> storage.k8s.io ***v1, v1beta1 ***


## Workloads

Workload resources are responsible for managing and running containers inside the cluster. [Containers](/kube-api.md#containers) are created by controllers through [Pods](/kube-api.md#pods). 

