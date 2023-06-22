# oracle linux 9.1

python 3 is preinstalled(3.9.16)

## general

sudo apt update
sudo apt upgrade

## bashrc

```txt
# molecule
export VAGRANT_WSL_ENABLE_WINDOWS_ACCESS="1"
export PATH="$PATH:/mnt/c/Program Files/Oracle/VirtualBox/"
export PATH="$PATH:/mnt/c/Windows/System32"
export PATH="$PATH:/mnt/c/Windows/system32/WindowsPowerShell/v1.0"
```

source ~/.bashrc

## hashicorp

wget -O- https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
sudo apt update && sudo apt install vagrant

# pin vagrant to set version

## apt

sudo apt install python3-pip
sudo apt install python3-venv


## pip

pip3 install pip-tools

ansible
molecule
molecule-vagrant




# venv

python3 -m venv my_env
source my_env/bin/activate


## dev stuff

sudo yum install python3-devel
sudo yum install libffi-devel
sudo yum install libssl-devel
sudo yum install gcc gcc-c++ kernel-devel make