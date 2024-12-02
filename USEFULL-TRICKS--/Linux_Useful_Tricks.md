# 🐧 Linux Useful Tricks

A curated list of useful tricks and shortcuts to enhance your productivity on Linux.

---

## 1. ⌨️ Keyboard Shortcuts

### 🔹 Basic Navigation
- **🖥️ Super + D**: Show desktop.
- **📋 Ctrl + C / Ctrl + V**: Copy / Paste.
- **🔄 Alt + Tab**: Switch between open windows.
- **🔧 Ctrl + Alt + T**: Open the terminal.
- **🗑️ Super + L**: Lock your screen.

### 🔹 Advanced Productivity
- **⬆️ Ctrl + Alt + Arrow (Up/Down/Left/Right)**: Switch between workspaces (desktops).
- **🖱️ Alt + F2**: Open the "Run" command window.
- **🔎 Ctrl + Shift + T**: Open a new terminal tab.
- **🖥️ Ctrl + Alt + Backspace**: Restart the X server (forces a logout in some distributions).
- **🧳 Alt + F4**: Close the current application/window.

---

## 2. 📁 File Manager Tips

### 🔹 Quick Navigation
- **📂 Ctrl + N**: Open a new file manager window.
- **🔄 Alt + Up Arrow**: Go up one directory.
- **🔍 Ctrl + F**: Open search in the file manager.
- **🔒 Ctrl + Shift + N**: Create a new folder.

### 🔹 Hidden Files
- **🔎 Ctrl + H**: Toggle the visibility of hidden files (files starting with a dot `.`).
  
---

## 3. 🖥️ Terminal Commands

### 🔹 Essential Commands
- `📄 ls`: List files and directories.
- `🗂️ cd <directory>`: Change directory.
- `📋 cp <source> <destination>`: Copy files.
- `🗑️ rm <file>`: Remove a file.
- `🛠️ sudo apt update`: Update package repositories (Debian/Ubuntu).
- `🔧 sudo apt upgrade`: Upgrade installed packages (Debian/Ubuntu).

### 🔹 File Permissions
- `📝 chmod +x <file>`: Make a file executable.
- `🔒 chmod 777 <file>`: Give full permissions (read/write/execute) to all users.
- `🔐 chown <user>:<group> <file>`: Change file ownership.

---

## 4. ⚙️ System Monitoring

### 🔹 Check System Resource Usage
- `💡 top`: Display running processes and resource usage.
- `📊 htop`: An enhanced version of `top` with a more user-friendly interface (install with `sudo apt install htop`).
- `⚡ free -h`: Display memory usage.
- `🔋 df -h`: Display disk usage.
- `💻 uname -a`: Get detailed system information.

### 🔹 Monitor Network
- `🌐 ifconfig`: Display network interface information.
- `🌍 ping <hostname>`: Test network connectivity to a specific host.
- `🚀 netstat -tuln`: Display network connections.

---

## 5. 🛠️ Package Management

### 🔹 Install and Update Packages (Debian/Ubuntu)
- `🛠️ sudo apt install <package>`: Install a new package.
- `🔄 sudo apt update`: Update package lists.
- `🔧 sudo apt upgrade`: Upgrade all installed packages.
- `❌ sudo apt remove <package>`: Uninstall a package.

### 🔹 Install and Update Packages (RedHat/CentOS)
- `🛠️ sudo yum install <package>`: Install a new package.
- `🔄 sudo yum update`: Update all packages.

---

## 6. 🖥️ Customization Tips

### 🔹 Change the Terminal Prompt
- To change your terminal prompt, edit the `.bashrc` file:
  - `nano ~/.bashrc`
  - Add `PS1="YourCustomPromptHere"` to the file and save.
  - Run `source ~/.bashrc` to apply the changes.

### 🔹 Install GNOME Tweaks
- **For GNOME Desktop**: Use `sudo apt install gnome-tweaks` to install GNOME Tweaks for advanced customization.
  
### 🔹 Change Desktop Environment
- **Install a new desktop environment**: `sudo apt install <desktop-environment-package>` (e.g., `sudo apt install xfce4` for XFCE).
  
---

## 7. 🧰 Useful Tools for Linux

- **📋 Clipboard Manager**: Install `clipman` or `copyq` for enhanced clipboard management.
- **🖼️ GIMP**: Image editing tool for Linux. Install with `sudo apt install gimp`.
- **⚙️ GNOME Tweaks**: For deeper GNOME customization. Install with `sudo apt install gnome-tweaks`.
- **🚀 Tmux**: Terminal multiplexer to manage multiple terminal sessions. Install with `sudo apt install tmux`.
- **🐧 WINE**: Run Windows apps on Linux. Install with `sudo apt install wine`.

---

## 8. 🛠️ System Security

### 🔹 Firewall Management (UFW)
- **🔒 sudo ufw enable**: Enable the firewall.
- **🛡️ sudo ufw status**: Check firewall status.
- **🔑 sudo ufw allow <port>/tcp**: Allow a specific port through the firewall.

### 🔹 User Management
- **👥 sudo adduser <username>**: Add a new user.
- **🧑‍💻 sudo deluser <username>**: Delete a user.

---

## 9. 🔗 Useful Links

- [📚 Official Ubuntu Documentation](https://help.ubuntu.com/)
- [🐧 Linux Command Cheat Sheet](https://www.cheatography.com/davechild/cheat-sheets/linux-command-line/)
- [🚀 Tmux GitHub Repository](https://github.com/tmux/tmux)
- [🛠️ Linux Security Tools](https://www.cyberciti.biz/tips/linux-security-tools.html)

---

Feel free to contribute by creating a pull request!
