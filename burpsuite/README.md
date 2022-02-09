# Burpsuite en mode GUI avec Docker

## Création de l'image 
> docker build -t burpsuite https://raw.githubusercontent.com/Cyrhades/dockers/master/burpsuite/Dockerfile

Pour Windows, installez XLaunch pour permettre de lancer vos interfaces Graphique


## Lancement de l'image
> docker run -e DISPLAY=192.168.X.X:0.0 burpsuite

Remplacez 192.168.X.X par votre adresse local
