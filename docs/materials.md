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
- damage tolerance.toughness Ti-SiC has a 2.71 (1.5% Ti) (Moradgholi et al., 2017) AT ROOM TEMP, SiCp/Al has a 15 (Song et al., 2008), Ni/SiC has a 9.3 (bimodal) (Babu et al., 2022)
- prior aerospace applications
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
