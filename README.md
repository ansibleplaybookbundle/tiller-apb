# tiller-apb

## Requirements

### Role

This APB must run with the "admin" role in the target namespace, because it
creates a role binding.

You can set this in the automation broker's config at `openshift.sandbox_role`.

### Cluster

This APB requires OpenShift.

## Using

After deploying, you can verify that tiller is working with the helm client:

```
$ helm version --tiller-namespace=$TILLER_NS
Client: &version.Version{SemVer:"v2.8.1", GitCommit:"6af75a8fd72e2aa18a2b278cfe5c7a1c5feca7f2", GitTreeState:"clean"}
Server: &version.Version{SemVer:"v2.8.1", GitCommit:"6af75a8fd72e2aa18a2b278cfe5c7a1c5feca7f2", GitTreeState:"clean"}
```
