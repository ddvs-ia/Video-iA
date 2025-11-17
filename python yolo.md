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




# trainning bois
## installation du projet
création des dosier
téléchargment des images

## label
lancé labellmg
box label les images
open dir > images
change save dir > labels

### importé les labels dans yolo
copier les labels (lablelmg/data/data
dnas YOLOv8_custom/classes.txt

## yolo ia installation
```bash
python l'envi virt YOLOv8_custom
pip3 install ultralytics
```

```bash
python
import torch
torch.__version__

exit()

install pytorch
```
 (cuda)
https://pytorch.org/get-started/locally/

```bash
pip3 install --upgrade torch torchvision --index-url https://download.pytorch.org/whl/cu130
python 
import torch
torch.cuda.is_available()
```
false -> nvidia GTX 1650 -> CUDA toolkit : https://developer.nvidia.com/cuda-downloads?target_os=Windows&target_arch=x86_64&target_version=10&target_type=exe_local

exit


### entrainement
```bash
yolo task=detect mode=train epochs=100 data=data_custom.yaml model=yolo11s.pt imgsz=640 batch=4
```
attendre 10 sec par epochs, ça a durée  7 min environ

## predict

le model ia entrainé est dans E:\DDVS IA\Solution IA\IA video\YOLOv8_custom\runs\detect\train12\weights\best.pt
copier le model best.pt à la racine
copier un fichier 1.jpg à la racine
```bash
yolo task=detect mode=predict model=best.pt show=True conf=0.6 source=1.jpg
```

