# IVRAR Group 02: Immersive VR Sensory-Stress Defensive Security Training under Low Visibility
**Course:** Introduction to Virtual Reality & Augmented Reality (IVRAR - Course Code: 702COI002)  
**Academic Term:** Academic Year 2026–2027 | Semester V  
**Institution:** SVKM's NMIMS MPSTME, Mumbai  

---

## 1. Authorized Research Title & Problem Statement
> "How can an immersive VR sensory-stress simulation improve target prioritization and reaction latency for defensive security trainees under simulated low-visibility nighttime conditions?"

### Core Engineering Focus
* **Interactive VR Environment:** Unity OpenXR tactical breach environment simulating nighttime mesopic illumination (0.5-5.0 lux) and volumetric fog (`Assets/index.html` and `Assets/Scripts/`).
* **Sensory-Stress Inoculation:** High-intensity acoustic startle cues (85-95 dB) and peripheral strobe glares during critical engagement windows (`Assets/Scripts/SensoryStressTargetManager.cs`).
* **Signal Detection Telemetry:** Continuous 90 Hz logging of millisecond reaction times, hit rates, false alarm rates, and Signal Detection Theory metrics (d', \beta) (`Assets/Scripts/ReactionLatencyTelemetryLogger.cs`).
* **Techno-Managerial Systems Evaluation:** Dimensionless operational model analyzing live-fire ammunition replacement and shoot-house facility rental substitution (`telemetry/sensory_stress_defense_roi.py`).
* **Human Factors & Cognitive Workload:** Standardized assessments via NASA-TLX, Kennedy SSQ cybersickness, and Situational Awareness Global Assessment Technique (SAGAT) (`telemetry/`).

---
## 2. Student Engineering Team Matrix

| Roll No | SAP ID | Student Name | Technical Role | Assigned Git Branch |
| :--- | :--- | :--- | :--- | :--- |
| `N024` | `70472400145` | **Ranish Devadiga** | Lead XR Systems Architect | `feat/n024-xr-systems-architect` |
| `N042` | `70472400224` | **Hriday Jain** | Human Factors & Usability Engineer | `feat/n042-human-factors-usabil` |
| `N047` | `70472400031` | **Vedika Kaki** | Spatial Telemetry & Data Lead | `feat/n047-spatial-telemetry-da` |
| `N062` | `70472400154` | **Medha Mishra** | Techno-Managerial Product Manager | `feat/n062-technoeconomic-produ` |

---
## 3. Sprint 0 Onboarding & Toolchain Verification
Verify your local Python, Unity/WebXR, and telemetry toolchain:
```powershell
git clone <repository_url>
cd <repository_root>/Group_02_Ranish_Hriday_Vedika_Medha
git checkout -b feat/n024-xr-systems-architect
python telemetry/test_evaluation_tools.py
python telemetry/sensory_stress_defense_roi.py