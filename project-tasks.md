# Project: Deployment Roulette


## Step 1: Deployment Troubleshooting


### Fix the hello-world App Deployment


The `apps/hello-world` deployment is facing deployment issues as the health check was miconfigured 


Screenshot of a successful health check 


```
 kubectl logs hello-world-698dfc7f8-2cqv2
```


![Terraform apply](img/fix-hello-world-dep.png)