# Para conectar un folder local a un repositorio en GitHub
Tenemos que generar una llave para la conexión remota desde nuestra máquina al repositorio Git:
<ul>
<li>
Ejecutar los siguientes pasos: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
</li>
<li>
Los comandos usuales de Git son:
</li>
…or create a new repository on the command line

echo "# ansible_advanced_JDG" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/jdcyrix/ansible_advanced_JDG.git
git push -u origin main

…or push an existing repository from the command line

git remote add origin https://github.com/jdcyrix/ansible_advanced_JDG.git
git branch -M main
git push -u origin main



Command line instructions
You can also upload existing files from your computer using the instructions below.
Git global setup
git config --global user.name "devops"
git config --global user.email "devops@example.com"
Create a new repository
git clone http://control.example.com:5050/devops/demo-project.git
cd demo-project
git switch -c main
touch README.md
git add README.md
git commit -m "add README"
git push -u origin main
Push an existing folder
cd existing_folder
git init --initial-branch=main
git remote add origin http://control.example.com:5050/devops/demo-project.git
git add .
git commit -m "Initial commit"
git push -u origin main
Push an existing Git repository
cd existing_repo
git remote rename origin old-origin
git remote add origin http://control.example.com:5050/devops/demo-project.git
git push -u origin --all
git push -u origin --tags

</ul>


# Para aprovisionar el ambiente
https://rhpds-redirect.opentlc.com/

# Buscar el Demo/Workshop
OCP4 Getting Started Workshop
