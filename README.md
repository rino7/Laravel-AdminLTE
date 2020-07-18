# Modificaciones para mis proyectos

# Instrucciones para implementar cambios
⚠️ Importante: para sincronizar los cambios del repo original hay que hacer lo siguiente:
1. `git checkout master` 
2. `git fetch upstream` Busco todas las ramas del repo original
3. `git rebase upstream/master` Bajo y sincronizo el repo original en la rama master
4. Mergear `master` => `customization-dolmedo` Mergeo los cambios del repo original con mis cambios
5. (Resolver conflictos) Si hay conflictos, los resuelvo
6. `git push origin customization-dolmedo` Subo todo a mi rama. Que es la que uso para mis proyectos

Utilizar para los proyectos la rama `customization-dolmedo`

# Instrucciones para el uso
1. Seguir las [instrucciones de instalación del repo original](https://github.com/rino7/Laravel-AdminLTE/tree/master#2-installation)
2. [Habilitar el uso de laravel-mix](https://github.com/jeroennoten/Laravel-AdminLTE#610-laravel-mix)
3. Instalar package translation español: `composer require laraveles/spanish`
4. Cambiar local en `config/app.php` a `locale => 'es'`
5. Cambiar los extends de los auth/views `https://github.com/jeroennoten/Laravel-AdminLTE#54-authentication-views`
6. Agregar archivos `public/js/{project}.js` y `public/css/{project}.css` 
7. Cambiar los nombres en `config/adminlte.php` (sección plugins)
8. Gracias al uso de larave-mix, se pueden overridear los colores que trae por defecto AdminLTE. Se hace editando el archivo `resources/sass/_variables.scss`. 
9. Ejemplo:
```css
//Body
 $body-bg: #f8fafc;
 
 // Typography
 $font-family-sans-serif: 'Nunito', sans-serif;
 $font-size-base: 0.9rem;
 $line-height-base: 1.6;
 
 // Colors
 $blue: #4788c7 !default;
 //$blue: #3490dc; Original
 $indigo: #6574cd;
 $purple: #9561e2;
 $pink: #f66d9b;
 $red: #e3342f;
 $orange: #f6993f;
 $yellow: #ffed4a;
 $green: #38c172;
 $teal: #4dc0b5;
 $cyan: #6cb2eb;
 ```
