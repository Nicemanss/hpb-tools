# hpb-tools
Tools to make hpb-life easier

# Setting up

sudo su -

apt install git

git clone https://github.com/Nicemanss/hpb-tools

cd hpb-tools


# Installing

bash ./hpb-install

# Upgrading to a specific version (1.0.2.3 in this case)

bash ./hpb-upgrade 1.0.2.3

# Upgrading to the latest commit

bash ./hpb-upgrade

# Start / Stop / Restart the service
systemctl start ghpb@root.service
systemctl stop ghpb@root.service
systemctl restart ghpb@root.service

# Attach to the HPB console
/opt/ghpb-bin/ghpb attach http://127.0.0.1:8545


# View logs
journalctl -u ghpb@root.service
