# Controlled ICMP Traffic Generation Lab Using Scapy

## 📌 Overview

This project demonstrates a controlled cybersecurity lab in which I used **Scapy** on a Kali Linux virtual machine to generate ICMP traffic toward an Ubuntu Linux virtual machine.

The experiment was conducted entirely within an isolated and controlled virtual environment for educational purposes. The objective was to gain practical experience with **network packets, ICMP communication, packet crafting, and network behaviour analysis**.

This lab is part of my ongoing journey to develop practical skills in **Cybersecurity, Linux, Networking, and Network Security**.

---

## 🎯 Objectives

The main objectives of this lab were to:

* Understand the basic behaviour of the **ICMP protocol**.
* Explore packet generation using **Scapy**.
* Understand how ICMP traffic travels between two virtual machines.
* Observe the response of a target system to generated ICMP traffic.
* Gain practical experience with **Kali Linux and Ubuntu Linux**.
* Improve my understanding of network communication and packet-level operations.
* Document cybersecurity experiments in a reproducible and professional manner.

---

## 🧪 Lab Environment

| Component           | Details                         |
| ------------------- | ------------------------------- |
| Attacker/Testing VM | Kali Linux                      |
| Target/Receiving VM | Ubuntu Linux                    |
| Tool                | Scapy                           |
| Protocol            | ICMP                            |
| Virtualisation      | Virtual Machine Environment     |
| Network             | Isolated/Controlled Lab Network |

---

## 🗺️ Lab Architecture

The basic lab setup consisted of two virtual machines communicating over a controlled virtual network:

```text
┌──────────────────────┐
│      Kali Linux      │
│                      │
│  Scapy               │
│  ICMP Traffic        │
│  Generation          │
└──────────┬───────────┘
           │
           │ ICMP Traffic
           ▼
┌──────────────────────┐
│      Ubuntu Linux    │
│                      │
│  Target/Receiving VM │
│  Traffic Observation │
└──────────────────────┘
```

---

## 🔬 Methodology

The lab was performed in the following stages:

1. Prepared two Linux virtual machines:

   * Kali Linux
   * Ubuntu Linux

2. Configured both virtual machines to communicate within a controlled virtual network.

3. Verified network connectivity between the two systems.

4. Used **Scapy** on the Kali Linux VM to generate ICMP traffic.

5. Observed the behaviour of the Ubuntu VM during the experiment.

6. Recorded the terminal sessions from both systems to document the practical demonstration.

7. Reviewed the results and analysed the network behaviour observed during the experiment.

---

## 🛠️ Technologies and Tools

* **Kali Linux**
* **Ubuntu Linux**
* **Scapy**
* **ICMP**
* **Virtual Machines**
* **Linux Networking**

---

## 📚 Key Concepts Learned

Through this experiment, I gained practical exposure to:

### ICMP

The **Internet Control Message Protocol (ICMP)** is a network-layer protocol commonly used for diagnostic and error-reporting purposes. Tools such as `ping` rely on ICMP Echo Request and Echo Reply messages to test network reachability.

### Scapy

**Scapy** is a Python-based packet manipulation framework that allows security researchers and network professionals to construct, send, capture, and analyse network packets.

### Packet-Level Networking

The experiment helped me better understand how network traffic can be generated and observed at the packet level rather than interacting only with high-level applications.

### Virtualised Security Labs

Using virtual machines provides a safe environment for learning and experimenting with networking and cybersecurity concepts without affecting external systems.

---

## 🎥 Demonstration

A screen recording was created during the experiment showing the activity on both the Kali Linux and Ubuntu Linux virtual machines.

The recording demonstrates the experiment in a controlled laboratory environment.

> **Note:** The demonstration is intended solely for educational and cybersecurity learning purposes.

---

## 📸 Evidence

Recording from the experiment can be found in the project repository.


---

## ⚠️ Ethical and Legal Disclaimer

This experiment was conducted exclusively in a **controlled, isolated, and authorised virtual laboratory environment**.

The techniques and tools demonstrated in this repository should only be used on systems that you own or have explicit permission to test.

This project is intended for:

* Cybersecurity education
* Network security learning
* Ethical security research
* Understanding network protocols
* Developing practical cybersecurity skills

Unauthorised testing or disruption of systems and networks is illegal and unethical.

---

## 🚀 Future Improvements

I plan to expand this lab by exploring:

* ICMP traffic analysis using Wireshark.
* Comparing normal ICMP traffic with abnormal traffic patterns.
* Studying network monitoring and detection techniques.
* Exploring how security tools identify unusual ICMP activity.
* Building a small network monitoring lab.
* Documenting additional packet-analysis experiments.

---

## 👨‍💻 Author

**Adnan Sadi**

BS Computer Science Student | Cybersecurity Enthusiast

This project is part of my ongoing cybersecurity learning journey, where I am developing practical experience in:

* Cybersecurity
* Linux
* Computer Networking
* Cloud Computing
* Network Security
* Security Research

---

## ⭐ Acknowledgement

This project was completed as part of my hands-on cybersecurity learning and practical experimentation in a controlled virtual environment.

If you find this project useful or interesting, feel free to explore the repository and follow my journey as I continue building practical cybersecurity projects.
