# Blog

Aplicación de ejemplo Laravel.

## Puesta en marcha

1. Arranca [dockerbox](https://github.com/ijaureguialzo/dockerbox).
2. Clona este repositorio de modo que quede en `sites/blog`.
3. Abre el proyecto en PhpStorm.
4. Crea una entrada para `blog.dockerbox.test` en el fichero `/etc/hosts`.
5. Recarga la configuración con `make reload`.
6. Accede a `phpmyadmin.dockerbox.test` y crea dos usuarios con sus bases de datos: `blog` y `test`.
7. Copia el fichero `.env.example` a `.env` y `.env.testing`.
8. Entra en el workspace con `make workspace` y navega al directorio `blog`.
9. Crea la clave de aplicación con `php artisan key:generate`.
10. Edita los datos de configuración de la base de datos en los ficheros `.env`.
11. Accede a la web en `https://blog.dockerbox.test`.
12. Lanza los tests con `vendor/bin/phpunit tests/Feature/EntradaTest.php`.
