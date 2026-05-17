## Introduction and Overview of DIY Wi-Fi Jammer Project  
<p align="center">
  <a href="https://youtu.be/URr2WkQa1V4?si=r3an5kJ09Gu4hK6e" target="_blank">
    <img 
      src="https://private-user-images.githubusercontent.com/142152441/593657931-71f0ab0b-07cd-4868-ba1d-2ec92d92b51e.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3Nzg5OTYyNzUsIm5iZiI6MTc3ODk5NTk3NSwicGF0aCI6Ii8xNDIxNTI0NDEvNTkzNjU3OTMxLTcxZjBhYjBiLTA3Y2QtNDg2OC1iYTFkLTJlYzkyZDkyYjUxZS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjYwNTE3JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI2MDUxN1QwNTMyNTVaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1mYTRmNWMwNDRiNzE3ZTRkZjNkYjZhYjJmYzkxYjFlZjJmYWRjZGFmMWMwNDQ2NjEzYThkMzdmYjFhOTg2OTNkJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZyZXNwb25zZS1jb250ZW50LXR5cGU9aW1hZ2UlMkZwbmcifQ.unulw8B8FNQX68sGhAfK3KLeXQPZU3JjkotGo0_mOfE"
      alt="Watch Video"
      width="700"
    />
  </a>
</p>

- The video introduces a **DIY Wi-Fi Jammer** built using the **NodeMCU ESP8266 board**.  
- The device functions as a **deauthentication (deauth) tool** to penetrate wireless networks by disconnecting clients.  
- A disclaimer is provided emphasizing the need for specific files to be installed on the ESP8266 board before use.  
- The ESP8266 connects to a PC via a **micro USB cable** for flashing the necessary firmware files.  
- The process involves downloading a zip file (provided via a link in the video description), extracting it, and locating two key files:  
  - A **.bin firmware file** to be flashed on the board.  
  - Another zip file containing the flashing tool for Windows.

  
**Flashing the ESP8266 Board with Firmware**  

- The flashing procedure uses the **ESP8266 Flasher tool** for Windows.  
- After opening the flasher:  
  - Navigate to the **config section** to select the downloaded **.bin file**.  
  - Access **Advanced options** to set the **board rate** (baud rate) — *specific value not provided*.  
  - In the **operation section**, select the appropriate **COM port** connected to the ESP8266.  
  - Click **Flash** to initiate the firmware upload process.
- The flashing duration is approximately **5 minutes**, requiring patience.

  
**Post-Flashing Setup and Initial Device Activation**  

