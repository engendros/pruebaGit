# Guia de GIT:

## Credenciales:
(https://docs.github.com/es/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
ssh-keygen -t ed25519 -C "your_email@example.com"
Vamos a git y lo añadimos en el repositorio
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/<cert_name>




