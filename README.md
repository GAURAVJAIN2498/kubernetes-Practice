# kubernetes-Practice

# set different namespace at default position

$ kubectl config set-context $(kubectl config current-context) --namespace=dev

$ kubectl config view | grep namespace:

# default range
request=minimum

limit=max

cpu:
     request=0.5
     limit=1
     
memory:
       request=500M
       limit=1G

# horizontal pod autoscaler

kubectl autoscale deployment mydeploy --cpu-percent=20 --min=1 --max=10

(when we work on given deploy pod and inc load on it automatically autoscale the pod according to demand of target and delete also when it cold down)
       
    
