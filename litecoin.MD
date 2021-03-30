
```sudo apt-get install libboost-system-dev libboost-filesystem-dev libboost-program-options-dev libboost-chrono-dev libboost-test-dev libboost-thread-dev;sudo apt-get install build-essential libtool autotools-dev autoconf pkg-config libssl-dev libdb-dev libdb++-dev libevent-dev```


Clone Bitcoin Repo

```git clone https://github.com/litecoin-project/litecoin.git;cd litecoin```

Checkout a preferred version

```git checkout v0.16.3```

Build 

```./autogen.sh;./configure --without-gui --with-incompatible-bdb;make -j6```


```cd src;sudo install -sv litecoind litecoin-cli /usr/local/bin```



```cd .litecoin;nano litecoin.conf```

rpcuser=username<br>
rpcpassword=password<br>
rpcport=10332<br>
server=1<br>
rpcallowip=0.0.0.0/0<br>
rpcbind=127.0.0.1<br>
rpcbind=ip<br>

