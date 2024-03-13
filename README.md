
## Running SonarQube Self Hosted Kubernetes

Create .env file with the following keys/values

```
db-user={username}
db-password={password}
```

Execute the kubectl

```

kubectl apply -k ./
```


Note: You might need to fixed file permission after the pod creation of the SonarQube. 
```
chmod 777 {main_path}\data
chmod 777 {main_path}\extensions
chmod 777 {main_path}\logs
```

