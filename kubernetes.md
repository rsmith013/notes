# Kubernetes

## Kubectl Commands

## General
- `kubectl {verb (get|describe)} {object (pods|secrets|deployments|services...)}`

#### Use JSON Path to extract a single element
- `kubectl get {object (pods|secrets|deployments|services...)} {object name} --output jsonpath="{.path.to.object}"`

#### View the resource manifest
- `kubectl get {object (pods|secrets|deployments|services...)} {object name} --output yaml`

### Container Logs
Without fancy interfaces like rancher, how to view the logs from a running or recently exited container

- `kubectl logs {POD_NAME}`
- `kubectl logs {POD_NAME} --previous`
