# Práctica Evaluable
git config --global user.email "tu@email.com"
git config --global user.name "Tu Nombre"
Estos comandos configuran la información del usuario que realizará cambios en el repositorio. Debes sustituir "tu@email.com" con tu dirección de correo electrónico y "Tu Nombre" con tu nombre.

mkdir practica_evaluable
cd practica_evaluable
git init
Crea un nuevo directorio llamado practica_evaluable, navega al directorio y lo inicializa como un repositorio Git.

git clone https://github.com/Bilal00211/Entornos2.git practica_evaluable_2
Clona un repositorio remoto desde GitHub a un nuevo directorio llamado practica_evaluable_2.

echo "Contenido del documento 1" > documento1.txt
echo "Contenido del documento 2" > documento2.txt
git add documento1.txt documento2.txt
git commit -m "Primer commit con dos documentos"
Crea dos archivos (documento1.txt y documento2.txt), añade cambios al área de preparación y realiza el primer commit.

echo "Nuevas líneas en documento 1" >> documento1.txt
git add documento1.txt
git commit -m "Añadidas líneas al documento 1"
Añade nuevas líneas al documento1.txt, añade los cambios al área de preparación y realiza un nuevo commit.

git revert HEAD
Revierte el último commit creado, creando un nuevo commit que deshace los cambios realizados.

git remote add origin https://github.com/Bilal00211/Entornos2.git
git push -u origin main
Configura el repositorio remoto llamado "origin" y sube los cambios al remoto en la rama main.

git checkout -b mirama
echo "Contenido de rama1" > rama1.txt
echo "Contenido de rama2" > rama2.txt
git add rama1.txt rama2.txt
git commit -m "Primer commit en mirama"
Crea una nueva rama llamada mirama, cambia a esa rama y realiza cambios en dos nuevos archivos.

git checkout main
git merge mirama
git branch -d mirama
Cambia a la rama main, fusiona los cambios de mirama en main y borra la rama mirama.

git push origin main
Sincroniza los cambios locales en la rama main con el repositorio remoto.

git tag V1
git push --tags
Crea una etiqueta llamada V1 y sube todas las etiquetas al repositorio remoto.

git clone https://github.com/Bilal00211/Entornos2.git practica_evaluable_2
Clona el repositorio remoto en un nuevo directorio llamado practica_evaluable_2.

cd practica_evaluable_2
git checkout -b mirama
echo "Cambios en documento1 en mirama" >> documento1.txt
git add documento1.txt
git commit -m "Cambios en documento1 en mirama"
git push -u origin mirama
Cambia al nuevo directorio, crea y cambia a una nueva rama llamada mirama, realiza cambios y sube la rama al repositorio remoto.

git checkout main
echo "Cambios en documento2 en main" >> documento2.txt
git add documento2.txt
git commit -m "Cambios en documento2 en main"
git push origin main
Cambia a la rama main, realiza cambios y sube la rama al repositorio remoto.

git checkout mirama
git merge main
git branch -d main
git push origin --delete main
git push origin mirama
Cambia a la rama mirama, fusiona los cambios de main, borra la rama main y sube los cambios al remoto.

echo "Nuevos cambios en documento2 en mirama" >> documento2.txt
git add documento2.txt
git commit -m "Nuevos cambios en documento2 en mirama"
Realiza cambios adicionales en documento2.txt en la rama mirama.

git checkout -b mirama_nueva
echo "Cambios diferentes en documento2 en mirama_nueva" >> documento2.txt
git add documento2.txt
git commit -m "Cambios diferentes en documento2 en mirama_nueva"
git checkout main
git merge mirama_nueva
 Resolver conflicto manualmente
git add documento2.txt
git merge --continue
Crea y cambia a una nueva rama llamada mirama_nueva, realiza cambios en documento2.txt, fusiona con main y resuelve conflictos.

git push origin main
Sincroniza los cambios en la rama main con el repositorio remoto.

echo "# Práctica Evaluable" > README.md
git add README.md
git commit -m "Añadido README.md"
git push origin main
Crea un archivo README.md, añade al área de preparación y sube al remoto.

cd ..
git clone https://github.com/Bilal00211/Entornos2.git practica_evaluable_2
Clona el repositorio remoto en un nuevo directorio llamado practica_evaluable_2.

cd practica_evaluable_2
ls
Verifica los archivos en el nuevo directorio clonado.
