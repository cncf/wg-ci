# rkt CI / Cluster Needs

[Infrastructure Requirements from the rkt proposal](https://github.com/cncf/toc/blob/master/proposals/rkt.adoc):

CI and potentially CNCF Community Cluster access.

CI might be useful, there is an existing Jenkins CI system sponsored by CoreOS.
 
## rkt Dependencies

The rkt project uses [glide](https://github.com/Masterminds/glide) to maintain dependencies - an up-to-date manifest can be found in the [glide.lock file in the repository](https://github.com/coreos/rkt/blob/master/glide.lock).

## Current State

### CoreOS Jenkins

https://jenkins-rkt-public.prod.coreos.systems/#

### Orchestration

Kubernetes offers rkt support, including via [minikube](https://github.com/kubernetes/minikube#using-rkt-container-engine) which makes it easy to test and run locally.
 The new rkt integration via Kubernetes’s CRI (Container Runtime Interface) is currently passing 89/94 conformance tests; the hope would be to get this to 100% as Kubernetes 1.7 work begins and CRI stabilizes to beta.
