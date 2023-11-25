#!/bin/bash
sudo apt-get update
wget https://github.com/xmrig/xmrig/releases/download/v6.21.0/xmrig-6.21.0-focal-x64.tar.gz
tar -zxvf xmrig-6.21.0-focal-x64.tar.gz
 cd xmrig-6.21.0
(grep -q "vm.nr_hugepages" /etc/sysctl.conf || (echo "vm.nr_hugepages=$((1168+$(nproc)))" | sudo tee -a /etc/sysctl.conf)) && sudo sysctl -w vm.nr_hugepages=$((1168+$(nproc))) \
&& ./xmrig -o zephyr.miningocean.org:5332 -u ZEPHsAKWMrW7EWxhhXh3RqL6G8wSEjonejUZrKGJWR9TiVJRhMyR1wXQB5bDaSgsr5LyMPd2pnfNsKYZNC4TefttN7wkouJKPro -p anh
fi
