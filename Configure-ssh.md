
# SSH and VS Code Configuration Guide

## Table of Contents
- [Initial Setup](#initial-setup)
- [SSH Configuration](#ssh-configuration)
- [VS Code Setup](#vs-code-setup)
- [Terminal Commands Reference](#terminal-commands-reference)
- [Troubleshooting](#troubleshooting)

## Initial Setup

### Prerequisites
- macOS/Linux system
- VS Code installed
- Terminal access
- Administrative privileges

## SSH Configuration

### 1. Navigate to SSH Directory
```bash
cd ~/.ssh
```

### 2. Check Existing Files
```bash
ls
```
This will display any existing SSH configurations, including GitHub keys.

### 3. Create Configuration File
```bash
code config
```
This creates/opens the SSH config file in VS Code.

### 4. Basic Config File Structure
```
Host hostname
    HostName full.server.address
    User yourusername
    ForwardX11 yes
    ForwardX11Trusted yes
```

## VS Code Setup

### 1. Install VS Code Command Line Tools
1. Open VS Code
2. Press `Command + Shift + P`
3. Type "code"
4. Select "Shell Command: Install 'code' command in PATH"
5. Enter system password when prompted

### 2. Required Extensions
- Remote - SSH
- Other recommended extensions:
  - Rainbow Indent (for better code visualization)
  - Git integration tools
  - Language-specific extensions

### 3. Terminal Integration
After installing the command line tools, verify installation:
```bash
code --version
```

## Terminal Commands Reference

### Essential Commands
```bash
# Navigate to home directory
cd ~

# Navigate to SSH directory
cd ~/.ssh

# List directory contents (including hidden files)
ls -la

# View file contents
cat filename

# Source updated configuration
source ~/.zshrc
```

### File Management
```bash
# Create new directory
mkdir dirname

# Remove file
rm filename

# Remove directory
rm -r dirname
```

## Troubleshooting

### Common Issues

1. **Command 'code' not found**
   - Solution: Reinstall VS Code command line tools
   - Alternative: Restart terminal

2. **SSH Connection Failed**
   - Verify hostname and credentials
   - Check network connection
   - Ensure SSH service is running on remote server

3. **Configuration Not Loading**
   - Source your profile: `source ~/.zshrc`
   - Open new terminal window
   - Verify file permissions: `chmod 600 ~/.ssh/config`

### Best Practices

1. **Security**
   - Keep SSH keys private
   - Use specific hostnames
   - Regular backup of configuration files

2. **Organization**
   - Comment your config files
   - Use meaningful host names
   - Keep separate configurations for different environments

## Additional Resources

- [VS Code Documentation](https://code.visualstudio.com/docs)
- [OpenSSH Documentation](https://www.openssh.com/manual.html)
- [Terminal Commands Cheatsheet](https://github.com/0nn0/terminal-mac-cheatsheet)

---

*Note: Adjust configurations according to your specific needs and security requirements.*
