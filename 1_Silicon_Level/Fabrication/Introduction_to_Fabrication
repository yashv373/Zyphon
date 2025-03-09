Author: Yashvardhan Singh

## Introduction
This is the actual process of physically making the transistors/hardware/chiplets in real life.
Semiconductor fabrication is the intricate process of transforming raw silicon into the advanced microchips that power modern technology. This involves a series of controlled steps each executed at the super small scale, to build transistors and interconnections layer by layer. From the atomic-level oxidation of silicon to complex patterning using lithography, every step in fabrication is a delicate balance of chemistry, physics, and engineering. The process takes place in ultra-clean environments known as **cleanrooms**, where even a single dust particle can ruin an entire chip. At its core, fabrication is the art and science of **sculpting silicon** into functional circuits, enabling everything from smartphones to supercomputers.

---
## Base
The base material for all fabrication is silicon due to multiple reasons, such as abundance, low reverse saturation current, ease of forming oxides, good thermals and good doping versatility.
## Cleaning
This is pre-requisite for the fabrication process as there are many kind of the impurities on the base that we operate on.
We generally have 2 cleaning processes:
1. RCA-1: deals with organic impurities such as wax , dust , oil.  Some other methods also exist for this like the piranha cleaning.
2. RCA-2: deals with inorganic impurities such as metallic ions.
3. All of the fabrication is carried out in a pre-defined controlled environment called Cleanrooms. Cleanrooms are classified into types on the basis of the number of particles present in the room. For instance, Class 10 would have 10 particles/cm^-3 and Class 100 which is the standard for most of the cleanrooms would have 100 particles/cm^-3.

---

# Fabrication Workflow
So, the stuff we discussed previously to this segment is mostly what we can call as the pre-requisites to carry out fabrication.
Steps involved in the fabrication workflow (order is not rigid):
1. Oxidation
2. Lithography
3. Etching
4. Deposition
5. Diffusion or Ion-Implantation

---

## Oxidation
Oxidation is the process where in we basically grow the oxide layer on top of our wafer.
SiO2 (Silicon dioxide) is the industry standard. Around 40-44% of the wafer is consumed while growing the oxide. For every 1 nm of SiO₂ grown, approximately **0.44 nm** of silicon is consumed.
There are 2 broad kinds of oxidative methodologies:

- **Dry Oxidation**: Si + O₂ → SiO₂ (Slow, high-quality oxide)
- **Wet Oxidation**: Si + 2H₂O → SiO₂ + 2H₂ (Faster, lower quality)

1. Dry Oxidation: Uses O2(oxygen) to carry out the oxidation reaction. This process is very efficient and is have negligible impurity concentration in output. But, this is a super slow process.
2. Wet Oxidation: Uses H2O (water) to carry out the oxidative process. Lower in terms of output quality with respect tot the dry oxidation process. So, places where we need isolative oxide, we generally opt for wet oxidation as the quality of oxide does not play a major role here.

---
## Lithography
It is basically a patterning technique, to create desirable patterns in the oxidation layer.
The general lithography process is as follows ( we are discussing the steps in the optical lithography process specifically here):

1. A layer of photoresist (PR) is deposited on top of the the oxide layer. This helps us in carrying out the patterning. PR is generally classified into 2:
   1. Positive Photoresist - becomes soluble on interaction with UV light, easier to handle than negative.
   2. Negative Photoresist - becomes hard (hardens) on interaction with UV light, or the areas become crosslinked and insoluble.
   
2. A mask is needed, which basically is used to block out the areas where we don't want removal of layer or the patterning to not occur. So, basically a stencil for us to use while incident-ing UV Light on the PR to make sure we only get rid of the areas that are non-essential to us. Masks can be of 2 kinds -> 
   1. Bright Field Mask - Allows UV light through most areas, exposing PR in those regions. Area not needed to be removed is opaque which is minor and everything else transparent which is major in terms of area shared.
   2. Dark Field Mask - Blocks UV light in most areas, preventing PR exposure. Area  needed is opaque which is major and the rest is transparent and minor in terms of area shared.
   
