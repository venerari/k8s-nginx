# k8s-nginx

sample1

kubectl apply -f https://raw.githubusercontent.com/venerari/k8s-nginx/master/k8s-nginx.yaml

kubectl delete deploy/my-nginx<br>
kubectl delete svc/my-nginx-svc


$ docker run -d --restart=always -e DOMAIN=cluster --name nginx-app -p 80:80 nginx

$ kubectl run --image=nginx nginx-app --port=80 --env="DOMAIN=cluster"
$ kubectl expose deployment nginx-app --port=80 --name=nginx-http
