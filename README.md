# 👋 Hello, I'm Yong Jie

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yong-jie-tan/)
[![Portfolio](https://img.shields.io/badge/Portfolio-2563eb?style=for-the-badge&logo=google-chrome&logoColor=white)](https://yongjiee.github.io)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:tan_yong_jie@outlook.com)

</div>

## 🚀 Robotics Systems Engineer

> Specializing in autonomous navigation, computer vision, and embedded systems integration

🎓 **Robotics Systems Student** @ Singapore Institute of Technology (Class of 2028)
🏆 **WorldSkills Singapore Medalist** (2020, 2021) — Mechatronics
🇸🇬 Based in Singapore

---

<div align="center">

### 📊 Quick Stats

| 🎓 Graduation | 🏆 Competitions | 💻 Projects | 🔧 Tech Stack |
|:-------------:|:---------------:|:-----------:|:-------------:|
| 2028 | 2× WorldSkills | 5+ Active | ROS2 • Python • C++ |

</div>

---

## 💡 About Me

I'm a robotics engineer passionate about building intelligent autonomous systems that bridge software and hardware. With a competitive mechatronics background and hands-on project experience across ROS2, computer vision, and distributed embedded systems, I focus on creating solutions that work reliably in the real world — not just in simulation.

**What I bring:**
- **Autonomous Systems**: ROS1/ROS2 navigation, SLAM, path planning, multi-node distributed architectures
- **Computer Vision**: OCR pipelines, barcode detection, multi-camera fusion, OpenCV
- **Hardware Integration**: Raspberry Pi, STM32, Pixy2, Parallax Propeller microcontrollers
- **System Design**: From concept to deployment — sensor integration, data pipelines, real-time processing
- **Team Leadership**: Technical lead across multiple university engineering projects

---

## 🛠️ Technical Arsenal

### Core Technologies
```text
Robotics        ROS1 • ROS2 Humble • Nav2 • SLAM Toolbox • RTAB-Map • Gazebo
Vision          OpenCV • Tesseract OCR • pyzbar • Picamera2 • Multi-camera Fusion
Languages       C/C++ • Python • SPIN (Propeller) • Ladder Logic
Hardware        Raspberry Pi 4 • STM32 • Pixy2 • Parallax Propeller • TurtleBot3 • LIMO
Databases       SQLite • DB Browser
Tools           VS Code • Git/GitHub • Linux (Ubuntu/WSL) • PLC • HMI Development
```

### Skills Badges
<div align="left">

![ROS2](https://img.shields.io/badge/ROS2_Humble-22314E?style=flat&logo=ros&logoColor=white)
![ROS](https://img.shields.io/badge/ROS1-22314E?style=flat&logo=ros&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=c%2B%2B&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=flat&logo=c&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=flat&logo=raspberrypi&logoColor=white)
![STM32](https://img.shields.io/badge/STM32-03234B?style=flat&logo=stmicroelectronics&logoColor=white)
![Gazebo](https://img.shields.io/badge/Gazebo-EF6C00?style=flat&logoColor=white)

</div>

---

## 🎯 Featured Projects

### 📦 [Omnidirectional Perception System (OPS)](https://github.com/YongJiee/Omnidirectional-Perception-System)
<div align="left">
<a href="https://github.com/YongJiee/Omnidirectional-Perception-System">
<img src="https://img.shields.io/badge/ROS2-22314E?style=for-the-badge&logo=ros&logoColor=white" />
<img src="https://img.shields.io/badge/Raspberry_Pi-A22846?style=for-the-badge&logo=raspberrypi&logoColor=white" />
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" />
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" />
</a>
</div>

> **Industry Partner: CEVA Logistics** | RSE2109 Project 4

A multi-camera warehouse scanning solution that eliminates barcode dependency by fusing OCR and barcode data across all six faces of a package — generating a **Universal Product Passport** per item in real time. Built on a distributed Raspberry Pi + WSL Ubuntu architecture communicating over ROS2.

**All 3 success criteria met ✅ — 43/43 test scenarios PASS**

| Criteria | Target | Result |
|:--------:|:------:|:------:|
| Resilience | Works when barcode fails | ✅ OCR fallback active |
| Efficiency | ≤ 3s end-to-end | ✅ ~2.1–2.9s per scan |
| Accuracy | ≥ 95% match rate | ✅ Up to 98.7% |

**Key Features:**
- 3× IMX708 cameras via Arducam mux — covers all 6 package faces across inbound + sorting modes
- Multi-signal fusion: Tesseract OCR (PSM 11) + pyzbar barcode + fuzzy SmartMatcher scoring
- Autonomous clock offset calibration (no NTP on isolated ethernet)
- SQLite Universal Product Passport with live DB updates visible in DB Browser
- Resilient to label obscuring, barcode damage, and real-world camera noise

[**→ View Repository**](https://github.com/YongJiee/Omnidirectional-Perception-System)

---

### 🤖 [Autonomous Maze Escape Robot](https://github.com/YongJiee/ROS2-Autonomous-exploration)
<div align="left">
<a href="https://github.com/YongJiee/ROS2-Autonomous-exploration">
<img src="https://img.shields.io/badge/ROS2-22314E?style=for-the-badge&logo=ros&logoColor=white" />
<img src="https://img.shields.io/badge/Nav2-4B8BBE?style=for-the-badge" />
<img src="https://img.shields.io/badge/SLAM_Toolbox-00599C?style=for-the-badge" />
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
</a>
</div>

A fully autonomous maze navigation system using ROS2 with real-time SLAM and intelligent frontier exploration — no prior mapping required. The robot builds its environment model on the fly and dynamically selects escape goals as it explores.

**Results: 95% success rate across 50+ test scenarios, avg. escape time 3.2 min**

**Key Features:**
- Real-time SLAM mapping and localization (SLAM Toolbox)
- Autonomous frontier exploration with dynamic goal selection
- Intelligent obstacle avoidance and recovery behaviours
- Modular multi-terminal system architecture

[**→ View Project Details**](https://yongjiee.github.io/project/project-4) | [**📖 Documentation**](https://github.com/YongJiee/ROS2-Autonomous-exploration#readme)

---

### 🏆 [Systems Engineering Project 1](https://github.com/YongJiee/Systems-Engineering-Project-1-Group-6)
<div align="left">
<a href="https://github.com/YongJiee/Systems-Engineering-Project-1-Group-6">
<img src="https://img.shields.io/badge/ROS1-22314E?style=for-the-badge&logo=ros&logoColor=white" />
<img src="https://img.shields.io/badge/RTAB_Map-4B8BBE?style=for-the-badge" />
<img src="https://img.shields.io/badge/LIMO_Robot-00599C?style=for-the-badge" />
<img src="https://img.shields.io/badge/Navigation-3776AB?style=for-the-badge" />
</a>
</div>

Led a 4-person team building a ROS1-based autonomous navigation system for the LIMO robot platform with RTAB-Map SLAM for indoor environments. Delivered **2 weeks ahead of schedule** with full navigation stack integration.

**Responsibilities:** System architecture · ROS nav stack tuning · Team coordination · Hardware-software integration · Technical documentation

[**→ View Project Details**](https://yongjiee.github.io/project/sep1) | [**📖 Documentation**](https://github.com/YongJiee/Systems-Engineering-Project-1-Group-6#readme)

---

## 📊 GitHub Statistics

<div align="center">

### 💻 Language Distribution

![Top Languages](https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=YongJiee&theme=github_dark&exclude=scss,css,html,javascript,typescript,markdown)
![Most Used Languages](https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=YongJiee&theme=github_dark&exclude=scss,css,html,javascript,typescript,markdown)

### 📈 GitHub Activity Overview

![Profile Summary](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=YongJiee&theme=tokyonight)

![Stats](https://github-profile-summary-cards.vercel.app/api/cards/stats?username=YongJiee&theme=tokyonight)
![Productive Time](https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=YongJiee&theme=tokyonight&utcOffset=8)

</div>

---

## 🏆 Achievements & Background

**🥇 WorldSkills Singapore — Mechatronics (2018–2021)**
- Medallion of Excellence (2020, 2021)
- Two-person team competitions: full system design, build, and programming under time constraints
- Skills developed: PLC programming, HMI development, electrical panel wiring, system integration

**🎓 Education**
- **Robotics Systems Engineering** — Singapore Institute of Technology (Current, Class of 2028)
- **Diploma in Mechatronics** — Nanyang Polytechnic

**💼 Technical Competencies**
- Autonomous robot navigation and control
- Multi-camera computer vision and OCR fusion pipelines
- SLAM and localization systems
- Embedded systems and distributed architecture (Pi + ROS2)
- Industrial automation and PLC systems
- Cross-functional team leadership

---

## 📫 Let's Connect!

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Let's_Connect-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yong-jie-tan/)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit_Site-2563eb?style=for-the-badge&logo=google-chrome&logoColor=white)](https://yongjiee.github.io)
[![Email](https://img.shields.io/badge/Email-Get_in_Touch-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:tan_yong_jie@outlook.com)

</div>

---

<div align="center">

*"Building intelligent systems that bridge the gap between software and hardware"*

![Profile Views](https://komarev.com/ghpvc/?username=YongJiee&color=2563eb&style=flat-square&label=Profile+Views)

⭐️ From [YongJiee](https://github.com/YongJiee)

</div>
