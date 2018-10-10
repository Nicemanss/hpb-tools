# hpb-tools
Tools to make hpb-life easier

# Setting up

sudo su -

apt install git

git clone https://github.com/Nicemanss/hpb-tools

cd hpb-tools


# Installing

bash ./hpb-install


# Upgrading to the latest release

bash ./hpb-upgrade

# Start / Stop / Restart the service
systemctl start ghpb@root.service
systemctl stop ghpb@root.service
systemctl restart ghpb@root.service

# Attach to the HPB console
/opt/ghpb-bin/ghpb attach http://127.0.0.1:8545


# View logs
journalctl -u ghpb@root.service
