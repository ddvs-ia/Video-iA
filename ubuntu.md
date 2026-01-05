# Yolo v12 on Ubuntu

# python
ouvrir un terminal
## installation
### python3
```bash
sudo apt install python3 python3-pip python3-venv
python3 -v
pip3 --version

python3 -m venv venv
source venv/bin/activate
```
### pytorch
CUDA 12.8
```bash
pip3 install torch torchvision
sudo apt install graphicsmagick-imagemagick-compat
```
### ultralitics
```bash
pip install -U ultralytics
```
