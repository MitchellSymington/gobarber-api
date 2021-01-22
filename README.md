# :notebook_with_decorative_cover: Instruções

### :fire: Rodar os comandos abaixo:

:one: Instale uma imagem do Redis</br>
`ddocker run --name redisbarber -p 6379:6379 -d -t redis:alpine`

:two: Instale uma imagem do Postgres</br>
`docker run --name database -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres:11`

:three: Instale uma imagem do MongoDB</br>
`docker run --name mongobarber -p 27017:27017 -d -t mongo`

:four: Subir bancos com Docker</br>
`$ docker start database`</br>
`$ docker start mongobarber`</br>
`$ docker start redisbarber`</br>

:five: Clonar projeto</br>
`$ git clone https://github.com/MitchellSymington/gobarber-api.git`

:six: Ir para o diretório </br>
`$ cd gobarber-api`

:seven: Rodando as migrations</br>
`yarn sequelize db:migrate`

:eight: Permitindo que haja o administrador no banco</br>
`yarn sequelize db:seed:all`

:nine: Instalar dependencias</br>
`$ yarn install`


:keycap_ten: Iniciar</br>
`$ yarn dev`</br>
`$ yarn queue`</br>

