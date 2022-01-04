# Rodando o KIND no M1

Este repositório é minha tentativa de fazer os exemplos no meu MacBook M1

[CRIANDO UM CLUSTER K8S COM NGINX INGRESS CONTROLLER EM SUA MÁQUINA](https://youtu.be/1lx91nhzNe0)

## Instalando no macOS

Utilizando o Homebrew:

```bash
brew install kind
```

## Usando

```bash
kind create cluster --name giropops-ingress --config kind-ingress.yaml

kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/kind/deploy.yaml

kubectl create -f testing-ingress.yaml
```

## Licença
[BeerWare](https://pt.wikipedia.org/wiki/Beerware)
