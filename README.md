# Wordpress-and-MySQL-docker-compose
To use the docker-compose.yml file to create a Wordpress site with a MySQL database. Uses volumes (within the Linux VM) to store data.
Just have Docker Desktop open and in your command line run:
```
docker compose up
```

If you want to use Kubernetes instead, have Docker Desktop open with Kubernetes on and use the single-replica-app.yml file by running this command:
```
kubectl apply -f single-replica-app.yml
```

To close it and keep your persistent volumes run this command in your terminal:
```
kubectl delete service/mysql-service service/wordpress-service deployment.apps/db deployment.apps/frontend
```
