# OneLineXNMMiningScript

This is a 'ONE LINE' script, just 

* Copy **all of them** and paste it into your linux terminal/console.
* Replace the **'YOUR_OWN_WALLET_ADDRESS'**.
* **'Enter'** to start mining $XNM.
* **Ctrl-a d** to detach from screen.

Easy.

Default DevFee is 1. (0.1% Donate to https://github.com/woodysoil/XenblocksMiner/)

```
sudo apt install screen && \
screen -dmS miner && \
screen -x miner -X stuff $'wget https://github.com/woodysoil/XenblocksMiner/releases/download/v1.4.0/xenblocksMiner-1.4.0-Linux.tar.gz && \
tar -zxvf xenblocksMiner-1.4.0-Linux.tar.gz && \
chmod +x xenblocksMiner && \
./xenblocksMiner --minerAddr YOUR_OWN_WALLET_ADDRESS --totalDevFee 1\n' && \
screen -x miner
```

List running sessions / screens

```
screen -ls
```

Check mining progress

```
screen -x miner
```

Inside screen and detach from screen (not kill mining program)

```
Ctrl-a d
```

Inside screen and kill mining program

```
Ctrl-c
```

Outside screen and kill mining program

```
screen -XS miner kill
```

