Platinum BitCoin - PT 

links on PlatinumCrypto.COM

linux compile example ubuntu (may need missing deps this is not a complete guide,everyone has a different setup)

sudo apt-get update 

sudo apt-get upgrade

sudo apt-get install g++  qt4-qmake libqt4-dev build-essential libssl-dev libdb5.1++-dev git libqrencode-dev libqtgui4 libboost-all-dev libdb5.1-dev  libglib2.0-dev libminiupnpc-dev libboost1.53-all-dev 

mkdir gits

cd gits

git clone https://github.com/CryptArc/Coin.git

cd Coin

qmake platinum-qt.pro 

make


nano ~/.platinum/platinum.conf

rpcuser=usernamegoeshere
rpcpassword=passwordgoeshere
rpcport=10126
server=1
listen=1
daemon=1

ctl-o , ctl-x
run Platinum , goto Platinumcrypto.com and explore!
Welcome to the community !!