3. The light incident is UV or ultraviolet light which is can be classified into 3 based on their wavelengths. Lesser the wavelength, better is the resolution. The best resolution for this optical-lithography process is 1um, due to diffractive limitations. UV lies in <450nm range.
   1. G line - 436 nm
   2. H line - 405 nm
   3. I line - 365 nm
   
4. Why optical lithography over other kinds of lithography?
   1. It is an easy process to execute.
   2. wafers with 6-10 inch radius can be manufactured.
   3. Fast process
   4. Cost-effective
   5. But as we saw in above discussions, the optimal resolution is 1um for this process and for technology nodes below that we will need better lithography. Some such contenders are the XRAY and DUV lithography, but they need custom PRs which significantly raises the cost. These methods are advanced and more cost demanding but provide much higher resolutions (lower tech. nodes). Some other maskless lithography processes are:
      1. Electron beam lithography
      2. Ion Beam or FIB (Focused Ion beam) Lithography
      3. Interference Lithography
      4. Deep Pen Nano-Lithography
  
5. Some more concepts to explore in the lithography stage of fabrication, that are slightly advanced:
   1. raster-scan
   2. serial process
   3. time-resolution tradeoff
   
6. A big thing In the lithography stage that we have to worry about is the distance between the mask and the photoresist. For this, we have 3 classifications:
   1. Contact-mode: virtually no gap between the mask and photoresist. Here, due to such close proximity, the light doesn't deflect and gets contaminated.
   2. Proximity-mode: very short but optimal gap between the mask and PR, and this is the one we prefer.
   3. Projection-mode: Relatively large gap, causing huge light deflection and inaccuracies in the lithography process.

---

## Etching
Etching is the process of removal of undesired layers that we previously deposited. This process can only take place if lithography has been completed. It is good to know that this process practically doesn't produce sharp vertical profiles, which can be misleading in many diagrams. It is majorly classified into two parts:
1. WET ETCHING -
   The exposed SiO2 which is undesired and marked with the help of mask and photoresist in the lithography is removed using Hydrogen fluoride because it has high selectivity. Vertical profiles are slanted (not sharp).  HF (hydrofluoric acid) is poured over the wafer, and it chemically reacts with the exposed SiO₂ (oxide), dissolving it into a soluble compound (like SiF₆²⁻ in the case of HF). The dissolved material is then rinsed away using a cleaning solution (usually DI water). The problem? Wet etching is isotropic, meaning it removes material in all directions, leading to slanted edges instead of sharp vertical walls.
2. DRY ETCHING -
   If sharper vertical profiles are required, we tend to go for dry etching which is also referred to as Reactive Ion Etching. Here, we instead use a plasma with the PR and SiO2, which etches them away.  Instead of using a liquid chemical, plasma (ionized gas) is used. This plasma contains reactive ions (like CF₄, SF₆, Cl₂, etc.) that bombard the surface, breaking atomic bonds in SiO₂ and making it volatile (turning it into a gas). The gaseous byproducts are then vacuumed away from the chamber. Since this is directional (anisotropic), it gives sharper, more vertical sidewalls.

---

## Deposition
1. Physical Vapor Deposition (PVD): PVD is a process where a thin film is deposited on a wafer by physically ejecting material from a solid target and transferring it to the substrate. Highly energetic ionic light beam is bombarded onto a metallic target (aluminum), which gets etched from the target, deflected towards the wafer and deposited onto the wafer surface. 
   1. Sputtering - using ions as the light beam
   2. Electron beam - electronics as the light beam
2. Chemical Vapor Deposition (CVD): This method doesn't need a target, and follows a oxidative-like approach. chemical reactions occur in a vapor phase, leading to thin film deposition on the wafer surface. This method allows for coatings and high-purity films.
   1. Atmospheric Pressure (APCVD) - at room pressure
   2. Low Pressure (LPCVD) - low pressure
   3. Plasma Enhanced CVD - using plasma to enhance this process and carry out cvd at low temperatures.

