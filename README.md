# 🖥️ Bash Health Monitor Script

## 👩 Author
**Khushi Dogra**

---

## 📌 Overview
This project is a Bash-based health monitoring script designed to automatically check the status of system services, attempt recovery if they fail, and log all activities with timestamps.

It helps reduce manual intervention in managing services on a Linux system.

---

## ⚙️ Features

✨ Reads list of services from a file (`services.txt`)  
✨ Checks whether each service is running  
✨ Attempts automatic restart if a service is down  
✨ Logs all events with timestamp and severity (INFO, WARN, ERROR)  
✨ Displays a structured summary of results  
✨ Includes user and hostname for unique output  

---

## 📂 Project Structure
bash_assignment_1/
│── health_monitor.sh
│── services.txt
│── output.png
│── README.md


---

## 🧾 How It Works

1. The script reads service names from `services.txt`
2. It checks each service using system commands
3. If a service is down:
   - It attempts to restart it
   - Waits for a few seconds
   - Re-checks the status
4. Logs are generated in:
5. A summary is displayed at the end

---

## ▶️ How to Run

```bash
chmod +x health_monitor.sh
./health_monitor.sh


