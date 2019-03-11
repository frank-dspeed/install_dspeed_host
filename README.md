# install_dspeed_host
Common Install for a fresh Host



## NodeJS

```bash
export VERSION=v11.11.0
export DISTRO=linux-x64
mkdir -p ~/bin
wget https://nodejs.org/dist/$VERSION/node-$VERSION-$DISTRO.tar.xz
tar -xJvf node-$VERSION-$DISTRO.tar.xz
ln -s ~/node-$VERSION-$DISTRO/bin/node ~/bin/node
ln -s ~/node-$VERSION-$DISTRO/bin/npm ~/bin/npm
ln -s ~/node-$VERSION-$DISTRO/bin/npx ~/bin/npx
```

## Docker
```bash
sudo apt-get update
sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg-agent \
    software-properties-common\
    git
 curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
 sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io
```

