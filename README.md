# :notebook_with_decorative_cover: Instruções

### Rodar os comandos abaixo:

#### Preparar os Bancos de Dados
Instale uma imagem do Redis</br>
`docker run --name redis -p 6379:6379 -d -t redis:alpine`

Instale uma imagem do Postgres</br>
`docker run --name database -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres:11`

Instale uma imagem do MongoDB</br>
`docker run --name mongodb -p 27017:27017 -d -t mongo`

Rodando as migrations</br>
`yarn sequelize db:migrate`

permitindo que haja o administrador no banco</br>
`yarn sequelize db:seed:all`


Clonar projeto</br>
`$ git clone https://github.com/MitchellSymington/gobarber-api.git`

Ir para o diretório </br>
`$ cd gobarber-api`

Instalar dependencias</br>
`$ yarn install`

Subir bancos com Docker
`$ docker start database`
`$ docker start mongodb`
`$ docker start redis`

Iniciar</br>
`$ yarn dev`
`$ yarn queue`