---

## Diffusion / Ion Implantation
This is the process of doping, or implanting desirable ions the region that we cleared out. Since the region we want to dope is now at the surface, without any PR or SiO2 on top of it, we can now dope those regions with requirement-based impurities, trivalent or pentavalent and make them n+ or p+ regions to get desired MOS structures.
This is generally a 2 step/way procedure, with its two steps as:
1. Spin on dopant/Diffusion - A liquid source containing dopant atoms is spun onto the wafer, forming a uniform layer. The wafer is then heated in a furnace, causing the dopant atoms to diffuse into the silicon lattice. This method is thermally driven and works well for shallow doping. 
2. Dry Beam/Ion Implantation - A high-energy ion beam is directed at the wafer, forcing dopant atoms deep into the silicon. The doping depth and concentration can be controlled precisely by adjusting the energy and dose of the ion beam. This method is preferred for sharp, controlled doping profiles and is commonly used in modern CMOS processes.


---

### Summarized General Workflow for Fabrication for CMOS:
1. Cleaning and Pre-preparation
2. Substrate selection (p-sub / n-sub)
3. SiO2 deposition by oxidation
4. Lithography for getting the desired patterns
5. Etching out unwanted depositions
6. Doping 1 and Doping 2 (N and P)
7. Deposition of Gate and other metal contacts (polysilicon)


---

## CMOS Fabrication Techniques:
1. N-well CMOS Fab - selecting substrate as P-sub in step 2 of the general workflow and fabricating n-wells into it. N-wells are created for PMOS transistors, while NMOS transistors are built directly on the p-substrate. Most common process due to its simpler fabrication and better NMOS performance.
2. P-well CMOS Fab - selecting substrate as N-sub in step 2 of the general workflow and fabricating a p-well. Less commonly used than the N-well process.
3. Twin Tub CMOS Fab - discussed ahead
4.  Silicon on Insulator Fab - discussed ahead

problems with N-well and P-well Fabrication:
1. Vth control: The Threshold voltage is dependent on doping concentrations. Since the nmos and pmos devices are fabricated in the same substrate with a well for the other type, controlling and maintaining similar doping for these regions is challenging and a problem for symmetric n and p devices in terms of doping, which helps us in turn take control of what happens to Vth and generally help us build more balanced circuitry.
2. Body biasing issues: n devices need p as a body connect and vice versa for the p devices. A singular body bias for the entire wafer is optimal as it helps have optimal characteristics and control over other properties, which can not be done here as they need separate body connections to different regions.
a potential solution to the above mentioned problems can to be to isolate the nmos and pmos cojoined devices as separate entities. This is precisely the foundation of the Twin - Tub Process.

---
## Twin Tub Process:
Generally same as the earlier processes, but here we do some different steps.
1. Selection of substrate
2. Cleaning
3. Forming the well
4. Gate oxide and Poly-Si
5. Doping
6. Metal contacts
- So we have our N-sub on which we deposit a Epitaxial layer.
- EPITAXY is a process of depositing material of same kind.
- On top of the Epitaxy layer, we deposit the SiO2 via oxidation.
- Then we do lithography to pattern the oxide, and subsequently etch it.
- A n-well is grown by doping the epitaxial layer. 
- Same process is repeated a couple of times to get a p well.
- After all of this, we should have our epitaxy layer with 2 separate wells, where the idea is that these 2 serve as 2 independent MOS devices eventually.
- Now we deposit SiO2, polysilicon, and Photoresist.
- Then we do lithography for the gate contact of both the wells.
- Then another lithography for the source and drain regions (as well as the body), followed by etching and relevant doping.
- After that we will go for the metal contact deposition and that gives us the twin tub structure. The NMOS and PMOS are electrically isolated and can be connected to each other using whatever wiring to metal contacts is needed according to requirements.
  
  #### Problems with the Twin Tub Process:
