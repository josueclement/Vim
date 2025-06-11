## WSL (Windows Subsystem for Linux)

- Open `Turn Windows features on or off`
- Check `Windows Subsystem for Linux`
- Restart
- In command prompt: `wsl --install -d Ubuntu`

If the error (Error code: Wsl/InstallDistro/Service/RegisterDistro/CreateVm/HCS/HCS_E_SERVICE_NOT_AVAILABLE) appears, enable virtualization in BIOS

To remove green highlighted color, edit `~/.bashrc` and add at the end of the file:

```Bash
LS_COLORS=$LS_COLORS:'ow=1;34:' ; export LS_COLORS`
```

## Neovim

### Installation

Ubuntu: 

```Bash
sudo add-apt-repository ppa:neovim-ppa/unstable
sudo apt install gcc
sudo apt install clang
sudo apt install neovim
```

Windows: [Nightly release](https://github.com/neovim/neovim/releases/nightly), [Stable release](https://github.com/neovim/neovim/releases/latest)

### Configuration

[init.lua](init.lua) is the Neovim configuration file

Windows path: `%LocalAppData%\nvim\`

Linux path: '~/.config/nvim'
