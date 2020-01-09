# Inblood
Sistema que permite la interacción entre potenciales donantes y un banco de sangre para que se lleven a cabo las donaciones de sangre.

## Instalación

1. Abrir terminal donde se quiere crear la carpeta del proyecto
2. Clonar repositorio de GitHub
```bash
git clone https://github.com/yodonante/inblood
cd inblood
```
3. Correr dependencias
```bash
composer install
composer dump-autoload
npm install
```
4. Crear una base de datos
5. Crear un archivo `.env` en base a `.env.example`
```bash
cp .env.example .env
```
6. Editar archivo `.env` con la base de datos que se acaba de crear
7. Generar la llave de la aplicación
```bash
php artisan key:generate
```
8. Correr seed
```bash
php artisan migrate:refresh --seed
```
9. Vínculo public/storage
```bash
php artisan storage:link
```

## Paquetes

1. [laravel-permission](https://github.com/spatie/laravel-permission) : Para el uso de roles y permisos.


## Solución a errores comunes:

### Errores de Vue: 

#### - Error code ELIFECYCLE ####

1. Ejecutar en la consola:  ```npm cache clean --force```
2. Eliminar carpeta ```node_modules```
3. Eliminar archivo ```package-lock.json```
4. Ejecutar en la consola:  ```npm install```
