# Docker_bases

Base Docker para projetos

## Subir o ambiente

``docker compose up -d --build``

## Acessar o container da aplicação
``docker exec -it app bash``

## Instalar dependências do Laravel
``composer install``

## Limpar e otimizar cache do Laravel
``php artisan optimize
php artisan config:clear
php artisan cache:clear
php artisan config:cache
php artisan route:clear
php artisan view:clear``

## Rodar servidor Laravel (dentro do container)
``php artisan serve --host=0.0.0.0 --port=8000``

## Sair do container
``exit``

## Derrubar e remover volumes
``docker compose down -v``
