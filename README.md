# Blog

Aplicación de ejemplo Laravel.

## Puesta en marcha

1. Arranca [dockerbox](https://github.com/ijaureguialzo/dockerbox).

2. Clona este repositorio de modo que quede en `sites/blog`.
3. Abre el directorioz `blog` en PhpStorm.

4. Crea una entrada para `blog.dockerbox.test` en el fichero `hosts` de tu sistema operativo.
5. Recarga la configuración con `make reload`.

6. Copia el fichero `.env.example` a `.env` y `.env.testing`.

7. Entra en el workspace con `make workspace` y navega al directorio `blog`.
8. Crea la clave de aplicación con `php artisan key:generate`.

9. Accede a `phpmyadmin.dockerbox.test` y crea dos usuarios con sus bases de datos asociadas: `blog` y `test`.
10. Modifica los ficheros de configuración para que apunten cada uno a su base de datos.
11. Lanza las migraciones de la base de datos con `php artisan migrate`.
12. Inserta datos de ejemplo con `php artisan db:seed`.

13. Accede a la web en `https://blog.dockerbox.test`.

14. Lanza los tests con `vendor/bin/phpunit`.
15. Genera el informe de cobertura de test
    con `XDEBUG_MODE=coverage vendor/bin/phpunit --colors --stop-on-failure --coverage-html coverage`.
