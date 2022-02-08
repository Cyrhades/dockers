# Firfox en mode GUI avec Docker

## Création de l'image
> wget https://github.com/Cyrhades/dockers/test_docker_firefox_gui/Dockerfile && docker build -t GUI_firefox .

## Lancement de l'image
> docker run -ti --rm -e DISPLAY=192.168.X.X:0.0 GUI_firefox

Pour Windows, installez XLaunch pour permettre de lancer vos interfaces Graphique