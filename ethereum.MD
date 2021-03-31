`sudo add-apt-repository -y ppa:ethereum/ethereum;sudo apt-get update;sudo apt-get install ethereum`


`nano /lib/systemd/system/geth.service`

[Unit]
Description=Geth Node
After=network-online.target
Wants=network-online.target
[Service]
WorkingDirectory=/root
User=root
ExecStart=/usr/bin/geth --syncmode full --rpc --rpcaddr 0.0.0.0 --rpcapi eth,web3,personal,debug --allow-insecure-unlock --cache=2048
Restart=always
RestartSec=5s
[Install]
WantedBy=multi-user.target

`service geth start`
