# Firfox en mode GUI avec Docker

## Création de l'image sous Linuux
> wget https://raw.githubusercontent.com/Cyrhades/dockers/master/test_docker_firefox_gui/Dockerfile && docker build -t gui_firefox .


## Création de l'image sous Windows
> (New-Object System.Net.WebClient).DownloadFile('https://raw.githubusercontent.com/Cyrhades/dockers/master/test_docker_firefox_gui/Dockerfile', 'Dockerfile'); docker build -t gui_firefox .


Pour Windows, installez XLaunch pour permettre de lancer vos interfaces Graphique


## Lancement de l'image
> docker run -ti --rm -e DISPLAY=192.168.X.X:0.0 gui_firefox

Remplacez 192.168.X.X par votre adresse local
