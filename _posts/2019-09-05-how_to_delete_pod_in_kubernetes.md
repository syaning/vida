---
layout: post
comments: true
title: How to Delete Pod in Kubernetes 
date: 2018-09-05 01:36:00
---

```shell
kubectl delete pod $(kubectl get pod --no-headers | awk '{print $1}')
```
