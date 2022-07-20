# Guia de GIT:

## Credenciales:
(https://docs.github.com/es/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

ssh-keygen -t ed25519 -C "your_email@example.com"
Vamos a git y lo añadimos en el repositorio
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/<cert_name>

## Crear el repositorio remoto

git init
git remote add origin <ssh_url>
git clone origin

## Crear una nueva rama

git checkout -b <nombre> //Crea una nueva rama y cambia directamente a ella
git branch <nombre> //Crea la rama
git checkout <nombre> //Cambia a esa rama

git branch -d <nombre> //Borra la rama

git push origin -d <nombre> //Borra una rama remota

## Mergear una rama
git checkout <mergeada> //Volvemos a la rama en la que vamos a mergear
git merge --no-ff <mergeadora> //No fusiona las historias
git merge <mergeadora> //Fusiona las historias

