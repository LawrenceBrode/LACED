# LACED™ – Laser-Assisted Controlled Etching and Delayering
## Author: Lorentio Brodesco - Brodesco Industries 2025
##### "Failure built precision."
##### 2025.05.10 - Revision 1.0
<img src="https://github.com/LawrenceBrode/LACED/blob/main/edited/halfhalf.png" width="400" alt="TEST PCB WITH EXPOSED LAYER 1 AND 2">

## Abstract
### Overview of the project
**LACED** is an innovative delayering technique developed for reverse engineering modern hardware, with a focus on multilayer PCBs, using an **extremely accessible and low-cost approach**. It combines **a low-power, budget-friendly UV laser**, simple chemical solutions, and micrometer-based precision tracking — enabling advanced circuit exploration without the need for industrial tools or cleanroom environments.

Through this process, **LACED achieves precision levels between 3.5 and 10 microns**, bridging the gap between DIY and professional-grade delayering.

More than just a method, **LACED is a mindset**:

> _To prove to the world that ingenuity beats million-dollar industries._

### Project Goals

The LACED™ technique was developed with the following goals in mind:

1.  **Accessibility**  
     To enable advanced delayering and reverse engineering using only low-cost, widely available tools — without the need for industrial machinery or cleanroom environments.
    
2.  **Precision**  
     To achieve micron-level control (3.5–10 µm) in the removal of FR4 and copper layers, making it suitable for high-resolution hardware analysis.
    
3.  **Documentation**  
     To create a detailed and replicable methodology that can be adopted, improved, and shared by the maker and research communities.
    
4.  **Empowerment**  
     To prove that a single person, in a bedroom lab, can match the results of processes that normally require million-dollar setups.
    
5.  **Emotional Purpose**  
     To explore not only circuitry, but memory — by uncovering physical messages hidden between PCB layers, turning reverse engineering into an act of personal and artistic expression.

### Key Results & Why It Matters
✅ Achieved physical precision between 3.5 and 10 microns, using a low-cost CNC diode laser (5W), micrometer tracking, and basic chemical etching — all performed in a home environment.

✅ Successfully exposed internal copper layers of a 6-layer PCB, proving that high-resolution delayering can be accomplished without industrial tools like FIB systems or pro-grade milling stations.

✅ Recovered a hidden message engraved between layers — showing that LACED is not only a technical method, but also a form of expression capable of revealing both data and meaning.

✅ Developed a fully documented, step-by-step methodology, reproducible with accessible equipment, allowing anyone with curiosity and discipline to explore modern hardware at micron scale.

> Why it matters:
> LACED lowers the entry barrier to advanced PCB analysis and digital preservation.
> It empowers individuals to explore, understand, and protect hardware — not with money, but with ingenuity, precision, and intent.

## Introduction

### Context & Origin
This process was born from a very specific need:
gaining access to the internal layers of multilayer PCBs for reverse engineering.

At first, I theorized that a 5W UV diode laser could be used to remove the soldermask without having to do it manually — eliminating the need for sandpaper and the inconsistent pressure of a human hand, which often leads to uneven surface removal.

Then came the realization:
the laser could also ablate the FR4 itself.
That’s when a deeper idea took shape — what if I could use the laser to remove all layers of FR4 and dielectric material with consistent precision, rather than relying on error-prone manual sanding?

But very quickly, I hit a fundamental physical limitation: copper.

The copper traces on the board would not be affected by the laser.
And even if I increased power to the point of engraving copper, the material’s thermal properties are so different from FR4 that I would overburn the substrate while barely affecting the copper itself.

That’s when a new idea struck:
I remembered how PCBs are fabricated — a process I had replicated at home.
In standard manufacturing, a uniform copper layer is coated with a photoresist, then selectively etched with acid, leaving only the designed traces.

What if we inverted the logic and used acid not to preserve the traces, but to remove them completely?

With this shift, the theoretical workflow became clear:
laser-assisted soldermask removal, acid-based copper etching, and layer-by-layer FR4 ablation.
A fully controlled, repeatable process — at least in theory.

> And as my friend Oppenheimer once said, “Theory only gets you so far.”

### How This Differs from Traditional Approaches
Traditional manual sanding — using fine sandpaper to gradually expose PCB layers — has long been the go-to method for low-budget delayering. While it’s simple and doesn’t require sophisticated tools, it suffers from major limitations:

❌ Inconsistent pressure from the hand leads to uneven layer removal.

❌ Risk of over-sanding or skipping layers, especially when approaching internal copper.

❌ Lack of precision tracking — no reliable way to measure removal depth micron by micron.

❌ Requires experience and luck to achieve uniformity across the board.

❌ Irreversible damage is common when targeting a specific layer.

LACED™ eliminates these issues by replacing guesswork with control.

✅ Uses a low-power CNC diode laser to ensure consistent surface processing across the entire PCB.

✅ Incorporates micrometer-based depth tracking after each pass.

✅ Combines chemical copper removal to avoid thermal stress and material distortion.

