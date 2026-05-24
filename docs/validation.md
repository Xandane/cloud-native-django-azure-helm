## Validation

### Prerequisites
- kind cluster running
- kubectl installed
- helm installed

### Deployment
```bash
./bootstrap.sh

erification

Check resources:

kubectl get all,cm,secret,ing -A

Check Helm releases:

helm list -A

Check storage:

kubectl get pv,pvc -A

Check pods:

kubectl get pods -A

Check autoscaling:

kubectl get hpa -A