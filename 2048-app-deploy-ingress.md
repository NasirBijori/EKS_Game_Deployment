# EKS_Game_Deployment

# 2048 App

## Create Fargate profile

```
eksctl create fargateprofile \
    --cluster demo-cluster \
    --region us-east-1 \
    --name alb-sample-app \
    --namespace game-2048
```

## Deploy the deployment, service and Ingress

```
kubectl apply -f https://raw.githubusercontent.com/kubernetes-sigs/aws-load-balancer-controller/v2.5.4/docs/examples/2048/2048_full.yaml
```
![image](https://github.com/NasirBijori/EKS_Game_Deployment/assets/93574607/13159ea9-d6f4-4713-9666-8fc871bee03b)

