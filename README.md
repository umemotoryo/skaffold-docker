# skaffold + kustomize docker image
## How to use skaffold and kustomize
- [skaffold repositry](https://github.com/GoogleContainerTools/skaffold)
- [kustomize](https://github.com/kubernetes-sigs/kustomize)

## Versions
- docker 18.06.1-ce
- kubectl v1.10.9
- skaffold v0.16.0
- kustomize v1.0.9

## How to use this image
notice: You must start docker daemon on host machine.

```
docker run --rm -it -v /var/run/docker.sock:/var/run/docker.sock -v $HOME/.kube:/root/.kube -v /path/to/your/repositry:/repositry skaffold ash -c 'cd /repositry && skaffold build'
```
