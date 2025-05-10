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

