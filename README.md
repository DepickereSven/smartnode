# SmartNode
### Bash installer for smartnode on Ubuntu 16.04 LTS x64
### ATTENTION: This installer is only suitable for a dedicated vps. The anti-ddos script in this installer will disable all ports including the http, https and dns ports. It will only leave the smartnode port open as well as a custom port for SSH.

#### This shell script comes with 3 cronjobs: 
1. Make sure the daemon is always running: *makerun.sh*
2. Make sure the daemon is never stuck: *checkdaemon.sh*
3. Make sure smartcash is always up-to-date: *upgrade.sh*

#### Login to your vps, donwload the install.sh file and then run it:
```
wget https://raw.githubusercontent.com/msg768/smartnode/master/install.sh
bash ./install.sh
```

#### On the client-side, add the following line to smartnode.conf:
```
node-alias vps-ip-address:9678	node-privatekey collateral-txid collateral-vout
```

#### Run the qt wallet, go to SmartNodes tab, choose your node and click "start alias" at the bottom.

#### You're good to go now. BEE $SMART! https://smartcash.cc
