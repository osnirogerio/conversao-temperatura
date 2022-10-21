# Projeto conversão de temperatura

### Passos para execução do container

  Com o docker instalado realize o download do projeto.
  
  Navegue até o conversao-temperatura/src/
  
  execute o comando :
  
  docker  build -t seuuser/conversao-temperatura:v1 .

  Para realizar o push da sua imagem para o Hubdocker
  
  docker push seuuser/conversao-temperatura:v1


  e a latest
  
  docker push seuuser/conversao-temperatura:latest

  execute o container
  
  docker container run -d -p 8080:8080 seuuser/conversao-temperatura:v1
  
  No navegador digite http://localhost:8080, para visualizar a aplicação.

### aula 02 
k3d cluster create meucluster -p "80:30000@loadbalancer"

docker build -t seuuser/conversao-temperatura:v1 .

docker image ls

docker push seuuser/conversao-temperatura:v1

docker tag seuuser/conversao-temperatura:v1 seuuser/conversao-temperatura:latest


docker push seuuser/conversao-temperatura:latest

cd k8s

kubectl apply -f deployment.yaml
