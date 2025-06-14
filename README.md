# 🧠 ChipTop – VLSI Physical Design Project (RTL to GDSII)

## 🔧 Tools Used
- **Synopsys Design Compiler** – RTL Synthesis  
- **Synopsys IC Compiler II (ICC2)** – Floorplan, Placement, CTS, Routing  
- **Synopsys PrimeTime** – Static Timing Analysis (STA)  
- **Technology Node**: 28nm standard cell library  

---

## 📘 Project Description
**ChipTop** is a physical design project implemented on **28nm technology**, operating at a target frequency of **1.2 GHz**, integrating **4 custom macros**. The physical implementation achieved efficient performance with **no congestion**, optimal utilization, and clean timing closure.

---

## 🛠 Flow Steps

### 1. RTL Synthesis (Design Compiler)
- RTL analyzed and elaborated
- Target and link libraries set
- Clock constraints applied
- Netlist generated with 10k standard cells
- Reports: area, power, and timing

### 2. Floorplanning (ICC2)
- Core utilization set to **60%**
- Aspect ratio of **1.0** (square)
- Macros placed manually for minimal interference
- IO pads placed **right-to-left**
- Core boundary and routing halos defined

### 3. Power Planning
- Power rings and horizontal stripes inserted
- IR drop checks ensured stable delivery
- Power and ground nets created based on macro placement

### 4. Placement
- Standard cells placed using congestion-aware algorithm
- Placement legalized and optimized
- No cell overlaps or density hotspots

### 5. Clock Tree Synthesis (CTS)
- Global and local clock tree built using H-tree
- Balanced skew and minimized insertion delay
- Clock tree buffers and inverters inserted

### 6. Routing
- Performed global then detailed routing
- DRC and antenna clean
- Metal layers assigned based on tech rules

### 7. Static Timing Analysis (PrimeTime)
- Setup and hold analysis run
- All paths met timing (no negative slack)
- Reports for worst path delay, slack, and arrival time generated

---

## 📊 Results

| Metric               | Value            |
|----------------------|------------------|
| Target Frequency     | 1.2 GHz          |
| Standard Cell Count  | ~10,000          |
| Macros Integrated    | 4                |
| Utilization          | 60%              |
| Aspect Ratio         | 1.0              |
| IO Placement         | Right to Left    |
| Congestion           | None (0%)        |
| DRC / LVS            | Clean            |
| Worst Slack (WNS)    | Positive (Met)   |
| Total Power          | Within limits    |

---

## 📸 Snapshots
*Note: Screenshots not uploaded due to NDA*

- Floorplan with macros and IO placement
- Placement view showing congestion-free layout
- Clock Tree Viewer snapshot with balanced branches
- Routing layout with metal layers and power nets
- PrimeTime report screenshot of setup/hold results

---

## 📌 Notes
- Work completed on a licensed Synopsys server under academic environment  
- Source files (.tcl scripts, RTL, libraries) not uploaded due to license constraints  
- All flow steps were scripted using Synopsys-standard commands  
- Reports and views reviewed manually at each stage to ensure clean results  

---

## 🎯 Purpose
This project demonstrates my hands-on experience in the complete RTL-to-GDSII Physical Design flow using industry-grade tools.  
It reflects my understanding of floorplanning, timing closure, congestion management, and layout optimization in an advanced node (28nm).  
The goal of this repository is to showcase my ability to work on real-world chip implementation with professional EDA tools and workflows.

