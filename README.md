## Digital Investigation Project

### Introduction  
This project documents a **cybersecurity automation and network traffic analysis** task conducted during my internship at **BNS Cyberlab Limited**.  
The investigation involved:  
- Analyzing **packet captures (PCAP)**  
- Reconstructing digital artifacts from raw network traffic  
- Performing **malware analysis** and **threat detection**  

It provided hands-on experience in **digital forensics**, **protocol analysis**, and **incident investigation** in real-world scenarios.

---

### Tools & Methodology  

#### Tools Used
| Tool           | Purpose |
|----------------|---------|
| **Wireshark**  | Network traffic capture, protocol analysis, HTTP traffic filtering |
| **HxD Hex Editor** | Binary file analysis, header inspection, file reconstruction |
| **VirusTotal** | Malware scanning, threat intelligence verification |

#### Methodology  
1. **Packet Capture Analysis**  
   - Filtered HTTP traffic to locate file downloads  
   - Extracted and reconstructed files from packet payloads

   <img width="931" height="244" alt="WS Captured act" src="https://github.com/user-attachments/assets/8e60a5a9-f3d6-4f33-b0bc-0b164a82ffab" />
   <img width="947" height="412" alt="TCP stream" src="https://github.com/user-attachments/assets/9240268f-75a7-41c1-9ea4-5a82d2166d85" />



2. **File Forensics**  
   - Verified file types using **magic numbers (hex signatures)**  
   - Inspected metadata and structure for anomalies

     <img width="952" height="488" alt="Raw DATA" src="https://github.com/user-attachments/assets/8e355b39-a008-4c58-a983-e4907c46c2c9" />


3. **Threat Detection**  
   - Scanned artifacts with **VirusTotal**  
   - Analyzed network patterns for malicious behavior  

---

### Key Findings  

#### 1. `BNS01.JPG` — JPEG Image
- **Signature:** `FF D8 FF` (Start) / `FF D9` (End)  
- **Artefact:**  
  - Congratulatory image featuring **Ali S. Benson**, lead trainer  
  - Cybersecurity-themed visual representing the Network Traffic Analysis module
    ![BNS01](https://github.com/user-attachments/assets/077f282b-c454-49d6-a47f-f8809ba0b76a)


#### 2. `BNS02.PNG` — PNG Logo
- **Signature:** `89 50 4E 47 0D 0A 1A 0A` (Start) / `49 45 4E 44 AE 42 60 82` (End)  
- **Artefact:**  
  - Official BNS Cyberlab Limited logo used in documentation
    ![BNS02](https://github.com/user-attachments/assets/69b17c08-161a-439e-b044-0e5c08f9a476)


#### 3. `BNS03.PDF` — Network Traffic Analysis Guide  
- **Signature:** `25 50 44 46` (Start) / `25 25 45 4F 46` (End)
- **Artefact**
  <img width="1437" height="792" alt="image" src="https://github.com/user-attachments/assets/152baaa8-39d8-4673-8974-950c5d824b20" />

- **Key Points:**  
  - Defines Network Traffic Analysis (NTA) as the process of capturing, inspecting, and interpreting network data  
  - Highlights NTA’s role in **threat detection**.   

#### 4. `BNS04.ZIP` — Supplemental Project Data  
- **Signature:** `50 4B 03 04`  
- **Artefact:**  
  - Contains a BNS-themed financial report, and a flier with the wordings inviting people to join BNC internship.
    
    <img width="634" height="856" alt="image" src="https://github.com/user-attachments/assets/90c4da36-8795-45e8-80fb-cf43d2aecb4a" />
    <img width="900" height="502" alt="image" src="https://github.com/user-attachments/assets/59865d5e-fb7a-4a27-a336-ee5978b4f5af" />



---

### Challenges & Solutions  
| Challenge | Solution |
|-----------|----------|
| Extra data in downloaded files | Used hex editing to isolate valid file content |
| Difficulty identifying file types | Verified magic numbers for accurate format detection |
| Malware risk in extracted files | Pre-scanned all artifacts using VirusTotal |

---

### Conclusion & Skills Gained  
This project strengthened my expertise in:  
- **Network Forensics** — Wireshark, PCAP analysis  
- **Binary File Reconstruction** — Hex editors, magic numbers  
- **Threat Intelligence Integration** — VirusTotal, malware detection  

It reinforced the importance of automation in cybersecurity — integrating email parsing, malware scanning, and network monitoring into a single defense workflow.

---

### Future Improvements  
- Automate file extraction from PCAPs using Python scripts. 
- Expand signature detection for advanced file types.  
- Integrate machine learning for anomaly detection in network traffic.  

---

**Prepared by:** Olatunji Lawal  
**Date:** 13th August, 2025  
