herbsters Core integration/staging tree
=====================================

Stratum Mining Pool: http://herbsters.com or http://140.82.10.244

Block Explorer: http://herbsters.com:3001 or http://140.82.10.244:3001

Wallet: http://bitcoinhopper.com or http://144.202.9.181

What is herbsters?
----------------

herbsters is an experimental digital currency that enables instant payments to
anyone, anywhere in the world. herbsters uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. herbsters Core is the name of open source
software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of
the herbsters Core software, see [http://herbsters.com](http://herbsters.com).

License
-------

herbsters Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

Developer IRC can be found on irc.herbsters.com at #herbsters-dev.

Berkeley DB 4.8
---------------

wget http://download.oracle.com/berkeley-db/db-4.8.30.zip

sudo apt install unzip

unzip db-4.8.30.zip

cd db-4.8.30

cd build_unix/

../dist/configure --prefix=/usr/local --enable-cxx

sudo make

sudo make install

Testing Ubuntu 18.04 Linux
--------------------------

sudo apt-get install software-properties-common -y

sudo add-apt-repository ppa:bitcoin/bitcoin

sudo apt-get update

sudo apt-get upgrade -y

sudo apt-get install libdb4.8-dev libdb4.8++-dev

sudo apt-get install git build-essential libcurl4-openssl-dev libdb-dev libdb++-dev screen

sudo add-apt-repository universe

sudo apt-get update

sudo apt-get install libboost-all-dev php-memcached python-pylibmc memcached php-memcached php-mysqlnd php-curl php-json libapache2-mod-php node-jsonfile python-cjson libconfig-json-perl libjs-json libjson-simple-java libjson-xs-perl php-json python-cjson php7.2-json python-jsondiff python-simplejson libssl-dev ftpd phpunit autoconf libevent-dev automake build-essential libcurl4-openssl-dev libdb5.3-dev libdb5.3++-dev mysql-server memcached php-mysqlnd php-curl php-json php-curl libapache2-mod-php php-memcached libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils python3 libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev

.profile
--------

export PATH=$PATH:/home/USERNAME/herbsters/src

installation from github
------------------------

git clone https://github.com/herbsters/herbsters.git

./autogen.sh

./configure --with-incompatible-bdb

make

.herbsters/herbsters.conf
-------------------------

server=1

txindex=1

addnode=149.28.46.64:7994

addnode=45.77.144.188:7994

rpcuser=otherb_user_id

rpcpassword=THISWHERETHAT_PWD

rpcport=7993

port=7994

rpcbind=0.0.0.0

rpcallowip=0.0.0.0/0

rpcallowip=127.0.0.1

rpcallowip=149.28.46.64

rpcallowip=45.77.144.188

rpcallowip=140.82.10.244

daemon=1

gen=1

listen=1

paytxfee=0.001

4way=1

commands
--------

START: herbstersd -deprecatedrpc=accounts -daemon

DATA: herbsters-cli getinfo

COIN CREDIT: herbsters-cli getbalance

TARGET BLOCK: herbsters-cli getblocktemplate

WALLET ADDRESS: herbsters-cli getaccountaddress ""

SEND COINS: herbsters-cli sendtoaddress "address" amount

MOVE COINS: herbsters-cli move "#" "" amount

wallet
------

http://bitcoinhopper.com or http://144.202.9.181

Coming soon market, exchange, hopper
