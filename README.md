# Curso de Kubernetes


## Parte 1 - Kubernetes: Pods, Services e ConfigMaps
- [x] 1. Conhecendo o Kubernetes
  - [x] 1.1 Introdução
  - [x] 1.2 O que é o Kubernetes?
  - [x] 1.3 Entendendo o Kubernetes
  - [x] 1.4 A arquitetura do Kubernetes
  - [x] 1.5 Entendendo a API
- [x] 2. Criando o cluster
  - [x] 2.1 Inicializando o cluster no Windows
  - [x] 2.2 Kubernetes e Windows
  - [x] 2.3 Inicializando o cluster no Linux
  - [x] 2.4 Instalando as ferramentas no Linux
  - [x] 2.5 Kubernetes e Linux
  - [x] 2.6 Inicializando o cluster no GCP + DOKS
- [x] 3. Criando e entendendo pods
  - [x] 3.1 Entendendo o que são pods
  - [x] 3.2 Pods e redes
  - [x] 3.3 O primeiro pod
  - [x] 3.4 Comandos do kubectl
  - [x] 3.5 Para saber mais: Onde imagens são armazenadas
  - [x] 3.6 Criando pods de maneira declarativa
  - [x] 3.7 Analisando arquivos YAML
  - [x] 3.8 Para saber mais: Validando YAML
  - [x] 3.9 Iniciando o projeto
  - [x] 3.10 Pods e containers
- [x] 4. Expondo pods com services
  - [x] 4.1 Conhecendo services
  - [x] 4.2 Vantagens de services
  - [x] 4.3 Criando um Cluster IP
  - [x] 4.4 Linkando services e pods
  - [x] 4.5 Criando um Node Port
  - [x] 4.6 Praticando NodePort's
  - [x] 4.7 Criando um Load Balancer
  - [x] 4.8 Praticando Load Balancers
- [x] 5. Aplicando services ao projeto
  - [x] 5.1 Acessando o portal
  - [x] 5.2 Definindo portas
  - [x] 5.3 Subindo o sistema
  - [x] 5.4 Escolhendo o service
  - [x] 5.5 Subindo o banco
- [x] 6. Definindo variáveis de ambiente
  - [x] 6.1 Utilizando variáveis de ambiente
  - [x] 6.2 Variáveis e definições
  - [x] 6.3 Criando um ConfigMap
  - [x] 6.4 Definindo ConfigMaps
  - [x] 6.5 Aplicando o ConfigMap ao projeto
  - [x] 6.6 Linkando Pods e ConfigMaps
  - [x] 6.7 Para saber mais: NodePort e IP's

## Parte 2 - Kubernetes: Deployments, Volumes e Escalabilidade

- [x] 7. Conhecendo ReplicaSets e Deployments
  - [x] 7.1 Introdução
  - [x] 7.2 Projeto inicial do treinamento
  - [x] 7.3 Antes de começar
  - [x] 7.4 Conhecendo ReplicaSets
  - [x] 7.5 Praticando ReplicaSets
  - [x] 7.6 Conhecendo Deployments
  - [x] 7.7 ReplicaSets vs Deployments
  - [x] 7.8 Aplicando Deployments ao projeto
  - [x] 7.9 Praticando Deployments
- [x] 8. Persistindo dados com o Kubernetes
  - [x] 8.1 Projeto da aula anterior
  - [x] 8.2 Persistindo dados com volumes
  - [x] 8.3 Volumes na prática
  - [x] 8.4 Volumes no Linux
  - [x] 8.5 Validando a definição de Volumes
  - [x] 8.6 Persistência com PersistentVolumes
  - [x] 8.7 Para saber mais: Mais informações sobre PersistentVolumes
  - [x] 8.8 Sobre PersistentVolumes
- [x] 9. Storage Classes e StatefulSets
  - [x] 9.1 Projeto da aula anterior
  - [x] 9.2 Utilizando Storage Classes
  - [x] 9.3 Sobre Storage Classes
  - [x] 9.4 Conhecendo StatefulSets
  - [x] 9.5 Sobre StatefulSets
  - [x] 9.6 Utilizando um StatefulSet
  - [x] 9.7 Analisando definições
- [x] 10. Checando status com Probes
  - [x] 10.1 Projeto da aula anterior
  - [x] 10.2 Conhecendo probes
  - [x] 10.3 Sobre probes
  - [x] 10.4 Utilizando Liveness Probes
  - [x] 10.5 Critérios do Liveness Probe
  - [x] 10.6 Utilizando Readiness Probes
  - [x] 10.7 Probes e suas instruções
  - [x] 10.8 Para saber mais: Startup Probes
- [x] 11. Como escalar com o Horizontal Pod Autoscaler
  - [x] 11.1 Projeto da aula anterior
  - [x] 11.2 Escalando pods automaticamente
  - [x] 11.3 Entendendo erros
  - [x] 11.4 Utilizando o HPA no Windows
  - [x] 11.5 Download do Git Bash
  - [x] 11.6 Definindo HPAs
  - [x] 11.7 Utilizando o HPA no Linux
  - [x] 11.8 Para saber mais: VerticalPodAutoscaler


### Estrutura do projeto implementado 
![Kubeview](https://user-images.githubusercontent.com/18218791/166169752-88dc7494-ca31-499d-87a4-f88034cf58d1.png)

### Frontend - Portal Noticias
![Login](https://user-images.githubusercontent.com/18218791/166169787-3d90ff05-db27-4d11-bbda-3b689167b22b.png)
![Front](https://user-images.githubusercontent.com/18218791/166169807-c17bd499-c6c0-48f5-88d1-8c9428e816c7.png)

### Backend - Sistema + API
![Sitema e API](https://user-images.githubusercontent.com/18218791/166169877-c24f76f1-9c0d-468d-bc34-49ed58cf13ec.png)

### DOKS
##### Cluster
![Cluster](https://user-images.githubusercontent.com/18218791/166169917-eb90037c-754d-4f4d-8f7c-526064596d2c.png)

##### LoadBalancer + Volumes
![loadbalancer](https://user-images.githubusercontent.com/18218791/166169942-8572f7aa-77c3-4789-b28b-28fa833df286.png)

### Dashboard Kubernetes
![Dashboard](https://user-images.githubusercontent.com/18218791/166169968-f4848f56-7628-4e38-ae9f-bfa3879109b6.png)
