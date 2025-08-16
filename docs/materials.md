Aerospace heat shield material focus right now is on the following:
Ti matrix and SiC fibre MMC (Ti/SiC) 
. reinforced with continuous SiC fibres w/ titanium matrix. [nickname Ti/SiC]
SiCp/Al
. reinforeced with silicon carbide particles w/ aluminium matrix. [nickname SiCp/Al]
Ni/SiC 
. reinforced with silicon carbide particles w/ nickel alloy matrix. [nickname Ni/SiC] 

Still need to search for the following information for each material:
- Tm SiCp/Al has 660C melting point (Fan et al., 2005) but SiCp does not melt, Ti/SiC 1668C (Rahman et al., 2017), Ni/SiC has 964C (Shi et al., 2020)
- thermal conductivity Ti-SiC has a 3.6 (Turner et al., 1993), SiC/Al has a 174 (Chu et al., 2009), Ni/SiC has a 12.6 (Anwar et al., 2021)
- expansion coefficient Ti/SiC has a 9 (BULK) 8.9 (NEUTRON DIFF) 8.6 (A-AXIS) 9.7 (C-AXIS) (Barsoum et al., 1999), SiCp/Al has a 4.7 (Kim et al., 2001) Ni/SiC has a 17 (Berthod et al., 2012)
- damage tolerance.toughness Ti-SiC has a 2.71 (1.5% Ti) (Moradgholi et al., 2017) AT ROOM TEMP, SiCp/Al has a 15 (Song et al., 2008) AT ROOM TEMP, Ni/SiC has a 9.3 (bimodal) (Babu et al., 2022) AT ROOM TEMP
- prior aerospace applications, TiSiC is used in aircraft engines for compressor rotors and high-temperature components, in airframe structural parts such as actuators, exhaust links, struts, ducts, and airfoils, and in applications requiring weight reduction, high-temperature operation, and resistance to low cycle fatigue and fatigue crack growth along the fiber direction (Singerman et al., 1996), SiCp/Al is used in optical mirror substrates for satellites, airborne optoelectronic platforms, space-based optomechanical structures, satellite and pilotless aircraft components, electronic packaging, heat sinks, supports for optical instruments, components for vibration-sensitive equipment, lightweight high-stiffness automotive parts, missile and aircraft structural components (Cui et al., 2008), Ni/SiC is used in internal combustion engine parts such as cylinders and pistons (USC Technologies, n.d.), also used in inhibiting corrosion (Li et al., 2021)
- layer thickness 3mm
Understanding these properties will inform the sim parameters and improve prediction of the failure mechanisms under thermal/mechanical stresses typical of spacecraft heat shield environments upon re-entry.

Thermal stress calculations: 
σ=E⋅α⋅ΔT
E = young modulus 
α = thermal expansion coeff

Initial temperature [T-Initial] = 2.7K (Lea, 2022)
Peak temperature (re-entry temperature) [T-final] = 1650C = 1923.15K
ΔT = 1923.15 - 2.7 = 1920.35

Ti/SiC thermal stress
Young modulus = 157.4GPa = 157.4 x 10^9 (transverse - causes most of the stress because resistance happens mostly along the length of the fibres) (Mahmoodi et al., 2010)
σ = 157.4 x 10^9 x 9 x 10^-6 x 1920.35
σ = 2.72036781 x 10^9

SiCp/Al thermal stress
Young modulus = 194GPa = 194 x 10^9 (Montoya-Dávila et al., 2010)
σ = 194 x 10^9 x 9 x 10^-6 x 1920.35
σ = 3.3529311 x 10^9 

Ni/SiC thermal stress 
Young modulus = 240GPa = 240 x 10^9 (Bajwa et al., 2016)
σ = 240 x 10^9 x 9 10^-6 x 1920.35
σ = 4.147956 x 10^9

All materials will be modelled in bulk for consistency, directional effects will not be included yet.

Density Ti/SiC
Ti₃SiC₂ ≈ 4.44 g/cm3
SiC ≈ 3.21 g/cm3
TiSiC (1.5% Ti) ≈ 3.23 g/cm3 (Du et al., 2025)

Density SiCp/Al
SiCp/Al (10% SiCp) ≈ 2.67 g/cm3 (Mulyadi et al., 2019)

Density Ni/SiC
Ni/SiC ≈ 7.4 g/cm3 (Anwar et al., 2021)

Specific heat capacity Ti/SiC at room temp
540J/kg·K (Barsoum et al., 1999)

Specific heat capacity SiCp/Al at room temp
844.7J/kg·K (Karthikeyan et al., 2011)

Specific heat capacity Ni/SiC at room temp
423J/kg·K (Ma et al., 2016) 

Thermal diffusivity TiSiC
2.04×10−5m2/s (calculated using thermal conductivity, specific heat capacity and density) (Barsoum et al., 1999)


