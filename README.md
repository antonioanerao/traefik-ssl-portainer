# Traefik para usar em producao

- Clonar o repositorio e acessar a pasta do projeto

      $ git clone git@github.com:aneraojunior/traefik-producao.git
               
- Criar uma rede chamada proxy

      $ docker network create proxy
      
- Editar o dominio no arquivo docker.compose.yml
- Editar o dominio no arquivo data/traefik.yml
- Editar a senha do Traefik Dashboard em data/configurations/dynamic.yml (formato bcrypt)
- Rode o Docker Compose

      $ docker-compose up -d
      
- Acesse a pasta main e edite o arquivo docker-compose.yml com seu dominio
- Rode o Docker Compose

      $ docker-compose up -d