✅ Achieves repeatable results down to 3.5–10 µm, far beyond manual sanding tolerances.

✅ Allows precise stopping at specific layers without overshooting.

> In short: manual sanding relies on intuition and hope. LACED relies on precision and repeatability.

## The Greatest Challenge in LACED
One of the most critical and frustrating challenges in the LACED process was the unintentional damage to copper traces — especially the finer ones — during laser carbonization of the FR4 substrate.

When using a diode laser to ablate the surface, excessive heating of the FR4 can occur. This heat, in turn, radiates into nearby areas, often beneath the copper traces. The result: localized carbonization and mechanical delamination of the copper, causing the traces to lift, warp, or detach.

This issue was particularly severe in the early phases, when I was still calibrating laser power and speed parameters. It was not just a technical setback — it was deeply frustrating, because it often ruined boards that had taken hours of precise work.

But today, that challenge has been overcome.

The process is now stable and predictable, thanks to those early failures.
And that’s why I say:

> Failure builds precision.

##### Early test on a SSD PCB with traces affected by unintended delamination due to carbonization
<img src="https://github.com/LawrenceBrode/LACED/blob/main/misc/damagedSSD.jpeg" width="300">

##### Successful test on a SSD PCB
<img src="https://github.com/LawrenceBrode/LACED/blob/main/misc/sucessefulSSD.jpeg" width="300">

## Tools and Materials

The following tools and chemicals were used to perform the LACED™ delayering process.
All items are low-cost, widely available, and suitable for a compact home lab setup.

🔧 Hardware & Instruments

##### ATOMSTACK A5 Diode Laser – 5W

~€160 — Entry-level CNC laser engraver with adjustable speed/power and good stability for micron-scale ablation.

##### Generic Micrometer – 1 µm resolution

~€10–15 — Used for precise measurement of PCB thickness after each pass.

##### Protective Laser Goggles

Included with the laser machine — Essential for eye protection during engraving.

🧪 Chemicals

##### Sodium Hydroxide (NaOH), 1 kg

~€5 — Used for soldermask softening and initial surface preparation.

##### Hydrochloric Acid (HCl), 32%, 1 L

~€1.50 — Primary agent for copper etching.

##### Hydrogen Peroxide (H₂O₂), 3%, 0.3 L (higher concentration >15% recommended)

~€2 — Used in combination with HCl for controlled etching of copper.

##### Acetone (C₃H₆O), 0.5 L

~€4 — Used for final cleaning and degreasing of PCB surfaces.

> Total estimated cost: under €200. For a fully functional, repeatable delayering lab — no cleanroom required.

## Chemical Insights

### 🧪 Sodium Hydroxide (NaOH)
Role: Soldermask softening and surface preparation
Sodium hydroxide is used to weaken and partially dissolve the soldermask layer, especially on PCBs with hard, cured resins.
It allows for easier removal via laser or abrasion by breaking down polymer bonds. NaOH also helps to degrease and open the surface, improving the penetration of etching agents in subsequent steps.

> Caution: NaOH is highly caustic — always use gloves and eye protection.

### 🧪 Hydrochloric Acid (HCl, 32%)
Role: Copper etching
Hydrochloric acid is the primary etchant used in combination with hydrogen peroxide.
While not aggressive toward FR4 or soldermask, it reacts readily with metallic copper.
Its effectiveness increases when paired with H₂O₂, enabling selective, controllable dissolution of copper layers, even under semi-transparent resin.

> The reaction produces heat and gas — use in well-ventilated areas.

### 🧪 Hydrogen Peroxide (H₂O₂, 3%–15%)
Role: Oxidizing agent for copper etching
Hydrogen peroxide provides the oxidizing power needed to accelerate the reaction between HCl and copper.
Higher concentrations (>15%) significantly improve etching speed and reduce undercutting.
It also enhances copper contrast for visual inspection during partial etching phases.

> For best results, use fresh peroxide and avoid light exposure.

### 🧪 Acetone (C₃H₆O)
Role: Post-laser cleaning and carbon residue removal
Acetone is used to clean the PCB after each laser pass, removing soot, carbonized epoxy, and organic residues.
This step ensures clear visibility, uniform laser interaction, and prevents thermal buildup caused by leftover debris.
Its strong solvency restores the board’s optical clarity before measurement or acid treatment.

> Evaporates quickly; apply in well-ventilated areas and avoid flames.

## Methodology - Step-by-step process of LACED
> NOTE: For clarity and readability, all intermediate measurements taken between optical passes are documented in the following chapters rather than inline with each step.

### Step 1: scanning the PCB

The first critical step is scanning the PCB before making any modifications.
In the context of reverse engineering, it's essential to preserve and archive every trace of information — no matter how small.

> Please excuse the image quality: at the time, I was limited to a 600 DPI scanner, but completeness took priority over perfection.

##### layer 1
<img src="https://github.com/LawrenceBrode/LACED/blob/main/edited/layer1.jpg" width="400">

