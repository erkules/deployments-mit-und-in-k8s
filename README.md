# Ich

erkan@linsenraum.de
@erkuleswastaken
xing/linkedin
https://devops-training.de/
https://devops-kubernetes-camp.de/


# Buzzwords

Deklarativ


# Deployments mit und in Kubernetes

Wir verwenden Hausmittel für

* Lifecyclemanagement/Upgrades
* Blue/Green Deployment
* Canary Deployment

* Recap vom Morgen (Deployment zum Kunden ausrollen)

* Deployments
* Service
* Ingress

# Deployment under the Hood

* Warum?
* Um es zu verstehen!

Deployments
ReplicaSets
Pods
~~~
kubectl -n jax applyt -f obj/deployment.yml
kubectl -n jax get all
~~~

# Vervollständigen

~~~
kubeclt -n jax apply -f obj/deployment-svc.yml
kubeclt -n jax apply -f obj/deployment-ing.yml
~~~

# Rolling Updates


* type: RollingUpdate,Recreate
* maxSurge
* maxUnavaillable
* ReadinessProbe
* minReadySeconds

# Blue Green

Update der Ingress Resource /o\

# Canary

Ein zweites Deployment mit gleichem Label *g*

Gewichtung nach Podsanzahl :/



# Service Mesh

Istio??!

https://landscape.cncf.io/category=service-proxy,api-gateway,service-mesh&format=card-mode&grouping=category


