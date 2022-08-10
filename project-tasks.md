# Project: Deployment Roulette


## Step 1: Deployment Troubleshooting


### Fix the hello-world App Deployment


The `apps/hello-world` deployment is facing deployment issues as the health check was miconfigured 


Screenshot of a successful health check 


```
 kubectl logs hello-world-698dfc7f8-2cqv2
```


![Fix Deployment](img/fix-hello-world-dep.png)


## Step 2: Canary Deployments



````
for i in $(seq 1 20); do curl  172.20.191.186; done > canary.txt 
````

## Step 3: Blue-green Deployments

Using the `curl ec2` instance to curl the `blue-green.udacityproject` URL

![blue-green](img/green-blue.png)

Commented the resource block creating the record for blue deployment and run `terraform apply`

![green-only](img/green-only.png)