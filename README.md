# pfSense-Initial-Setup
This repository provides the initial setup instructions for pfSense after installation. It covers prerequisites and steps to access the pfSense UI for the first time.

---

## Prerequisites

Ensure you have the following prerequisites before proceeding with the setup:

1. **pfSense Server**  
   - pfSense should already be installed on a physical or virtual machine.
   - The pfSense server should have at least two network interfaces: one for the WAN and one for the LAN.

2. **LAN Connection**  
   - A host device (computer, laptop, etc.) connected to the LAN side of the pfSense server.
   - This device will be used to access the pfSense UI.

3. **IP Address Configuration**  
   - By default, pfSense assigns the LAN interface IP as **192.168.1.1**. Ensure your host device is on the same subnet (e.g., `192.168.1.x`).

4. **Web Browser**  
   - Any modern web browser (e.g., Chrome, Firefox, Edge) installed on the host device to access the web-based UI.

---

## Steps to Access the pfSense UI

1. **Connect to the LAN Network**  
   Ensure your host device is connected to the same LAN network as the pfSense server.

2. **Open a Web Browser**  
   Open a browser on the host device and type the following address in the URL bar:
   ```plaintext
   https://192.168.1.1
   ```
   - Note: If the LAN IP was changed during installation, use that IP instead.

3. **Bypass Security Warning (if any)**  
   - Since pfSense uses a self-signed certificate, your browser may display a security warning.
   - Select **Advanced** and proceed to the pfSense interface.

4. **Log in to the pfSense Dashboard**  
   - The default credentials are:
     - **Username**: `admin`
     - **Password**: `pfsense`
   - **Important**: Change the default password after logging in.

5. **Complete the Initial Setup Wizard**  
   - Upon first login, pfSense may guide you through an initial setup wizard.
   - Follow the prompts to configure basic settings such as timezone, hostname, and LAN/WAN interface settings.

---

## Additional Configuration (Optional)

After completing the initial setup, consider configuring additional pfSense features, such as:

- **Firewall Rules**: Set rules to allow or block traffic as per your network requirements.
- **DHCP Server**: Configure DHCP for dynamic IP allocation to devices on your LAN.
- **DNS and VPN**: Set up DNS or VPN services if needed.

---

## Troubleshooting

- **Cannot Access UI**: 
  - Verify the host device’s IP address is in the same subnet as the pfSense LAN interface.
  - Check network cables or VM network settings if using a virtualized setup.

- **Forgot Password**: If you forgot the pfSense admin password, access the pfSense server console and use the option to reset the password.

---
🎉 Congratulations! 🎉

You've successfully installed and configured your pfSense firewall! Setting up network security and management tools is a crucial step in securing your infrastructure, and you've taken a big step forward.

From here, you can explore the powerful features that pfSense offers, such as firewall rules, VPNs, traffic shaping, and much more. Remember to keep learning, experimenting, and optimizing your setup!

Welcome to the world of pfSense – your network just got a whole lot smarter! 🛡️✨
