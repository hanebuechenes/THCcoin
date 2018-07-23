THCCoin
========

Installation from source
------------------------

Recommended linux environment, Ubuntu.

Install dependencies:

    sudo apt-get install git build-essential libtool autotools-dev automake pkg-config libssl-dev \
        libevent-dev bsdmainutils libboost-all-dev libqrencode-dev qt4-qmake libqt4-dev \
        libprotobuf-dev protobuf-compiler software-properties-common
     
    sudo add-apt-repository ppa:bitcoin/bitcoin
    sudo apt-get update
    sudo apt-get install libdb4.8-dev libdb4.8++-dev

Get the source:

    git clone https://github.com/thccoin-project/thccoin.git

To compile `thccoind` under linux:

    cd thccoin/src/
    make -f makefile.unix USE_O3=1 USE_ASM=1 USE_LEVELDB=1

To compile `thccoin-qt` under linux

    cd thccoin
    qmake USE_O3=1 USE_ASM=1 USE_LEVELDB=1
    make

See docs/

RPC Port: 31543
Network Port: 31544
