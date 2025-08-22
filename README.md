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
    