##### layer 6
<img src="https://github.com/LawrenceBrode/LACED/blob/main/edited/layer6.jpg" width="400">

### Step 2: Soldermask Removal
The second step involves removing the soldermask layer, using a purely chemical process rather than a mechanical one.
Approximately 200 grams of sodium hydroxide (NaOH) are dissolved in 500 mL of water heated to around 80 °C to accelerate the reaction.

>⚠️ Warning:
Do not inhale fumes and avoid any contact with the solution.
Always protect your eyes and respiratory system, and carry out this step outdoors or in a well-ventilated area.
A solution at this temperature is capable of breaking down organic material in a matter of minutes.

<img src="https://github.com/LawrenceBrode/LACED/blob/main/misc/IMG_3027.jpg" width="200">

<img src="https://github.com/LawrenceBrode/LACED/blob/main/misc/IMG_3026.jpg" width="200">

##### Result:
<img src="https://github.com/LawrenceBrode/LACED/blob/main/misc/IMG_3029.jpg" width="400">

<img src="https://github.com/LawrenceBrode/LACED/blob/main/misc/IMG_3031.jpg" width="400">

### Step 3: scanning the soldermask-less PCB
<img src="https://github.com/LawrenceBrode/LACED/blob/main/edited/layer1soldermaskless.jpg" width="400">

<img src="https://github.com/LawrenceBrode/LACED/blob/main/edited/layer6soldermaskless.jpg" width="400">

### Step 4: Copper Removal (HCl+H2O2+H2O)
In the fourth step, we remove the first and sixth copper layers using a chemical-only approach.
The etching solution is composed of approximately 250 g of hydrogen peroxide (3%), 100 g of hydrochloric acid (32%), and about 50 g of water heated to 80 °C to enhance the overall energy of the solution and accelerate the reaction.

> Adding hot water increases the thermal energy of the mixture, which boosts the chemical reaction rate without the risks of directly heating reactive components. This method helps achieve a faster and more uniform copper removal, especially when working with larger surface areas.

<img src="https://github.com/LawrenceBrode/LACED/blob/main/misc/IMG_3032.jpg" width="200">

##### The PCB during the etching process
<img src="https://github.com/LawrenceBrode/LACED/blob/main/misc/IMG_3034.jpg" width="200">

##### The PCB post etching (scan)
<img src="https://github.com/LawrenceBrode/LACED/blob/main/edited/layer1copperless.jpg" width="400">

<img src="https://github.com/LawrenceBrode/LACED/blob/main/edited/layer6copperless.jpg" width="400">

### Step 5: Laser setup

In this phase, we configure the laser settings through dedicated software.
For this project, I used LaserGRBL, a free and lightweight tool for managing CNC laser paths.

While I won’t go into detail about how to generate the CNC masking paths, I will focus on the core settings used to achieve consistent, high-precision results:

Nominal Laser Power: 5 Watts

Active Power Setting: 250/1000 (~1.25 W)

Resolution: 10 lines per millimeter

Engraving Speed: 2000 mm/min

> These parameters were carefully calibrated to ensure controlled ablation of the FR4 substrate without damaging copper traces or underlying layers.

> Based on average measurements, this configuration achieves an ablation depth of approximately 12.75 microns per pass.
Higher precision can be obtained by either reducing the laser power or increasing the engraving speed.
The finest resolution recorded during testing was 3.2 microns per pass.

### Step 6: Laser Engraving Cycle
<img src="https://github.com/LawrenceBrode/LACED/blob/main/misc/IMG_3036.jpg" width="400">

This process was carried out over 10 laser passes, though the removal depth was not perfectly consistent across all cycles. Variations were likely caused by minor surface irregularities, non-uniform PCB layering, and subtle fluctuations in laser focus.

Additionally, as the ablation approached the copper layers, the removal depth per pass tended to decrease slightly — most likely due to the higher thermal conductivity of copper, which dissipates heat more effectively and limits localized burn-in.

The PCB, measuring 5×5 cm, required approximately 15 minutes per pass. After each cycle, the surface was cleaned thoroughly using a soft brush and acetone, to remove carbonized residue and ensure optimal laser interaction for the following pass.

> NOTE: After nine laser passes, the copper layer was nearly exposed. At this stage, a multimeter reading showed a resistance of approximately 120 MΩ, indicating a near-contact condition.
Following the tenth pass, the copper was fully exposed, and the measured resistance dropped significantly to 0.7 Ω, confirming direct electrical continuity.

### Step 7: Cleaning and Scanning
<img src="https://github.com/LawrenceBrode/LACED/blob/main/misc/IMG_3047.jpg" width="600">

<img src="https://github.com/LawrenceBrode/LACED/blob/main/misc/IMG_3043.jpg" width="600">

<img src="https://github.com/LawrenceBrode/LACED/blob/main/edited/layer2.jpg" width="400">

<img src="https://github.com/LawrenceBrode/LACED/blob/main/edited/layer2gray.jpg" width="400">

