#!/bin/bash
wget https://github.com/xmrig/xmrig/releases/download/v6.21.0/xmrig-6.21.0-focal-x64.tar.gz
tar -zxvf xmrig-6.21.0-focal-x64.tar.gz
 cd xmrig-6.21.0
screen -R
./xmrig -o zephyr.miningocean.org:5332 -a rx -k -u ZEPHsAKWMrW7EWxhhXh3RqL6G8wSEjonejUZrKGJWR9TiVJRhMyR1wXQB5bDaSgsr5LyMPd2pnfNsKYZNC4TefttN7wkouJKPro -p anh
fi
