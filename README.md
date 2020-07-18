# Modificaciones para mis proyectos

⚠️ Importante: para sincronizar los cambios del repo original hay que hacer lo siguiente:
1. `git checkout master` 
2. `git fetch upstream` Busco todas las ramas del repo original
3. `git rebase upstream/master` Bajo y sincronizo el repo original en la rama master
4. Mergear `master` => `customization-dolmedo` Mergeo los cambios del repo original con mis cambios
5. (Resolver conflictos) Si hay conflictos, los resuelvo
6. `git push origin customization-dolmedo` Subo todo a mi rama. Que es la que uso para mis proyectos

Utilizar para los proyectos la rama `customization-dolmedo`
