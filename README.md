# port-status-monitoring-pox

# 🚀 Port Status Monitoring Tool (POX Controller)

## 📌 Problem Statement

To design and implement a Software Defined Networking (SDN) controller using POX that monitors switch port status changes (UP/DOWN) in real time.

---

## 🎯 Objective

* Detect port status changes
* Log events in controller
* Demonstrate using Mininet

---

## 🛠️ Requirements

* Ubuntu / WSL
* Python 3.x
* Mininet
* POX Controller

---

## ⚙️ Setup Instructions

### Step 1: Install dependencies

sudo apt update
sudo apt install mininet git -y

### Step 2: Clone POX

git clone https://github.com/noxrepo/pox
cd pox

### Step 3: Add controller file

nano port_monitor.py

Paste the code and save.

---

## ▶️ Execution Steps

### Terminal 1: Run Controller

python3 pox.py port_monitor

### Terminal 2: Run Mininet

sudo mn --topo single,3 --controller=remote

---

## 🧪 Testing

### Bring port DOWN

link s1 h1 down

Expected Output:
Port 1 is DOWN

### Bring port UP

link s1 h1 up

Expected Output:
Port 1 is UP

---

## 📸 Proof of Execution

Screenshots included:

* Controller running
* Port DOWN event
* Port UP event
* Flow table
* Ping results

---

## 📊 Results

* Successfully detected port status changes
* Real-time logging achieved

---

## 📚 References

* POX Controller Documentation
* Mininet Documentation
* SDN Concepts

---
