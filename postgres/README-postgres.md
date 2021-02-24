Reference: https://severalnines.com/database-blog/using-kubernetes-deploy-postgresql

## Setup

Will deploy Postgres for a TODO application configured with a persistent volume. Be sure to deploy in the correct namespace you desire.

```
kubectl create -f postgres/postgres-todo.yaml -n default
```

## Delete Everything
```
kubectl delete all -l app=postgres -n default
kubectl delete pvc postgres-pv-claim -n default
kubectl delete pv postgres-pv-volume -n default
```