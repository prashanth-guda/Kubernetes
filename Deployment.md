
## K8s_deployment


```bash
  apiVersion: apps/v1
kind: Deployment
metadata:
  name: python-app
spec:
  replicas: 2
  selector:
    matchLabels:
      app: python-app
  template:
    metadata:
      labels:
        app: python-app
    spec:
      containers:
      - name: python-app
        image: my-python-app:latest
        ports:
        - containerPort: 5000

```
    
