# Flux Bootstrap

Thanks to: https://docs.technotim.live/posts/flux-devops-gitops/

## Requirements
1. Make sure flux is installed on local machine `brew install fluxcd/tap/flux`
2. `github_token` secret defined in the ansible vault

## Play
```
- hosts: localhost
  connection: local
  roles:
    - role: flux_bootstrap
```

## Caveats
Currently only support bootstrapping github (not git, gitlab, bitbucket, etc)
