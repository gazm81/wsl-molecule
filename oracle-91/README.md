# oracle linux 9.1

python 3 is preinstalled(3.9.16)

## general

sudo yum update
sudo yum upgrade

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

sudo yum install -y yum-utils
sudo yum-config-manager --add-repo https://rpm.releases.hashicorp.com/RHEL/hashicorp.repo
sudo yum -y install vagrant

## pip 

pip3 install pip-tools

## dev stuff

sudo yum install python3-devel
sudo yum install libffi-devel
sudo yum install libssl-devel
sudo yum install gcc gcc-c++ kernel-devel make