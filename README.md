# metabase-k8s

This is k8s to create metabase service
Before apply, make sure you have secrets. To add them use below commands
kubectl create secret generic mbpass --from-literal MB_DB_PASS=<pass>
kubectl create secret generic mbuser --from-literal MB_DB_USER=<user>
kubectl create secret generic postgresuser --from-literal POSTGRES_USER=<user>
kubectl create secret generic postgrespass --from-literal POSTGRES_PASSWORD=<pass>
kubectl create secret generic pgmail --from-literal PGADMIN_DEFAULT_EMAIL=<mail>
kubectl create secret generic pgpass --from-literal PGADMIN_DEFAULT_EMAIL=<pass>