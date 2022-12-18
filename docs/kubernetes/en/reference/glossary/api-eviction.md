---
title: API-initiated eviction
id: api-eviction
date: 2021-04-27
full_link: /docs/kubernetes/en/concepts/scheduling-eviction/api-eviction/
short_description: >
  API-initiated eviction is the process by which you use the Eviction API to create an
  Eviction object that triggers graceful pod termination.
aka:
tags:
- operation
---
API-initiated eviction is the process by which you use the [Eviction API](/docs/kubernetes/en/reference/generated/kubernetes-api/{{<param "version">}}/#create-eviction-pod-v1-core)
to create an `Eviction` object that triggers graceful pod termination.

<!--more-->

You can request eviction either by directly calling the Eviction API 
using a client of the kube-apiserver, like the `kubectl drain` command. 
When an `Eviction` object is created, the API server terminates the Pod. 

API-initiated evictions respect your configured [`PodDisruptionBudgets`](/docs/kubernetes/en/tasks/run-application/configure-pdb/)
and [`terminationGracePeriodSeconds`](/docs/kubernetes/en/concepts/workloads/pods/pod-lifecycle#pod-termination).

API-initiated eviction is not the same as [node-pressure eviction](/docs/kubernetes/en/concepts/scheduling-eviction/node-pressure-eviction/).

* See [API-initiated eviction](/docs/kubernetes/en/concepts/scheduling-eviction/api-eviction/) for more information.
