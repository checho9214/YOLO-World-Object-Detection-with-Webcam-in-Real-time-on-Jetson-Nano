# YOLO-World-Object-Detection-with-Webcam-in-Real-time

sudo apt update

sudo apt upgrade

sudo apt install -y build-essential libssl-dev zlib1g-dev libncurses5-dev libncursesw5-dev libreadline-dev libsqlite3-dev libgdbm-dev libdb5.3-dev libbz2-dev libexpat1-dev liblzma-dev libffi-dev libc6-dev

wget https://www.python.org/ftp/python/3.8.12/Python-3.9.19.tar.xz

tar -xf Python-3.9.19.tar.xz
cd Python-3.9.19

./configure --enable-optimizations --with-ssl

make -j4  # Utiliza el número apropiado de núcleos de CPU para acelerar la compilación
sudo make altinstall

python3.8 --version

python3.8 -c "import ssl; print(ssl.OPENSSL_VERSION)" 

pip install inference
pip install opencv-python
pip install supervision
pip install inference[yolo-world]
python3 app.py

![image](https://github.com/user-attachments/assets/3fe28b50-512c-442a-bbe0-6ce81516b0fc)

