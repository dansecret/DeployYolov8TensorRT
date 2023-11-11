
# Manual Set Up YOLOv8 for NVIDIA Jetson



## Install ultralytics Package

Step 1 Acces terminal jetson device and install pip and upgrade

```bash
  sudo apt update
  sudo apt install -y python3-pip -y
  pip3 install --upgrade pip
```

Step 2. install ultralytics Package

```bash
  pip3 install ultralytics
```

Step 3. upgrade numpy version to lastest

```bash
   pip3 install numpy -U
```

Step4. REboot the device

```bash
  sudo reboot
```


## uninstall Torch and Torchvision


```bash
  pip3 uninstall toch torchvision
```

## install Torch and Torchvision
install torch according to your jetpack version in following format pip3

```bash
  wget <URL> -O <file_name>
  pip3 install <filename>
```
here we are running JP5.1.1 and therefore we choose Pytorch v2.0.0
example:

```bash
sudo apt-get install -y libopenblas-base libopenmpi-dev
wget https://nvidia.box.com/shared/static/i8pukc49h3lhak4kkn67tg9j4goqm0m7.whl -O torch-2.0.0+nv23.05-cp38-cp38-linux_aarch64.whl
pip3 install torch-2.0.0+nv23.05-cp38-cp38-linux_aarch64.whl
```

install torchvision 
```bash
sudo apt install -y libjpeg-dev zlib1g-dev
git clone https://github.com/pytorch/vision torchvision
cd torchvision
git checkout v0.15.2
python3 setup.py install --user
```


if you want a more detailed list version torch vision compatible , check [this link](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)


## Install ONNX


```bash
  pip3 install onnx
```
