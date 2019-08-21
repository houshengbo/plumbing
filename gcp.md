# GCP project

Automation for the `tektoncd` org runs in a GKE cluster which
[members of the governing board](https://github.com/tektoncd/community/blob/master/governance.md#permissions-and-access)
have access to.

- The GCP project the is used for GKE, storage, etc. is called
  [`tekton-releases`](http://console.cloud.google.com/home/dashboard?project=tekton-releases)
- The GKE cluster that `Prow` (and `Tekton`) run in is called
  [`prow`](https://console.cloud.google.com/kubernetes/clusters/details/us-central1-a/prow?project=tekton-releases)

This project and cluster are used for:

- [CI automation with Prow](prow.md)
- Release automation, e.g.
  [Tekton Pipelines releases](https://github.com/tektoncd/pipeline/tree/master/tekton#release-pipeline)