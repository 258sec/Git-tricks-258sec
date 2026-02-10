INICIALIZACIÓN DEL REPOSITORIO



- git init
- git add .
- git commit -m "Commit inicial"

─────────────────────────────

CREACIÓN DE RAMAS PRINCIPALES



- git branch main
- git switch main
- git switch -c develop

────────────────────────────

CREACIÓN DE RAMAS DE TRABAJO



- git switch -c feature-login
- git add .
- git commit -m "Desarrollo feature-login"

───────────────────────────

CAMBIO ENTRE RAMAS



- git switch develop
- git switch feature-login

──────────────────

MERGE DE FEATURE EN DEVELOP



- git switch develop
- git merge feature-login

──────────────────────────

RESOLUCIÓN DE CONFLICTOS (SI APARECEN)



- git add archivo_en_conflicto
- git commit -m "Resolución de conflicto"

─────────────────────────────────────

CONEXIÓN CON GITHUB (REMOTO)



- git remote add origin URL_DEL_REPOSITORIO

───────────────────────────

SUBIDA DE RAMAS A GITHUB



- git push -u origin main
- git push -u origin develop
- git push -u origin feature-login

───────────────────────

BAJAR CAMBIOS DESDE GITHUB



- git fetch
- git pull

─────────────────────────

INTEGRAR CAMBIOS ENTRE RAMAS


- Traer una rama completa:

git merge nombre-rama


- Traer un commit concreto:

git cherry-pick abc123


- Copiar un archivo desde otra rama:

git checkout rama -- archivo

───────────────────────────

ELIMINACIÓN DE RAMAS

- Borrar rama local:

git branch -d nombre-rama


- Borrar rama remota:

git push origin --delete nombre-rama

───────────────────

FLUJO DE TRABAJO DIARIO

1- git pull

2- git switch develop

3- git switch -c feature-nueva

4- git add .

5- git commit -m "Cambios en feature-nueva"

6- git switch develop

7- git merge feature-nueva

8- git push


──────────────────────
