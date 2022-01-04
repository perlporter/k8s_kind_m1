# README.md

brew install kind

kind create cluster --name giropops-ingress --config kind-ingress.yaml

kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/kind/deploy.yaml

kubectl create -f testing-ingress.yaml

