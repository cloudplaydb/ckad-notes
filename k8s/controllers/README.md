### Reference: 
+ https://kubernetes.io/docs/concepts/workloads/controllers/deployment/

### Commands: 

kubectl apply -f nginx-deployment.yaml
kubectl get deployments
kubectl get rs
kubectl get pods --show-labels
kubectl set image deployment.v1.apps/nginx-deployment nginx=nginx:1.16.1
kubectl edit deployment/nginx-deployment
kubectl rollout status deployment/nginx-deployment
kubectl describe deployments
kubectl rollout history deployment/nginx-deployment
kubectl rollout history deployment/nginx-deployment --revision=2
kubectl rollout undo deployment/nginx-deployment
kubectl rollout undo deployment/nginx-deployment --to-revision=2
kubectl get deployment nginx-deployment
kubectl describe deployment nginx-deployment
kubectl scale deployment/nginx-deployment --replicas=10
kubectl autoscale deployment/nginx-deployment --min=10 --max=15 --cpu-percent=80
kubectl get deploy
kubectl set image deployment/nginx-deployment nginx=nginx:sometag
kubectl rollout pause deployment/nginx-deployment
kubectl set image deployment/nginx-deployment nginx=nginx:1.16.1
kubectl set resources deployment/nginx-deployment -c=nginx --limits=cpu=200m,memory=512Mi
kubectl rollout resume deployment/nginx-deployment
kubectl get rs -w
kubectl rollout status deployment/nginx-deployment
kubectl patch deployment/nginx-deployment -p '{"spec":{"progressDeadlineSeconds":600}}'
kubectl get deployment nginx-deployment -o yaml
kubectl rollout status deployment/nginx-deployment