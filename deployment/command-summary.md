kubectl apply -f ./4-deployment.yaml
kubectl get all
kubectl logs hello-769fc65b75-8r85k
kubectl logs -f hello-769fc65b75-8r85k
kubectl scale deployment/hello --replicas=3
kubectl get all
kubectl get pods
kubectl get pods -l job=say-hello
kubectl logs hello-769fc65b75-mxn25
kubectl delete pod hello-769fc65b75-mxn25
kubectl get pods -l job=say-hello