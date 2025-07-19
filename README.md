# setup-mason-for-termux
A bash script to set up packages for Neovim Mason in Termux. This script solves 'failed to install lua_ls' in termux nvim and the 'current platform not supported' error when installing packages with Mason, specifically in Termux.

## How to Use

### Step 0: Ensure you have "which" installed on termux
```bash
pkg install which
```

### Step 1: Copy the script Directly to `/data/data/com.termux/files/usr/bin/install-in-mason`
Run the following command to copy the script directly into `/data/data/com.termux/files/usr/bin/install-in-mason`, making it immediately usable:

```bash
curl -o /data/data/com.termux/files/usr/bin/install-in-mason  https://raw.githubusercontent.com/Amirulmuuminin/setup-mason-for-termux/main/install-in-mason
```

### Step 2: Make the Script Executable
Set the executable permissions:

```bash
chmod +x /data/data/com.termux/files/usr/bin/install-in-mason
```

### Step 3: Run the Script
Now, you can use the script to install any package for Neovim Mason. For example:

```bash
install-in-mason lua-language-server
```

### Requirements
- Termux
- Neovim with Mason installed (Mason is automatically installed if you use LazyVim or any similar setup)
