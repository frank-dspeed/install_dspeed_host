# install_dspeed_host
Common Install for a fresh Host

export VERSION=v11.11.0
export DISTRO=linux-x64
mkdir -p ~/bin
wget https://nodejs.org/dist/$VERSION/node-$VERSION-$DISTRO.tar.xz
tar -xJvf node-$VERSION-$DISTRO.tar.xz
ln -s ~/node-$VERSION-$DISTRO/bin/node ~/bin/node
ln -s ~/node-$VERSION-$DISTRO/bin/npm ~/bin/npm
ln -s ~/node-$VERSION-$DISTRO/bin/npx ~/bin/npx



#sudo mkdir -p /usr/local/lib/nodejs
#sudo tar -xJvf node-$VERSION-$DISTRO.tar.xz -C /usr/local/lib/nodejs 
