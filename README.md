# UAV Landing Gear Assembly: CAD, Kinematics & Structural Analysis

**Overview:** A complete engineering workflow designing a 50kg UAV landing gear system from a blank screen to shop-ready blueprints.

### 🛠️ Skills Demonstrated
*   **Parametric CAD Modeling:** Assembly constraints, top-down design (Siemens NX)
*   **Sheet Metal Design:** Flat patterns, bend allowances, and bend sequences
*   **Kinematic Motion Simulation:** Mechanism validation, zero-velocity joint resolution
*   **Finite Element Analysis (FEA):** Linear static stress and displacement testing
*   **Technical Drafting:** Multi-view orthographic projection & GD&T (ASME/ISO standards)
*   **Engineering Decision Making:** Root Cause Analysis (RCA) and design optimization

---

### 🎥 Kinematic Motion & Rendering
*To validate the mechanical clearances, a kinematic motion study was conducted to ensure the linkage arm and main strut translated properly without binding.*



[Kinematic_Motion](https://github.com/user-attachments/assets/8580b6ab-cd87-40c4-be00-655cc6567109)




<img width="841" height="595" alt="Render_image" src="https://github.com/user-attachments/assets/8c842d30-fbad-45f6-93b7-1798658b1a34" />

---

### 📐 Engineering Drafting & GD&T
*A complete, shop-ready blueprint was generated. This includes the Bill of Materials (BOM), auto-ballooning, multi-view orthogonal layouts, and a 1:1 scaled sheet metal flat pattern for laser cutting. Critical datum surfaces and position tolerances (GD&T) were applied to ensure axle alignment.*

<img width="1186" height="842" alt="Drafting_Master_Engineering_Drawing" src="https://github.com/user-attachments/assets/a73dbf42-391d-40ac-a725-26c3afc01ba2" />


---

### 🔍 Structural Validation & Root Cause Analysis
*To ensure safety during a hard landing scenario, the assembly was subjected to a 500N upward vertical load on the wheel axle in Nastran.*

<img width="1256" height="830" alt="FEA_Von_Mises_Stress_Results" src="https://github.com/user-attachments/assets/7b9ec96c-cc41-4dec-8b55-79dc3d7829ee" />
<img width="1485" height="830" alt="FEA_Displacement_Results" src="https://github.com/user-attachments/assets/9d81e9d8-60f3-4a8a-9524-8e0aee198fc1" />


> **Root Cause Analysis (Hard Landing Simulation):** 
> During the simulated 500N hard landing, the Aluminum 6061 main strut exhibited localized stresses exceeding the material yield limit (276 MPa). The failure mode is localized plastic deformation at the upper pivot hole due to highly concentrated bending moments (the strut acts as a lever arm). 
> 
> **Corrective Action Proposal:** Increase the outer diameter of the upper pivot boss by 4mm to add structural material to the high-stress zone. If geometric envelope constraints prevent making the part thicker, upgrade the strut material from Aluminum 6061-T6 to Titanium Ti-6Al-4V (Yield: 880 MPa).
