# ===============================
# INICIALIZACIÓN DEL REPOSITORIO
# ===============================

git init
git add .
git commit -m "Commit inicial"


# ===============================
# CREACIÓN DE RAMAS PRINCIPALES
# ===============================

git branch main
git switch main
git switch -c develop


# ===============================
# CREACIÓN DE RAMAS DE TRABAJO
# ===============================

git switch -c feature-login
# trabajar en la feature
git add .
git commit -m "Desarrollo feature-login"


# ===============================
# CAMBIO ENTRE RAMAS
# ===============================

git switch develop
git switch feature-login


# ===============================
# MERGE DE FEATURE EN DEVELOP
# ===============================

git switch develop
git merge feature-login


# ===============================
# RESOLUCIÓN DE CONFLICTOS (SI APARECEN)
# ===============================

# editar archivos manualmente
git add archivo_en_conflicto
git commit -m "Resolución de conflicto"


# ===============================
# CONEXIÓN CON GITHUB (REMOTO)
# ===============================

git remote add origin URL_DEL_REPOSITORIO


# ===============================
# SUBIDA DE RAMAS A GITHUB
# ===============================

git push -u origin main
git push -u origin develop
git push -u origin feature-login


# ===============================
# BAJAR CAMBIOS DESDE GITHUB
# ===============================

git fetch
git pull


# ===============================
# INTEGRAR CAMBIOS ENTRE RAMAS
# ===============================

# Traer una rama completa
git merge nombre-rama

# Traer un commit concreto
git cherry-pick abc123

# Copiar solo un archivo desde otra rama
git checkout rama -- archivo


# ===============================
# ELIMINACIÓN DE RAMAS
# ===============================

# Borrar rama local
git branch -d nombre-rama

# Borrar rama remota
git push origin --delete nombre-rama


# ===============================
# FLUJO DE TRABAJO DIARIO
# ===============================

git pull
git switch develop
git switch -c feature-nueva
# trabajar en la feature
git add .
git commit -m "Cambios en feature-nueva"
git switch develop
git merge feature-nueva
git push

