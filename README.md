## Comandos Básicos Docker

```bash
docker --version  # Mostra a versão do Docker instalada
```

```bash
docker pull <imagem>  # Baixa uma imagem do Docker Hub
```

```bash
docker images  # Lista todas as imagens locais
```

```bash
docker run <imagem>  # Cria e inicia um novo container a partir de uma imagem
```

```bash
docker ps  # Lista todos os containers em execução
```

```bash
docker ps -a  # Lista todos os containers, incluindo os que não estão em execução
```

```bash
docker stop <container_id>  # Para um container em execução
```

```bash
docker rm <container_id>  # Remove um container parado
```

```bash
docker rmi <imagem>  # Remove uma imagem local
```

```bash
docker exec -it <container_id> /bin/bash  # Acessa o terminal de um container em execução
```

## Comandos Docker Compose

```bash
docker-compose up  # Inicia os serviços definidos no arquivo docker-compose.yml
```

```bash
docker-compose down  # Para e remove os containers definidos no arquivo docker-compose.yml
```

```bash
docker-compose build  # Constrói ou reconstrói os serviços definidos no arquivo docker-compose.yml
```

```bash
docker-compose ps  # Lista os containers gerenciados pelo Docker Compose
```

## Comandos para Portainer

```bash
docker volume create portainer_data  # Cria um volume para armazenar os dados do Portainer
```

```bash
docker run -d -p 9000:9000 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce  # Inicia o Portainer
```

```bash
docker stop portainer  # Para o container do Portainer
```

```bash
docker rm portainer  # Remove o container do Portainer
```

```bash
docker volume rm portainer_data  # Remove o volume de dados do Portainer
```
