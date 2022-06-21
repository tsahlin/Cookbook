# Ubuntu

See also [Bash](../bash/README.md)

### Page contents

 - [Show OS version](#show-os-version)
 - [Upgrade to a new release](#upgrade-to-a-new-release)

### Show OS version
```bash
lsb_release -a

cat /etc/os-release
```

### Upgrade to a new release
```bash
# Make sure all packages are up to date
sudo apt update
sudo apt upgrade
sudo apt autoremove

# Run upgrade
sudo apt dist-upgrade
sudo apt install update-manager-core
sudo do-release-upgrade -d

# In WSL, when asked to restart, answer Yes and then just close and reopen the terminal window
```