- After flashing completes, the board is unplugged and plugged back in to restart.  
- The next step involves connecting to the ESP8266's own Wi-Fi access point from a PC or mobile device.  
- Once connected, users must open a browser and navigate to the local IP:  
  $$
  \text{http://192.168.4.1}
  $$
- A **warning page** is displayed, advising users to read carefully before proceeding; users must acknowledge by clicking "I understand".  
- This page serves as the control interface for the Wi-Fi penetration process.

  
**Scanning and Selecting Target Wi-Fi Networks**  

- The interface allows users to **scan for wireless networks** in the vicinity.  
- The video shows the scan result, with the presenter’s **home Wi-Fi network** appearing as the first option.  
- The presenter emphasizes the ethical aspect: **do not use this tool for harm or unauthorized access**.  
- The same Wi-Fi network is connected to a secondary phone, demonstrating multiple devices on the network.

  
**Deauthentication Attack on Connected Devices**  

- Users navigate to the **station section** of the interface to manage connected clients.  
- Clicking the **start button** initiates the **deauthentication attack** against selected connected devices.  
- The ESP8266 disconnects devices from the targeted Wi-Fi network, demonstrated by the secondary phone losing connectivity.  
- During scanning phases, users may need to reconnect to the ESP8266 Wi-Fi network to continue managing the attack.  
- Reloading the control page updates the list of connected clients, showing devices currently connected to the target network.

  
**Attack Modes and Results of Deauthentication**  

- Three different attack modes are available; the presenter selects **authentication attack mode** for demonstration.  
- The attack causes the targeted device (secondary phone) to disconnect and prevents reconnection to the original Wi-Fi.  
- The primary device used to control the ESP8266 also needs to reconnect to its Wi-Fi after attacks due to temporary disconnections.  
- Stopping the attack allows disconnected devices to successfully reconnect to the network.

  
**Clone Mode and Flooding of Fake Wi-Fi Networks**  

- Besides deauthentication, the device supports a **clone mode** that **clones the targeted Wi-Fi network’s SSID**.  
- This mode floods the airwaves with multiple **fake Wi-Fi networks** broadcasting the same or similar SSIDs, causing confusion and potential denial of service.  
- The presenter shows that many clone networks appear on a PC scan, all broadcast by the ESP8266 jammer.  
- There is also a **random mode** to flood random Wi-Fi IDs, enhancing the jamming effect.  
- Users can manually set the SSID for cloning, allowing custom fake networks to be broadcasted.

  
**Conclusion and Call to Action**  

- The video ends by thanking viewers and encouraging them to follow for more content related to hacking and DIY projects.  
- The presenter reiterates the ethical use of these tools, warning against misuse.

---

### Summary of Key Components and Actions


| Step                    | Description                                                                     | Notes                                |
| ----------------------- | ------------------------------------------------------------------------------- | ------------------------------------ |
| Download firmware files | Obtain `.bin` firmware and ESP8266 flasher tool from provided link              | Files provided via video description |
| Flash ESP8266           | Use ESP8266 Flasher on Windows to upload firmware to NodeMCU board              | Takes ~5 minutes                     |
| Connect to ESP8266 AP   | Connect PC/mobile to ESP8266 Wi-Fi; navigate to `http://192.168.4.1`            | Interface for attacks                |
| Scan Wi-Fi networks     | Scan surroundings for available Wi-Fi SSIDs                                     | Identify target network              |
| Select client devices   | View and select connected devices to attack                                     | List updated after scan              |
| Launch deauth attack    | Choose attack mode (authentication, others); start attack to disconnect clients | Devices lose Wi-Fi                   |
| Clone mode              | Broadcast cloned SSIDs to flood network space                                   | Causes fake Wi-Fi networks           |
| Random mode             | Flood random Wi-Fi IDs                                                          | Increases jamming effect             |


---

### Key Insights

- The **NodeMCU ESP8266** can be repurposed as a lightweight **Wi-Fi jammer and penetration testing tool** via firmware flashing.  
- The process requires **flashing a custom `.bin` firmware** and then controlling the device through a dedicated **web interface at 192.168.4.1**.  
- The jammer supports multiple attack modes:  
  - **Authentication attack** to disconnect devices forcibly.  
  - **Clone mode** to broadcast fake SSIDs flooding the wireless spectrum.  
  - **Random mode** to generate random Wi-Fi IDs for broader interference.
- The tool is useful for **penetration testing and educational purposes**, but ethical considerations and legal compliance are strongly emphasized.  
- The jamming effects are **temporary and reversible** by stopping the attack, allowing devices to reconnect normally.

---
# 🛒 Components Purchase Links

| Component | Description | Buy Link |
|------------|-------------|-----------|
| ESP32 | WiFi + Bluetooth Microcontroller Development Board | [Buy Now](https://amzn.to/4dhowbO) |
| NRF24L01 | 2.4GHz Wireless Transceiver Module | [Buy Now](https://amzn.to/4nzxSTT) |
| 0.96-inch OLED Display Module | 4-Pin I2C OLED Display Screen | [Buy Now](https://amzn.to/4nxZj0d) |

---

## 📦 Components Used in This Project

- ESP32 Development Board  
- NRF24L01 Wireless Communication Module  
- 0.96-inch OLED I2C Display  

---

## 🔗 Quick Access Links

- ESP32 → https://amzn.to/4dhowbO  
- NRF24L01 → https://amzn.to/4nzxSTT  
- OLED Display → https://amzn.to/4nxZj0d  
### Ethical Disclaimer

- The video stresses **not to use this device to harm or disrupt unauthorized networks**.  
- It is designed for **educational and penetration testing purposes only**.

---
