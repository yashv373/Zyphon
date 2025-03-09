## Introduction 
- MOS (Metal-Oxide-Semiconductor) capacitor is a fundamental structure that serves as the building block for modern MOSFETs.
- This is something that was used to eventually end up at the modern day mosfet that we know of. a MOS capacitor is essentially a MOSFET without source and drain regions—it consists only of the gate, oxide, and substrate.
- It aptly explains the capacitive properties of the transistor, and how it is used to control the transistor.

## Structure
The structure is as follows: (from top to bottom)
1. polysilicon (gate contact): The conductive gate material that modulates the electric field.
2. silicon dioxide (SiO2) (the dielectric separation between conductors): An insulating layer that prevents direct charge flow but allows capacitive coupling.
3. Semiconductor substrate (P-type substrate for N-type transistor): A p-type substrate (for NMOS) that reacts to the applied gate voltage.
### Fabrication
Oxide thickness, Threshold voltage, and Doping levels, depend on the fabrication process, and cannot be changed by design; they are technology parameters.

### Overview of Working
The dielectric prevents direct contact between the polysilicon gate contact and the p-type substrate but the build up of charges caused due to applied external voltage can help us control the charge carrier behavior in the p-substrate. i.e. applied gate voltage modulates the surface potential, leading to accumulation, depletion, or inversion in the semiconductor.
## Energy Band analysis

When a **DC bias** (\(V_G\)) is applied to a MOS capacitor, the **energy bands of the semiconductor bend**, influencing charge distribution at the oxide-semiconductor interface. The degree of bending determines the operating mode of the MOS capacitor.
#### Why is Flat Band Important?
- It acts as a **reference** to analyze how energy bands shift when \(V_G\) changes.
- In practical devices, \(V_{FB}\) is **rarely zero** due to charges in the oxide or interface traps.

## Operation Modes
There are different modes in which the MOS Capacitor operates in, namely:
#### 1. Accumulation: 
 `A negative gate voltage attracts holes to the interface.` 
If we apply a negative voltage to the gate terminal (lets call this applied voltage as Vg, standing for Gate voltage), due to the capacitive behavior, the positive charges in the semiconductor (holes) will be drawn to the top side of the substrate, near the interface of substrate and oxide. This gathering of multiple positive charges near the interface is why we call it accumulation, but the applied voltage is negative and in small magnitude. Also, attracting positive charge carriers can't really help us creating a path to carry current, because remember, hole is just the vacancy or absence of electron. The capacitance equation relevant here is:
$C ox = εins/d$
#### 2. Depletion
`A small positive voltage repels holes, creating a depletion region.`
Like we discussed in the accumulation discussion, our goal is to manipulate the charge carriers in such a way so as to get a useful application out of it, which is creating a path to carry current, just like a wire, but for that we really need electrons and not holes. So let's invert polarity of the applied external voltage from negative to positive. Doing this will give us a region which is depleted of positive charge carriers i.e. holes and leave behind immobile ions. Remember that these immobile ions cannot contribute to charge movement as they aren't mobile. So, essentially, this region is pretty much devoid of any charge carriers, leaving behind a barren region depleted of mobile charge carriers, which we refer to as the depletion region.
The depletion capacitance varies with voltage and is given by: 

$C dep​ = ε si​ / W$

 $ε si​$ is the permittivity of silicon and $W$ is the depletion width.

#### 3. Inversion
`A sufficiently large positive voltage attracts minority carriers (electrons), forming an inversion layer, mimicking an n-type region."`
Now, if we increase the magnitude of the positive external voltage that we previously applied, it will overcome and start affecting the carriers in the regions beyond the depleted region. This will cause attraction of electrons to the interface now. This turning point where we gain access to regions beyond the depletion region is referred to as the Threshold voltage or Vth. So when the applied Vg becomes greater than the threshold, i.e. Vth, these electrons now give us a path of electron movement in the p-type substrate. It is important to note that we have achieved a significant thing doing this. We are simulating n-type behavior with electrons as majority charge carriers in a originally p-type substrate, which has holes as majority charge carriers. This very fact will be crucial towards the understanding of how MOSFETS function and help us change and manipulate this behavior in the substrate.
