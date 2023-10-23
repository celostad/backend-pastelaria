backend-pastelaria

- Na pasta do projeto digite
composer update

php artisan key:generate

- Crie um arquivo .env e copie e cole as variáveis do arquivo .env.example
touch .env

Configure seu banco de dados.
DB_DATABASE=challenge_pastelaria
DB_USERNAME=root
DB_PASSWORD=secret

- Permissões de pastas e link simbólico :
$ chmod 777 -R storage
$ php artisan storage:link

- Para criar as tabelas e gerar as fotos dos pasteis digite os comandos:

$ php artisan migrate --seed
$ php artisan serve

Para testar o ambiente de desenvolvimento da API. use Postman ou similar.
