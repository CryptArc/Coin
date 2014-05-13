Platinum Coin - PT 

linux compile example ubuntu (may need missing deps this is not a complete guide,everyone has a different setup)

sudo apt-get update 

sudo apt-get upgrade

sudo apt-get install g++ libboost-all-dev qt4-qmake libqt4-dev build-essential libssl-dev libdb5.1++-dev git libqrencode-dev libqtgui4 libboost-all-dev libdb5.1-dev  libglib2.0-dev libminiupnpc-dev

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

rpcuser=usernamegoeshere

rpcpassword=passwordgoeshere

rpcport=10126


ctl-o , ctl-x

./platinumd

Or go onto make a gui wallet .

cd ..

qmake-qt4 platinum-qt.pro "USE_UPNP=-"

make -j2

if you get the error about libleveldb.a then 

cd src/leveldb

make -f Makefile libmemenv.a libleveldb.a

cd ..

cd ..

make -j2


launch Platinum-PT 

donate to the Platinum Developers

BTC:1BYPqPS8TUEC987FK2Rr29daYtRxZU63SQ

PT:PUwH4AhNFhwEHTmQRsj1tR9WKM35e8iYy4
