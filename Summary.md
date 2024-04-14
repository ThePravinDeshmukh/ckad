## Application Deployment


Rolling update provie a zero downtime solution
maxSurge controlls how many new pods are created
When creating a deployment, use --save-config to store metadata about the deployment in the annotations
Deploy,emt support a rollout satus and history. You can rollback to previous deployment

k create deploy [deployment-name] --image=[image-name]:[tag] --dry-run=client -o yaml > deploy.yaml

