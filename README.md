docker build -t hello .

kubectl config use-context docker-desktop

kubectl get nodes

kubectl cluster-info

docker run -d -p 5000:5000 --restart=always --name hello registry:2

docker tag hello sunwukhan/hello

docker push sunwukhan/hello

kubectl apply -f deployment.yml

kubectl get pods

kubectl get deployment

kubectl get service