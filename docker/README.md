# Docker

### Install on Ubuntu in WSL
```bash
# Switch to iptables-legacy
sudo update-alternatives --config iptables

# Add apt source
. /etc/os-release
curl -fsSL https://download.docker.com/linux/${ID}/gpg | sudo tee /etc/apt/trusted.gpg.d/docker.asc
echo "deb [arch=amd64] https://download.docker.com/linux/${ID} ${VERSION_CODENAME} stable" | sudo tee /etc/apt/sources.list.d/docker.list
sudo apt update

# Install Docker
sudo apt install docker-ce docker-ce-cli containerd.io

# Start dockerd
nohup sudo -b dockerd </dev/null >/mnt/c/docker/dockerd.log 2>&1
```
