---
title: "Scheduling, Preemption and Eviction"
weight: 95
content_type: concept
description: >
  In Kubernetes, scheduling refers to making sure that Pods are matched to Nodes
  so that the kubelet can run them. Preemption is the process of terminating 
  Pods with lower Priority so that Pods with higher Priority can schedule on 
  Nodes. Eviction is the process of proactively terminating one or more Pods on
  resource-starved Nodes.
no_list: true
---

In Kubernetes, scheduling refers to making sure that {{<glossary_tooltip text="Pods" term_id="pod">}}
are matched to {{<glossary_tooltip text="Nodes" term_id="node">}} so that the
{{<glossary_tooltip text="kubelet" term_id="kubelet">}} can run them. Preemption
is the process of terminating Pods with lower {{<glossary_tooltip text="Priority" term_id="pod-priority">}}
so that Pods with higher Priority can schedule on Nodes. Eviction is the process
of terminating one or more Pods on Nodes.

## Scheduling

* [Kubernetes Scheduler](/docs/kubernetes/en/concepts/scheduling-eviction/kube-scheduler/)
* [Assigning Pods to Nodes](/docs/kubernetes/en/concepts/scheduling-eviction/assign-pod-node/)
* [Pod Overhead](/docs/kubernetes/en/concepts/scheduling-eviction/pod-overhead/)
* [Pod Topology Spread Constraints](/docs/kubernetes/en/concepts/scheduling-eviction/topology-spread-constraints/)
* [Taints and Tolerations](/docs/kubernetes/en/concepts/scheduling-eviction/taint-and-toleration/)
* [Scheduling Framework](/docs/kubernetes/en/concepts/scheduling-eviction/scheduling-framework)
* [Dynamic Resource Allocation](/docs/kubernetes/en/concepts/scheduling-eviction/dynamic-resource-allocation)
* [Scheduler Performance Tuning](/docs/kubernetes/en/concepts/scheduling-eviction/scheduler-perf-tuning/)
* [Resource Bin Packing for Extended Resources](/docs/kubernetes/en/concepts/scheduling-eviction/resource-bin-packing/)
* [Pod Scheduling Readiness](/docs/kubernetes/en/concepts/scheduling-eviction/pod-scheduling-readiness/)

## Pod Disruption

{{<glossary_definition term_id="pod-disruption" length="all">}}

* [Pod Priority and Preemption](/docs/kubernetes/en/concepts/scheduling-eviction/pod-priority-preemption/)
* [Node-pressure Eviction](/docs/kubernetes/en/concepts/scheduling-eviction/node-pressure-eviction/)
* [API-initiated Eviction](/docs/kubernetes/en/concepts/scheduling-eviction/api-eviction/)
