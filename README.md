# Rancher Fleet Testing

## Installation

1. Navigate to Cluster Explorer -> Continuous Delivery -> Git Repos.

```yaml
apiVersion: fleet.cattle.io/v1alpha1
kind: GitRepo
metadata:
  name: oxr463-rancher-fleet-testing
  namespace: fleet-local
spec:
  branch: master
  insecureSkipTLSVerify: false
  paths: []
  repo: https://github.com/oxr463/rancher-fleet-testing.git
  targets:
  - clusterSelector: {}
type: fleet.cattle.io.gitrepo
```

## Reference

- [Fleet Docs - Expected Repo Structure](https://fleet.rancher.io/gitrepo-structure)
