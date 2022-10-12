# Arquitetura e Administração de Containers, Microservices, Kubernetes

<p align="center" width="100%">
    <img src="https://avatars.githubusercontent.com/u/5429470?s=200&v=4" width="100" />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
    <img src="https://github.com/docker/compose/blob/v2/logo.png?raw=true" width="100" />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
    <img src="https://github.com/kubernetes/kubernetes/raw/master/logo/logo.png" width="100" />

</p>

---

## Tecnologias

- [Docker](https://www.docker.com/);
- [Docker Compose](https://docs.docker.com/compose/);
- [Kubernetes](https://kubernetes.io/);

## Docker

Para instalar o docker acesse esse [link](https://docs.docker.com/engine/install/).

**Logar no Docker Hub**

```bash
docker login
```

**Criando Imagem**

```bash
docker build -t lucaslira/avaliacao:questao01 .
```

**Criando Container**

```bash
docker run -d -p 8080:80 --name avaliacao01 lucaslira/avaliacao:questao01
```

**Subindo Imagem para o Container Registre**

```bash
docker image push lucaslira/avaliacao:questao01
```

## Docker Compose

Para instalar o docker compose acesse esse [link](https://docs.docker.com/compose/install/).

**Rodar docker compose**

```bash
docker-compose up --build -d
```

## Kubernetes

> ⚠️ Para executar esses exemplos, vamos instalar o [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/) para executar a CLI e o [minikube](https://kubernetes.io/pt-br/docs/tutorials/hello-minikube/) que disponibiliza um ambiente Kubernetes gratuito e acessível via navegador

**Criar pod**

```bash
kubectl create -f pod-meu-nginx.yaml
```

**Visualizar pods**

```bash
kubectl get pods
```

**Criar deployment**

```bash
kubectl create -f deploy-meu-nginx.yaml
```

**Visualizar deployments**

```bash
kubectl get deployments
```

**Criar service**

```bash
kubectl create -f service-meu-nginx.yaml
```

**Visualizar services**

```bash
kubectl get svc
```

> ⚠️ Agora só acessar o ambiente através do comando **minikube dashboard**

## Como contribuir

- Faça um fork desse repositório;
- Cria uma branch com a sua feature: `git checkout -b feature/minha-feature`;
- Faça commit das suas alterações: `git commit -m 'feat: Minha nova feature'`;
- Faça push para a sua branch: `git push origin feature/minha-feature`.

Depois que o merge da sua pull request for feito, você pode deletar a sua branch.

Feito com 💜 &nbsp;por Marcos Vinicius 👋 &nbsp;[Mande um Aló](https://www.linkedin.com/in/marcos-vinicius-38a320187/)
