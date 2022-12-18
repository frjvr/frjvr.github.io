---
title: API Access Control
weight: 30
no_list: true
---

For an introduction to how Kubernetes implements and controls API access,
read [Controlling Access to the Kubernetes API](/docs/kubernetes/en/concepts/security/controlling-access/).

Reference documentation:

- [Authenticating](/docs/kubernetes/en/reference/access-authn-authz/authentication/)
   - [Authenticating with Bootstrap Tokens](/docs/kubernetes/en/reference/access-authn-authz/bootstrap-tokens/)
- [Admission Controllers](/docs/kubernetes/en/reference/access-authn-authz/admission-controllers/)
   - [Dynamic Admission Control](/docs/kubernetes/en/reference/access-authn-authz/extensible-admission-controllers/)
- [Authorization](/docs/kubernetes/en/reference/access-authn-authz/authorization/)
   - [Role Based Access Control](/docs/kubernetes/en/reference/access-authn-authz/rbac/)
   - [Attribute Based Access Control](/docs/kubernetes/en/reference/access-authn-authz/abac/)
   - [Node Authorization](/docs/kubernetes/en/reference/access-authn-authz/node/)
   - [Webhook Authorization](/docs/kubernetes/en/reference/access-authn-authz/webhook/)
- [Certificate Signing Requests](/docs/kubernetes/en/reference/access-authn-authz/certificate-signing-requests/)
   - including [CSR approval](/docs/kubernetes/en/reference/access-authn-authz/certificate-signing-requests/#approval-rejection)
     and [certificate signing](/docs/kubernetes/en/reference/access-authn-authz/certificate-signing-requests/#signing)
- Service accounts
  - [Developer guide](/docs/kubernetes/en/tasks/configure-pod-container/configure-service-account/)
  - [Administration](/docs/kubernetes/en/reference/access-authn-authz/service-accounts-admin/)
- [Kubelet Authentication & Authorization](/docs/kubernetes/en/reference/access-authn-authz/kubelet-authn-authz/)
  - including kubelet [TLS bootstrapping](/docs/kubernetes/en/reference/access-authn-authz/kubelet-tls-bootstrapping/)
