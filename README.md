Platinum - PT

windows binaries are in the binaries folder.
linux compile example ubuntu 32 bit

sudo apt-get update 

sudo apt-get upgrade

sudo apt-get install g++ libboost-all-dev qt4-qmake libqt4-dev build-essential libssl-dev libdb5.1++-dev git libqrencode-dev libqtgui4 libboost-all-dev libdb5.1-dev  libglib2.0-dev

mkdir gits

cd gits

git clone https://github.com/PlatinumTokenCrypto/Coin.git

cd Coin/src

mkdir obj

make -f makefile.unix "USE_UPNP=-"

at this point you have the platinumd compiled and sitting in your src folder,
you could run it 

strip platinumd 

./platinumd

nano ~/.platinum/platinum.conf

rpcuser=username

rpcpassword=passwordgoeshere

rpcport=10126

ctl-o , ctl-x

./platinumd

Or go onto make a gui wallet .

cd ..

qmake

make

if you get the error about libleveldb.a then 

cd leveldb

make -f Makefile libmemenv.a libleveldb.a

cd ..

make


launch Platinum-PT 

donate to the Platinum Developers

BTC:1BYPqPS8TUEC987FK2Rr29daYtRxZU63SQ

PT:PNQ2EyxdmUtJD3VDLpqsdEA5Wk1zEyTQwD
