# Node.js

### Install NVM on Ubuntu
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
nvm -v
nvm install node
nvm use node
node -v

# Show installed versions
nvm list

# Show remote versions
nvm ls-remote

# Remove system version
sudo apt remove nodejs
sudo apt autoremove
```
