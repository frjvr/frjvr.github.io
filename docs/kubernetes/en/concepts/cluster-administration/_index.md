---
title: Cluster Administration
reviewers:
- davidopp
- lavalamp
weight: 100
content_type: concept
description: >
  Lower-level detail relevant to creating or administering a Kubernetes cluster.
no_list: true
---

<!-- overview -->

The cluster administration overview is for anyone creating or administering a Kubernetes cluster.
It assumes some familiarity with core Kubernetes [concepts](/docs/kubernetes/en/concepts/).

<!-- body -->

## Planning a cluster

See the guides in [Setup](/docs/kubernetes/en/setup/) for examples of how to plan, set up, and configure
Kubernetes clusters. The solutions listed in this article are called *distros*.

{{< note  >}}
Not all distros are actively maintained. Choose distros which have been tested with a recent
version of Kubernetes.
{{< /note >}}

Before choosing a guide, here are some considerations:

- Do you want to try out Kubernetes on your computer, or do you want to build a high-availability,
  multi-node cluster? Choose distros best suited for your needs.
- Will you be using **a hosted Kubernetes cluster**, such as
  [Google Kubernetes Engine](https://cloud.google.com/kubernetes-engine/), or **hosting your own cluster**?
- Will your cluster be **on-premises**, or **in the cloud (IaaS)**? Kubernetes does not directly
  support hybrid clusters. Instead, you can set up multiple clusters.
- **If you are configuring Kubernetes on-premises**, consider which
  [networking model](/docs/kubernetes/en/concepts/cluster-administration/networking/) fits best.
- Will you be running Kubernetes on **"bare metal" hardware** or on **virtual machines (VMs)**?
- Do you **want to run a cluster**, or do you expect to do **active development of Kubernetes project code**?
  If the latter, choose an actively-developed distro. Some distros only use binary releases, but
  offer a greater variety of choices.
- Familiarize yourself with the [components](/docs/kubernetes/en/concepts/overview/components/) needed to run a cluster.

## Managing a cluster

* Learn how to [manage nodes](/docs/kubernetes/en/concepts/architecture/nodes/).

* Learn how to set up and manage the [resource quota](/docs/kubernetes/en/concepts/policy/resource-quotas/) for shared clusters.

## Securing a cluster

* [Generate Certificates](/docs/kubernetes/en/tasks/administer-cluster/certificates/) describes the steps to
  generate certificates using different tool chains.

* [Kubernetes Container Environment](/docs/kubernetes/en/concepts/containers/container-environment/) describes
  the environment for Kubelet managed containers on a Kubernetes node.

* [Controlling Access to the Kubernetes API](/docs/kubernetes/en/concepts/security/controlling-access) describes
  how Kubernetes implements access control for its own API.

* [Authenticating](/docs/kubernetes/en/reference/access-authn-authz/authentication/) explains authentication in
  Kubernetes, including the various authentication options.

* [Authorization](/docs/kubernetes/en/reference/access-authn-authz/authorization/) is separate from
  authentication, and controls how HTTP calls are handled.

* [Using Admission Controllers](/docs/kubernetes/en/reference/access-authn-authz/admission-controllers/)
  explains plug-ins which intercepts requests to the Kubernetes API server after authentication
  and authorization.

* [Using Sysctls in a Kubernetes Cluster](/docs/kubernetes/en/tasks/administer-cluster/sysctl-cluster/)
  describes to an administrator how to use the `sysctl` command-line tool to set kernel parameters
.

* [Auditing](/docs/kubernetes/en/tasks/debug/debug-cluster/audit/) describes how to interact with Kubernetes'
  audit logs.

### Securing the kubelet

* [Control Plane-Node communication](/docs/kubernetes/en/concepts/architecture/control-plane-node-communication/)
* [TLS bootstrapping](/docs/kubernetes/en/reference/access-authn-authz/kubelet-tls-bootstrapping/)
* [Kubelet authentication/authorization](/docs/kubernetes/en/reference/access-authn-authz/kubelet-authn-authz/)

## Optional Cluster Services

* [DNS Integration](/docs/kubernetes/en/concepts/services-networking/dns-pod-service/) describes how to resolve
  a DNS name directly to a Kubernetes service.

* [Logging and Monitoring Cluster Activity](/docs/kubernetes/en/concepts/cluster-administration/logging/)
  explains how logging in Kubernetes works and how to implement it.

