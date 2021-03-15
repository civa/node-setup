
```sudo apt-get install libboost-system-dev libboost-filesystem-dev libboost-program-options-dev libboost-chrono-dev libboost-test-dev libboost-thread-dev```
```sudo apt-get install build-essential libtool autotools-dev autoconf pkg-config libssl-dev libdb-dev libdb++-dev libevent-dev```


Clone Bitcoin Repo

```git clone https://github.com/bitcoin/bitcoin.git```
```cd bitcoin```

Checkout a preferred version

```git checkout v0.19.1```

Build 

```./autogen.sh```
```./configure --without-gui --with-incompatible-bdb```
```make -j6```


```cd src```
```sudo install -sv bitcoind bitcoin-cli /usr/local/bin```



```cd .bitcoin```
```nano bitcoin.conf```

rpcuser=bitcoin
rpcpassword=bitcoin
rpcport=8332
server=1
rpcallowip=0.0.0.0/0
rpcbind=127.0.0.1
rpcbind=ip

