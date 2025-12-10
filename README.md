##  Project Summary
#  Porject : Alstom-Foldable-Stackable-Rack-for-Railway-Packaging  
#  Mission : Innovative-Design-Optimization-and-Testing-for-Efficient-Logistics


## Situation
The project took place during a PFA internship at **ALTEN Delivery Center (Rabat)**, working on a project for **Alstom**, a global leader in railway transport. The specific context involved the logistics of railway components (such as air conditioning systems) which are transported on steel frames called "embases". These frames are constructed from S235J2G3 steel profiles and OSB wood plates, designed to be stacked up to three levels high during transport, carrying loads between 150 kg and 250 kg per unit.

## Problematic
The core issue identified was the **lack of logistical efficiency** in the existing frame design.
* **Rigidity:** The standard frames are rigid and non-foldable.
* **"Empty Return" Inefficiency:** When returning empty after delivery, the frames occupy the exact same volume (3.73 m³) as when they are full. This forces Alstom to "ship air," wasting massive amounts of space in containers and trucks.
* **Cost & Storage:** This rigidity leads to high transportation costs, increased carbon footprint, and wasted warehouse storage space.

## Solution Proposed
An innovative **foldable steel packaging frame** was proposed, inspired by the mechanism of camping chairs. The objective was to create a structure that remains robust under load but can collapse into a compact form for return transport.
* **Mechanism:** A modular design utilizing a central "Cross" piece and universal joints (2 degrees of freedom) to allow the frame to fold inward.
* **Digitalization:** Development of a Desktop Application to automate the calculation of dimensions for manufacturing.

## Action Plan
To validate and implement this solution, a rigorous V-Cycle engineering approach was followed:
1.  **Analysis:** Analyze the existing standard frame to establish a performance baseline.
2.  **Design (CAD):** Model the new foldable mechanism using standard hollow profiles to ensure low manufacturing costs.
3.  **Simulation (CAE):** Perform Finite Element Analysis (FEA) to verify the new design resists static loads and stacking forces better than the original.
4.  **Automation:** Develop a Python script to streamline the manufacturing specification process.

## Procedures
* **Structural Design:** Specific critical components were designed, including a central "Cross" node, universal joints for articulation, and removable longitudinal/transverse bars that lock the structure in place during use.
* **Folding Logic:** A 4-step folding process was defined: (1) Remove support bars, (2) Detach transverse/longitudinal bars, (3) Reconfigure the main structure from rectangular to square, (4) Fold the legs inward toward the center.
* **Validation Simulations:** Three specific static simulations were conducted on both the old and new designs using SolidWorks:
    1.  **Base on Ground:** Testing the frame under full load.
    2.  **Top Frame:** Testing the frame supported only by the legs of the unit below.
    3.  **Vertical Legs:** Testing the columns under the combined weight of a stacked column (approx. 5630 N).
* **Software Development:** A Python/Tkinter GUI application was created where manufacturers input global Length/Width, and the script automatically calculates the precise cut dimensions for all steel profiles.

## Results
The comparative analysis between the Standard Design and the New Design yielded impressive quantitative results:
* **Logistical Optimization:** The return volume per unit dropped from **3.73 m³** (Standard) to **0.1843 m³** (New).
* **Space Savings:** This represents a **94.71% reduction** in occupied space during return logistics.
* **Structural Performance:** The new design proved to be mechanically superior:
    * **Factor of Safety (Base on Ground):** Improved from **7** (Standard) to **12** (New).
    * **Maximum Displacement:** Reduced from **0.239 mm** (Standard) to **0.067 mm** (New), indicating higher rigidity.
    * **Vertical Leg Strength:** The Factor of Safety for the legs increased from **26** to **43**, confirming massive load-bearing reserve.

## Conclusion and Impact
The project successfully demonstrated that a foldable packaging solution is not only feasible but mechanically superior to the existing rigid standard. The new design offers a **robust safety margin** (FOS 12+) while solving the critical "empty return" problem.
* **Impact:** Implementing this solution would drastically cut logistics costs and CO2 emissions for Alstom by maximizing truck/container fill rates during return trips.
* **Innovation:** The integration of the Python application adds an "Industry 4.0" dimension, reducing human error in the manufacturing phase.
