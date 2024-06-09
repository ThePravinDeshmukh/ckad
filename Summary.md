## Application Deployment


Rolling update provie a zero downtime solution
maxSurge controlls how many new pods are created
When creating a deployment, use --save-config to store metadata about the deployment in the annotations
Deploy,emt support a rollout satus and history. You can rollback to previous deployment

k create deploy [deployment-name] --image=[image-name]:[tag] --dry-run=client -o yaml > deploy.yaml



## API Deprecations

Display the k8s major and minor version
kubectl version -o yaml


Display all API Groups
and versions for the cluster. sort by kind
kubectl api-resources --sort-by=kind

Display  the api group and versio nfor ingresses
Kubectl explain ingresses

Display available versions for the autoscaling API group
k api-versions | grep autoscaling

Display the preferred version for the autosysling API group

List any alpha versions enabled on the cluster
