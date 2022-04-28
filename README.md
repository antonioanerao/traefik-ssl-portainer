# Traefik para usar em producao

- Clonar o repositorio e acessar a pasta do projeto

      $ git clone git@github.com:aneraojunior/traefik-producao.git
               
- Criar uma rede chamada proxy

      $ docker network create proxy
      
- Editar o dominio no arquivo docker.compose.yml
- Editar o dominio no arquivo data/traefik.yml
- Editar a senha do Traefik Dashboard em data/configurations/dynamic.yml (formato bcrypt)
- Alterar a permissão do arquivo data/acme.json para 600

      chmod 600 acme.json
      
- Rode o Docker Compose

      $ docker-compose up -d
      
- Acesse a pasta main e edite o arquivo docker-compose.yml com seu dominio e rode o Docker Compose (opção 1)

      $ docker-compose up -d

- Antes de rodar o docker-compose do wordpress, leia as instruções que estão na pasta (opç
