## 概要

curl -sL https://deb.nodesource.com/setup_22.x | sudo -E bash -
sudo apt install nodejs -y
sudo apt install jq -y
git clone https://github.com/mud-chain/mud-deploy.git && cd mud-deploy && npm i
修改config.json指定安装目录
node common-node.js --start=false
修改moniker

sudo ufw allow from 152.53.82.141 to any port 22 proto tcp && sudo ufw allow 80/tcp && sudo ufw allow 443/tcp && sudo ufw allow 26656/tcp && sudo ufw allow from 152.53.81.88 to any port 26657 proto tcp && sudo ufw allow from 152.53.81.88 to any port 45876 proto tcp && echo 'y' | sudo ufw enable && sudo ufw status numbered

sudo npm i pm2 -g && mkdir beszel && cd beszel && curl -sL "https://github.com/henrygd/beszel/releases/latest/download/beszel-agent_$(uname -s)_$(uname -m | sed -e 's/x86_64/amd64/' -e 's/armv6l/arm/' -e 's/armv7l/arm/' -e 's/aarch64/arm64/').tar.gz" | tar -xz -O beszel-agent | tee ./beszel-agent >/dev/null && chmod +x beszel-agent && pm2 start ./beszel-agent --name "beszel-agent" -- -listen 45876 -key "ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIPSo54+IX59Iszo1L3ljv+Sv99J3aOQZTU6+S1TpvS/z"

