# How to Connect sbRIO to the Internet via Laptop Wi-Fi

Steps to share your laptop's internet connection with an NI sbRIO device.

---

## 1. Open Network Settings
- Open **Control Panel**.
- Go to **Network and Sharing Center**.
- Click **Change adapter settings**.

![Insert screenshot of Network and Sharing Center here](image-link-1)

---

## 2. Configure Ethernet Adapter
- Right-click on **Ethernet** and select **Properties**.
- Select **Internet Protocol Version 4 (TCP/IPv4)** and click **Properties**.
- Choose the appropriate IP settings.

![Insert screenshot of Ethernet properties and IPv4 settings here](image-link-2)

---

## 3. Enable Internet Sharing
- Right-click your **Wi-Fi** adapter and select **Properties**.
- Go to the **Sharing** tab.
- Enable **Internet Connection Sharing** and select the Ethernet adapter.

![Insert screenshot of Sharing tab here](image-link-3)

---

## 4. Connect sbRIO
- Turn on the **sbRIO** and connect it to your laptop via LAN cable.
- Open **NI MAX** to check the connection:
  - If **Gateway** and **DNS** fields are filled, the sbRIO is connected to the internet.
  - If they show `0.0.0.0`, disable and re-enable Internet Connection Sharing, then reconnect the LAN cable.

![Insert screenshot of NI MAX showing connected sbRIO here](image-link-4)

---

**Notes:**  
- Ensure you have administrative rights on the laptop to modify network settings.  
- This method shares your laptop’s Wi-Fi connection over Ethernet to the sbRIO.
