# Jenkins
Projet Jenkins 

lancer l'installation depuis Vagrant

```
vagrant up --provision
```
se connecter en ssh puis lancer jenkins dans docker dans laquelle on va récupérer le mdp jenkins
```
vagrant ssh
docker exec -it jenkins-jenkins-1 cat /var/jenkins_home/secrets/initialAdminPassword
```
vérification de la présence de l'image docker
![verification de la présence de l'image docker](images/jenkins-demo0.png)

une fois le "initialAdminPassword" collé, la connexion à Jenkins est possible et on peut configurer le premier utilisateur

![connexion](images/jenkins-demo1.png)

Bienvenue dans le tableau de bord !
![tableau de bord](images/jenkins-demo2.png)
