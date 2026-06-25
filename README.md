# dlink-router-deployment-Configuration

# Project: Broadband Router Configuration & DHCP Setup

## Project Overview
This project demonstrates how to connect to a broadband router (D-Link), configure local area network (LAN) settings, expand the DHCP client IP pool, and secure the wireless network with WPA encryption. 

* **Author:** Muhammad Muhsin

---

## Configuration Steps

### Step 1: Connecting and Logging In
1. Connected a host PC to the router via Ethernet/Wi-Fi.
2. Accessed the gateway interface via browser using `http://192.168.1.1`.
3. Logged in using the management credentials[cite: 1].

![Login Screen](images/your-screenshot-1.png)

### Step 2: LAN & DHCP Pool Modification
* **Objective:** Expand the available IP address pool to allow more connected hosts.
* **Action:** Navigated to **Settings > LAN**[cite: 1]. Changed the default DHCP Client Range from `192.168.1.13 - 192.168.1.50` to a wider scope: `192.168.1.2 - 192.168.1.254`[cite: 1].
* **Work Mode:** Kept as **Server** so the router dynamically assigns IPs automatically[cite: 1].

![DHCP Config](images/your-screenshot-2.png)

### Step 3: Wireless Security (Wi-Fi Setup)
* **SSID:** Root AP-dlink-M921[cite: 1]
* **Encryption & Authentication:** Configured WPA-Mixed Personal mode (Pre-Shared Key) using TKIP/AES cipher suites to prevent unauthorized network access[cite: 1].

### Step 4: Verification and Testing
After clicking **Save & Apply** and waiting for the router to cycle[cite: 1], I connected a mobile phone to the newly secured wireless network. 
* **Result:** The device successfully pulled a dynamic IP address of `192.168.1.3` from the newly configured DHCP pool, verifying the configuration works perfectly[cite: 1].
