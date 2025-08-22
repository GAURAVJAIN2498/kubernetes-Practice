# kubernetes-Practice

# set different namespace at default position

$ kubectl config set-context $(kubectl config current-context) --namespace=dev
$ kubectl config view | grep namespace:
