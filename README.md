# Anti-DDoS Protection System for Growtopia Private Server (GTPS)

![License](https://img.shields.io/badge/license-MIT-blue)  
![Platform](https://img.shields.io/badge/platform-Windows-blue)  
![Language](https://img.shields.io/badge/language-C%2B%2B-blue)  

Anti-DDoS Protection System for Growtopia Private Server (GTPS) is a C++-based application designed to detect and mitigate Distributed Denial-of-Service (DDoS) attacks targeting Growtopia private servers. This system includes an **auto block IP** feature to automatically block malicious IPs and protect your GTPS from downtime.

---

## ⚙️ Features

- **DDoS Attack Detection:** Identifies suspicious traffic patterns in real-time on your GTPS.
- **Automatic Mitigation:** Automatically blocks IPs detected as malicious, preventing attacks.
- **Traffic Analysis:** Monitors and analyzes packet volume and types on the server.
- **Log Activity:** Logs suspicious activities and IPs for further analysis and review.
- **Easy to Use:** No installation required; just download and run the executable file (.exe).
- **GTPS Support:** Specifically designed for Growtopia private servers (GTPS).
- **Run as Administrator:** Automatically requests administrator privileges to ensure proper functioning.  
  **Note:** The program requires administrator privileges to access network resources and block malicious traffic.

---

## 🚀 How to Use

### Prerequisites

- **Windows 10/11:** This program is designed to run on Windows.
- **Growtopia Private Server (GTPS):** Ensure that your GTPS instance is running before using this tool.
- **Administrator Privileges:** Admin rights are required to run the application if network access is needed.

### Run the Program

1. **Download the Executable:**  
   Download the `.exe` file from the [Release Page](https://github.com/RenzyAmstrg/AntiDoS/releases/tag/release).

2. **Run the Program as Administrator:**  
   - Right-click on `anti_ddos.exe` and select **Run as administrator**.  
   - Alternatively, you can run it via Command Prompt with administrator privileges:
     ```cmd
     right-click and select "Run as administrator"
     anti_ddos.exe
     ```

   **Important:**  
   - When you run the program with administrator privileges, it will have the necessary access to monitor network traffic and block suspicious IP addresses. If prompted, click **Yes** to allow the program to run with administrator rights.
   - If you want to avoid being prompted each time, you can create a shortcut for `anti_ddos.exe`, then configure it to **Always Run as Administrator**:
     - Right-click on the `.exe` file and choose **Create Shortcut**.
     - Right-click on the shortcut, select **Properties**.
     - In the **Shortcut** tab, click **Advanced** and check the box for **Run as administrator**. This will make the program always run with the necessary privileges.

3. **Configure (Optional):**  
   Edit the `config.json` file to adjust system parameters such as detection thresholds, traffic limits, or IP block list.

4. **Activate Auto Block:**  
   The program will automatically detect suspicious traffic and block the associated IP addresses. Blocked IPs will be logged in the `activity.log` file.

---

## 📂 Project Structure
AntiDoS/ ├── anti_ddos.exe # Executable file ├── config/ │ ├── config.json # Configuration file for settings ├── logs/ │ ├── activity.log # Activity log with blocked IPs ├── README.md # Project documentation ├── app.manifest # Manifest file to request admin privileges
