### Faça o seguinte antes de iniciar o seu docker-compose

- Crie uma pasta para armazenar o conteúdo do WordPress e uma para o conteúdo do MySql

      $ mkdir wordpress
      $ mkdir database

- Crie um volume para o WordPress e outro para o MySql

      $ docker volume create --driver local --opt type=none --opt device=$(pwd)/wordpress --opt o=bind wordpress
      
      $ docker volume create --driver local --opt type=none --opt device=$(pwd)/database --opt o=bind db
      
- Rode o docker-compose
      $ docker-compose up -d
