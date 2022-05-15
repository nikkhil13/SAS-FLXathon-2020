We created a model in Python and publish it to a private Docker destination. The connections are already configured on the EEC171 image. Once you book a EEC171 image, you will receive a 2vCPU CentOS with Docker installed. 

*  Within the Model Manager Screen, publish the Model in to a Private Docker Destination - which is already configured. 
*  In order to see your docker image, SSH to your EEC171 CentOS machine using "root" and "Orion123"

Type the following commands - 

```sh
docker ps
```
This will list down the docker processes running on your machine.

```sh
docker exec -it *name_of_the_registry* sh
```

You are now inside the docker registry. Change the directory to repositories.

```sh
cd /var/lib/registry/docker/registry/v2/repositories
```

You will see your model here. 

In ordet to simulate the resquests to the model to demonstrate container elasticity, we use a tool called as Apache Bench. Use the below command to test the same - 

```sh
ab -p json.txt -T application/json -c 100 -n 100000 http://10.96.4.77/final_result/
```

You can visualize the containers using Weave Scope using below link - 

```sh
http://10.96.6.6:31450/#!/state/{%22topologyId%22:%22pods%22,%22topologyOptions%22:{%22pods%22:{%22namespace%22:[%22default%22]}}}
```