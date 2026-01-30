# Sommaire 
# ia vidéo python - yolo
### installation
 - [ubuntu](ubuntu.md)



# projets-video-ia
[python yolov11 ubuntu](python%20yolov11%20ubuntu.md)

# Ubuntu
## installer et config python3
```bash
mkdir python
sudo apt install python3.12
python3-pip
python3 -m venv venv
source venv/bin/activate
```
## installation des librairies
```python
#pour une GTX 1650 Q-max 4go (laptop)
pip install ultralytics, pytorch, torch, torchvision --index-url https://download.pytorch.org/whl/cu130
```
### test si CUDA et le GPU est activé avec pytorch
si GPU nvidia, utlisé CUDA, 
si GPU AMD, utilisé 
en bash : 
```bash
nvidia-smi
```
en python : 
```python
nano test_pytorch_cuda.py


import torch
print("torch.CUDA disponible ?", torch.cuda.is_available())

python3 test_pytorch_cuda.py
```

## création de l'environnement yolo
```bash
mkdir yolov12
cd yolov12
mkdir 1_train
mkdir 2_valider
mkdir 3_predire
mkdir 4_export
mkdir 5_benchmark
mkdir 6_livestream

```
