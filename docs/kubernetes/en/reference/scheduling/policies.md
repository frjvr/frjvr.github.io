---
title: Scheduling Policies
content_type: concept
sitemap:
  priority: 0.2 # Scheduling priorities are deprecated
weight: 30
---

<!-- overview -->

In Kubernetes versions before v1.23, a scheduling policy can be used to specify the *predicates* and *priorities* process. For example, you can set a scheduling policy by
running `kube-scheduler --policy-config-file <filename>` or `kube-scheduler --policy-configmap <ConfigMap>`.

This scheduling policy is not supported since Kubernetes v1.23. Associated flags `policy-config-file`, `policy-configmap`, `policy-configmap-namespace` and `use-legacy-policy-config` are also not supported. Instead, use the [Scheduler Configuration](/docs/kubernetes/en/reference/scheduling/config/) to achieve similar behavior.

## {{% heading "whatsnext" %}}

* Learn about [scheduling](/docs/kubernetes/en/concepts/scheduling-eviction/kube-scheduler/)
* Learn about [kube-scheduler Configuration](/docs/kubernetes/en/reference/scheduling/config/)
* Read the [kube-scheduler configuration reference (v1)](/docs/kubernetes/en/reference/config-api/kube-scheduler-config.v1/)
