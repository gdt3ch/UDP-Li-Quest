
![UDP Li-Quest Banner](https://raw.githubusercontent.com/gdt3ch/udp-li-quest/main/banner.png)

# UDP Li-Quest <sup>`v1.0`</sup>

**UDP Li-Quest** is a powerful and easy-to-use installer and manager for the Hysteria-based UDP server. This project is designed to simplify the setup and administration of a secure and high-performance UDP tunnel, ideal for gaming, streaming, and other latency-sensitive applications.

## ✨ Features

-   **🚀 Automated Installer:** A single command to set up the entire server environment.
-   **📊 User Management:** An interactive menu-driven manager for adding, editing, and removing users.
-   **⚙️ Dynamic Configuration:** Real-time updates to the server configuration without manual file editing.
-   **🔒 Secure:** Generates self-signed SSL certificates for encrypted communication.
-   **⚡ High Performance:** Built on Hysteria, a feature-rich proxy and relay tool optimized for lossy and unstable networks.
-   **🎨 Modern Interface:** A visually appealing and user-friendly command-line interface with loaders and progress indicators.

## 📦 Installation

To install UDP Li-Quest on your Debian-based server (e.g., Ubuntu), simply run the following command:

```bash
bash <(curl -s -H "Cache-Control: no-cache" https://raw.githubusercontent.com/gdt3ch/udp-li-quest/main/installer.sh)
```

The installer will automatically handle the following:
1.  **Dependency Checks:** Ensures all required packages (`curl`, `sqlite3`, `jq`, `figlet`, `lolcat`) are installed.
2.  **Hysteria Binary:** Downloads and installs the latest Hysteria binary.
3.  **Configuration:** Creates the necessary configuration files.
4.  **User Database:** Sets up a SQLite database for user management.
5.  **SSL Certificates:** Generates self-signed certificates for secure connections.
6.  **Systemd Service:** Configures and enables the `hysteria-server` service.
7.  **Firewall Rules:** Sets up `iptables` rules for traffic forwarding.
8.  **Manager Script:** Installs the `udpli` command for easy server management.

## 🛠️ Usage

Once the installation is complete, you can manage your server using the `udpli` command:

```bash
udpli
```

This will open the UDP Li-Quest Manager, an interactive menu where you can perform the following actions:

-   **Add, Edit, or Delete Users:** Easily manage user credentials.
-   **View Users:** List all current users.
-   **Modify Server Settings:** Change the domain, obfuscation string, and speed limits.
-   **Restart Server:** Apply changes by restarting the Hysteria service.
-   **Uninstall Server:** Completely remove the UDP Li-Quest server and all its components.

> Thank you