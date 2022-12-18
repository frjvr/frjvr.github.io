---
title: Reference
approvers:
- chenopis
linkTitle: "Reference"
main_menu: true
weight: 70
content_type: concept
no_list: true
---


<!-- overview -->

This section of the Kubernetes documentation contains references.



<!-- body -->

## API Reference

* [Glossary](/docs/kubernetes/en/reference/glossary/) -  a comprehensive, standardized list of Kubernetes terminology

* [Kubernetes API Reference](/docs/kubernetes/en/reference/kubernetes-api/)
* [One-page API Reference for Kubernetes {{< param "version" >}}](/docs/kubernetes/en/reference/generated/kubernetes-api/{{< param "version" >}}/)
* [Using The Kubernetes API](/docs/kubernetes/en/reference/using-api/) - overview of the API for Kubernetes.
* [API access control](/docs/kubernetes/en/reference/access-authn-authz/) - details on how Kubernetes controls API access
* [Well-Known Labels, Annotations and Taints](/docs/kubernetes/en/reference/labels-annotations-taints/)

## Officially supported client libraries

To call the Kubernetes API from a programming language, you can use
[client libraries](/docs/kubernetes/en/reference/using-api/client-libraries/). Officially supported
client libraries:

- [Kubernetes Go client library](https://github.com/kubernetes/client-go/)
- [Kubernetes Python client library](https://github.com/kubernetes-client/python)
- [Kubernetes Java client library](https://github.com/kubernetes-client/java)
- [Kubernetes JavaScript client library](https://github.com/kubernetes-client/javascript)
- [Kubernetes C# client library](https://github.com/kubernetes-client/csharp)
- [Kubernetes Haskell client library](https://github.com/kubernetes-client/haskell)

## CLI

* [kubectl](/docs/kubernetes/en/reference/kubectl/) - Main CLI tool for running commands and managing Kubernetes clusters.
    * [JSONPath](/docs/kubernetes/en/reference/kubectl/jsonpath/) - Syntax guide for using [JSONPath expressions](https://goessner.net/articles/JsonPath/) with kubectl.
* [kubeadm](/docs/kubernetes/en/reference/setup-tools/kubeadm/) - CLI tool to easily provision a secure Kubernetes cluster.

## Components

* [kubelet](/docs/kubernetes/en/reference/command-line-tools-reference/kubelet/) - The
  primary agent that runs on each node. The kubelet takes a set of PodSpecs
  and ensures that the described containers are running and healthy.
* [kube-apiserver](/docs/kubernetes/en/reference/command-line-tools-reference/kube-apiserver/) -
  REST API that validates and configures data for API objects such as  pods,
  services, replication controllers.
* [kube-controller-manager](/docs/kubernetes/en/reference/command-line-tools-reference/kube-controller-manager/) - Daemon that embeds the core control loops shipped with Kubernetes.
* [kube-proxy](/docs/kubernetes/en/reference/command-line-tools-reference/kube-proxy/) - Can
  do simple TCP/UDP stream forwarding or round-robin TCP/UDP forwarding across
  a set of back-ends.
* [kube-scheduler](/docs/kubernetes/en/reference/command-line-tools-reference/kube-scheduler/) - Scheduler that manages availability, performance, and capacity.
  
  * [Scheduler Policies](/docs/kubernetes/en/reference/scheduling/policies)
  * [Scheduler Profiles](/docs/kubernetes/en/reference/scheduling/config#profiles)

* List of [ports and protocols](/docs/kubernetes/en/reference/ports-and-protocols/) that
  should be open on control plane and worker nodes

## Config APIs

This section hosts the documentation for "unpublished" APIs which are used to
configure  kubernetes components or tools. Most of these APIs are not exposed
by the API server in a RESTful way though they are essential for a user or an
operator to use or manage a cluster.

* [kube-apiserver configuration (v1alpha1)](/docs/kubernetes/en/reference/config-api/apiserver-config.v1alpha1/)
* [kube-apiserver configuration (v1)](/docs/kubernetes/en/reference/config-api/apiserver-config.v1/)
* [kube-apiserver encryption (v1)](/docs/kubernetes/en/reference/config-api/apiserver-encryption.v1/)
* [kube-apiserver event rate limit (v1alpha1)](/docs/kubernetes/en/reference/config-api/apiserver-eventratelimit.v1alpha1/)
* [kubelet configuration (v1alpha1)](/docs/kubernetes/en/reference/config-api/kubelet-config.v1alpha1/) and
  [kubelet configuration (v1beta1)](/docs/kubernetes/en/reference/config-api/kubelet-config.v1beta1/)
* [kubelet credential providers (v1alpha1)](/docs/kubernetes/en/reference/config-api/kubelet-credentialprovider.v1alpha1/)
* [kubelet credential providers (v1beta1)](/docs/kubernetes/en/reference/config-api/kubelet-credentialprovider.v1beta1/)
* [kube-scheduler configuration (v1beta2)](/docs/kubernetes/en/reference/config-api/kube-scheduler-config.v1beta2/),
  [kube-scheduler configuration (v1beta3)](/docs/kubernetes/en/reference/config-api/kube-scheduler-config.v1beta3/) and
  [kube-scheduler configuration (v1)](/docs/kubernetes/en/reference/config-api/kube-scheduler-config.v1/)
* [kube-proxy configuration (v1alpha1)](/docs/kubernetes/en/reference/config-api/kube-proxy-config.v1alpha1/)
* [`audit.k8s.io/v1` API](/docs/kubernetes/en/reference/config-api/apiserver-audit.v1/)
* [Client authentication API (v1beta1)](/docs/kubernetes/en/reference/config-api/client-authentication.v1beta1/) and 
  [Client authentication API (v1)](/docs/kubernetes/en/reference/config-api/client-authentication.v1/)
* [WebhookAdmission configuration (v1)](/docs/kubernetes/en/reference/config-api/apiserver-webhookadmission.v1/)
* [ImagePolicy API (v1alpha1)](/docs/kubernetes/en/reference/config-api/imagepolicy.v1alpha1/)

## Config API for kubeadm

* [v1beta2](/docs/kubernetes/en/reference/config-api/kubeadm-config.v1beta2/)
* [v1beta3](/docs/kubernetes/en/reference/config-api/kubeadm-config.v1beta3/)

## Design Docs

An archive of the design docs for Kubernetes functionality. Good starting points are
[Kubernetes Architecture](https://git.k8s.io/design-proposals-archive/architecture/architecture.md) and
[Kubernetes Design Overview](https://git.k8s.io/design-proposals-archive).
