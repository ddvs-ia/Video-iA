# Video-iA
solution de tracking par Intelligence Artificielle

## Installation Windows
### Installation Python3
donwload python 3
créer le dossier du prjet
ouvrir un CMD dans le projet : 

créer l'environnement virtuel
```bash
py -m venv venv
py venv\Script\activate
```
Installation PyQt5 lxml
```bash
pip3 install PyQt5
pip3 install lxml
```

download projet github
unzip
```bash
cd labelImg-master
pyrcc5 -o libs/resources.py resources.qrc
```

run l'interface graphique
```bash
python labelImg.py
```
dans data/predefined_classes.txt -> list des objects
W -> créer une box




