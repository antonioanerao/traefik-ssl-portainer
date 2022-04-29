### Faça o seguinte antes de iniciar o seu docker-compose

- Crie uma pasta para armazenar o conteúdo do site

      $ mkdir html
      

- Crie um volume para o seu site

      $ docker volume create --driver local --opt type=none --opt device=$(pwd)/html --opt o=bind debian10-php74-sqlsrv
            
- Rode o docker-compose
      $ docker-compose up -d
