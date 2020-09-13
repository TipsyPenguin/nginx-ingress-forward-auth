![image-20200512154011363](./README.assets/image-20200512154011363.png)

![sequencediagram](./README.assets/sequencediagram.png)

Enable ingress addon:
```bash
minikube addons  enable ingress
```

Install auth-service:
```bash
helm install auth ./auth
```

Install app-service:
```bash
helm isntall app ./app
```

Run newman tests for postman-collection:
```
newman run forward-auth.postman_collection.json
```
