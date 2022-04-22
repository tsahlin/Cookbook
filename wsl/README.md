# WSL - Windows Subsystem for Linux

### List installed distributions

```pwsh
wsl -l -v
```

### Upgrade a distribution from WSL 1 to WSL 2

```pwsh
wsl --set-version <Dist> 2
# Replace Dist with the distribution name:
wsl --set-version Ubuntu 2
```
