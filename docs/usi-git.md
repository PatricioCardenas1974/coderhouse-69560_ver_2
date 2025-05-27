## Uso de Git

Crear una rama o branch llamada prueba:

   git branch prueba

Cambiar a esa rama

   git switch prueba

Listar las ramas para ver que se esta bien parado

    git branch

Hacer los cambios necesarios y enviarlos al staging area.

    git add archivo

o, si queremos pasar todos los archivos, hacer:

     git add .

Luego, crear un commit con un mensaje

     git commit -m "Comentario sobre los cambios hechos"

[Leer: Convenciones de mensajes de commit] (3-mensaje-commit.md)

Una vez que se terminaron de hacer todos los commit necesarios y se los quiere
fusionar a la rama principal, tener cuidado de no dejar archivos con cambios sin
commit. Pararse en la rama principal.

      git checkout manin

Fusionar los commit de la rama prueba en main:

      git merge prueba

Se puede seguir trabajando en prueba:

      git checkout prueba

o se la puede borrar:

      git branch -D prueba

Cuando se quieran subir los cambios a la nube, es decir, a Github, cambiarse a la rama principal:

    git checkout main

y luego "empujar" todos los commit nuevos a la rama main de Github (se llama origin/main)

    git push