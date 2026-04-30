# Docker_bases

Base Docker para projetos

## Subir o ambiente

``bash
docker compose up -d --build
``

## Acessar o container da aplicação
``bash
docker exec -it app bash
``

## Instalar dependências do Laravel
``bash
composer install
``

## Limpar e otimizar cache do Laravel
``bash
php artisan optimize
php artisan config:clear
php artisan cache:clear
php artisan config:cache
php artisan route:clear
php artisan view:clear
``

## Rodar servidor Laravel (dentro do container)
``bash
php artisan serve --host=0.0.0.0 --port=8000
``

## Sair do container
``bash
exit
``

## Derrubar e remover volumes
``bash
docker compose down -v
``
