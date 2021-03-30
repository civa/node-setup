
```sudo apt-get install libboost-system-dev libboost-filesystem-dev libboost-program-options-dev libboost-chrono-dev libboost-test-dev libboost-thread-dev;sudo apt-get install build-essential libtool autotools-dev autoconf pkg-config libssl-dev libdb-dev libdb++-dev libevent-dev```


Clone Bitcoin Repo

```git clone https://github.com/bitcoin/bitcoin.git;cd bitcoin;git checkout v0.19.1```

Build 

```./autogen.shz;./configure --without-gui --with-incompatible-bdb;make -j6```


```cd src;sudo install -sv bitcoind bitcoin-cli /usr/local/bin;cd```



```nano .bitcoin/bitcoin.conf```

rpcuser=username<br>
rpcpassword=password<br>
rpcport=8332<br>
server=1<br>
rpcallowip=0.0.0.0/0<br>
rpcbind=127.0.0.1<br>
rpcbind=ip<br>