- formation of PN Junctions at the various P and N interfaces -  The P-well and N-well regions create multiple PN junctions within the wafer. This can lead to leakage currents and unwanted diode effects.
- Formation of SCR - silicon controlled rectifier / thyristor - The P-N-P-N structure can lead to formation of SCR If triggered, it can cause unintended conduction, leading to high currents, overheating, and failure. This Problem is referred to as CMOS Latch Up.

#### Latch-Up Problem:
Latch-up occurs when an unintended P-N-P-N structure inside a CMOS device forms a parasitic thyristor (SCR). This SCR, once triggered by a voltage spike or transient current, enters a conducting state and creates a low-resistance path between Vdd and Vss. This results in excessive current flow, overheating, and possible device failure. The only way to stop it is by cutting power.
For latch-up to occur, two parasitic transistors are unintentionally formed inside the silicon:
A PNP transistor (inside the N-well)
An NPN transistor (inside the P-well)
These two transistors form a positive feedback loop, meaning:
A small current spike (e.g., due to noise, radiation, or voltage fluctuations) turns on one transistor. This feeds into the second transistor, turning it on too. The second transistor feeds back into the first one, reinforcing the loop. Now, both transistors are stuck in the ON state permanently, creating a low-resistance path from power (Vdd) to ground (Gnd).
Result - Massive current flows, overheating, and possibly destroying the device.
 In simple terms, it’s like flipping a light switch that won’t turn off, no matter what.
 
 How to overcome Latch Up?
Lower resistance in the device means it’s harder for the feedback loop to sustain itself.
The base resistance of these parasitic transistors determines how easily they turn on.
Higher resistance in feedback loop → Harder for latch-up to trigger.
Lower resistance in feedback loop→ Easier for latch-up to happen.
Since we don’t want latch-up, we need to increase resistance in the right places (between wells and substrate) while keeping resistance low where we need good conduction.
We Lower Resistance in the Right Places to Drain the Trigger Current Away
If we lower the resistance of well and substrate contacts (e.g., by adding guard rings or using heavily doped regions), we give the excess current a safe path to escape instead of feeding back into the parasitic SCR.
This prevents enough voltage buildup to forward-bias the parasitic transistors and stops the feedback loop before it can start.

So basically: 
- Increase resistance in the feedback path → Makes it harder for the loop to sustain itself.
- Lower resistance in well and substrate contacts (device)→ Helps drain unwanted current safely before it can trigger latch-up.

So how do we decrease the resistance in device?
1. More doping - but this can cause high leakage 
2. Guard Rings - Extra doped regions that act as a drain for excess current.
3. Trench Creation - isolate n-well and p-well from the sub
4. Graded Doping - gradient concentration of doping
5. Epitaxy - was previously discussed, but this is very expensive process
6. SOI or Silicon on Insulator - best solution for the Latch up issue
## Silicon on Insulator (SOI) Process:
Here we have a Sapphire (Al2O3) substrate which is good for high power applications. then we deposit silicon onto this sapphire substrate, and this process is called hetero-epitaxy (depositing unlike materials), and then we have our regular sio2 and polysilicon.
Sapphire and SiO2 have least lattice mismatch meaning they are super compatible and show great output, are stress-resistant and don't develop cracks.
SOI doesn't struggle with latch-up and provides great electrical isolation.
Modern SOI mainly uses **buried SiO₂ (BOX - buried oxide layer)** instead of Sapphire (SOS) due to thermal incompatibility as an insulator instead.

SOI Technologies:
1. SOS - silicon on sapphire -Silicon deposited on a sapphire substrate. Great for high-frequency & radiation-resistant applications.
2. SIMOX - separation by implanted oxide -Oxygen ions are implanted into silicon, creating a buried SiO₂ layer after annealing.
3. BESOI - bond and etch back SOI -Two silicon wafers are bonded with SiO₂, and one is etched down to a thin active layer.
4. ELTRAN - epitaxial layer transfer - Uses an epitaxial silicon layer on a removable donor wafer, later transferred to another substrate.
5. Smart Cut - Uses ion implantation and wafer bonding to precisely control the thickness of the top silicon layer. 

---
