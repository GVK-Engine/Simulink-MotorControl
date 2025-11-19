# Simulink-MotorControl
Simulink + MATLAB Motor Control Experiment
# ⚙️Simulink & MATLAB Motor Control
**Course:** Mechatronic Systems  
**Author:** VamshiKrishna Gadde
**Institution:** Arizona State University  

![MATLAB](https://img.shields.io/badge/Software-MATLAB-red)
![Simulink](https://img.shields.io/badge/Tool-Simulink-orange)
![Control](https://img.shields.io/badge/Control-Motor_Control-blue)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📘 Overview
This lab focuses on building a **Simulink closed-loop motor control system** and validating the response in MATLAB.  
The objective is to understand:

- First-order plant modeling  
- Step response shaping  
- Simulink block-level control design  
- MATLAB-based parameter tuning  
- Velocity tracking performance  

Full report available in:  
📄 `report/Lab4_RAS550.pdf`

---

## 🧩 Repository Structure
```
RAS550-Lab4-Simulink-MotorControl/
├── report/
│   └── Lab4_RAS550.pdf
├── simulink/
│   └── lab4_model.slx
├── matlab/
│   └── lab4_script.m
└── results/
    ├── output_plot.png
    ├── simulink_screenshot.png
    └── block_diagram.png
```

---

## 🛠 Tools Used
| Tool | Purpose |
|------|---------|
| **MATLAB** | Simulation + control analysis |
| **Simulink** | Block-level motor model |
| **Scope & Workspace Logging** | Data visualization |
| **Google Drive** | Video demonstration |

---

## 🚀 How to Run the Model
### **1. Open Simulink Model**
```
simulink/lab4_model.slx
```

### **2. Run Simulation**
Click **Run** to generate motor response.

### **3. Execute MATLAB Script**
```
run matlab/lab4_script.m
```

This script:
- Imports simulation data  
- Plots motor output  
- Computes dynamic parameters  

---

## 🧠 MATLAB Script (example)
```matlab
load('motor_data.mat');

t = simout.time;
y = simout.signals.values;

figure; plot(t, y, 'LineWidth', 2);
xlabel('Time (s)');
ylabel('Output');
title('Motor Response - Lab 4');
grid on;
```

---

## 📊 Output Plot

<img width="1736" height="1046" alt="Lab4_PD_Position_Response2" src="https://github.com/user-attachments/assets/0d18845a-bf53-47b7-8b06-606717b12766" />


---

## 🎥 Demonstration Video
- **Google Drive Folder:** https://drive.google.com/drive/folders/12fN4H_ZdaTMknls4Ac_HjabLGKm6GTJe?usp=sharing

## 🧩 Key Learnings
- Importance of **time constant** and **gain** in first-order systems  
- How Simulink simulates dynamic behavior  
- Effect of parameter tuning on rise time & settling time  
- Linking MATLAB scripting with Simulink output  

---

## 👤 Author
**VamshiKrishna Gadde**  
📧 vgadde5@asu.edu  
🔗 LinkedIn: https://www.linkedin.com/in/vamshikrishna-gadde9999/  
💻 GitHub: https://github.com/GVK-Engine  

---

## 🪪 License
MIT License – free for academic use.
