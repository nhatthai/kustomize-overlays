# Kubernetes Kustomize Overlays
    Example: create overlays for each environment using Kustomize

### Prerequisite
    + Install Minikube
    + Install [Kustomize](https://kubectl.docs.kubernetes.io/installation/kustomize/)

### Usage
+ Build Base
    ```
    kustomize build .\base
    ```

+ Preview output in Test
    ```
    kustomize build overlays/test
    ```

+ Apply/Deploy output in Test
    ```
    kustomize build overlays/test | kubectl apply -f -
    ```