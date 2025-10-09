---
disable-header-and-footer: true
---

# Introduction
The Zeeman effect is a quantum mechanical effect where a molecular energy levels split into several sub-levels when 
transitioning from a higher rotational energy level to a lower one. This effect occur only for molecules whose 
electron spin is different from zero, and that the molecule reside within a external field, such as Earths. 

Most published work in recent years within the context of remote sensing in Earths atmosphere have focused on 
theoretical modeling, satellite observations and ground based observations from mid latitude microwave radiometers.
Observations from high latitude instruments have never measured this effect, until the KIruna Microwave RAdiometer(KIMRA)
was configured to measure oxygen at 235 GHz in 2023. In this study will detailed comparisons between measurements 
and simulations be conducted to characterize this effect.

Microwave measurements of oxygen have been used for decades to retrieve altitude dependent temperature 
profiles. In this study will a investigation be conducted whether the oxygen measurements obtained
with KIMRA, at 235 GHz could be used for retrieval of temperature profiles and this could potentially unlock new and 
exciting studies in Arctic atmospheric sciences.

# Method and data
Microwave radiometers detect radiation emitted when molecules transition from a higher energy state to a lower one. 
Because molecular energy levels are quantized, these transitions occur only at specific wavelengths. As a result, 
the radiometer records distinct spectral lines corresponding to those transitions. Since the Zeeman effect is splitting
the transitional energy levels into sub levels for oxygen will instead several sub lines be measured instead of one 
distinct line. Additionally, the emitted radiation from a molecule affected by the Zeeman effect is polarized circularly along
the magnetic field lines. Therefore will the relation between the local magnetic field and the line of sight of 
the radiometer unveil different sub lines. The polarization components for the emitted radiation can be described 
with *Stokes formalism* for the intensity vector $\bar{I_\nu} = \begin{bmatrix}I, Q, U, V \end{bmatrix}^{T}$. Where
$I$ is the total intensity, $Q$ and $U$ is linear components and $V$ is the circular component

## Characterization of Zeeman sub-lines
One of the topics in this study is characterization of the sub lines observed with KIMRA from the oxygen line 
located at 235 GHz. The transition will, in the case of the 235 GHz line, be split into four $\sigma_{\pm}$ lines and 
two $\pi$ lines.

Due to instrumental limitations, KIMRA can only measure linearly polarized radiation. While the emission is 
intrinsically circularly polarized along magnetic field lines, it appears linearly polarized in the perpendicular 
plane: horizontally for the $\sigma_{\pm}$ lines and vertically (parallel to the field) for the $\pi$ lines.

On January 4, 2024, four KIMRA measurements were carried out in the cardinal directions. Based on the polarization 
geometry, $\sigma_{\pm}$ lines are expected when pointing North and South, while East and West orientations should 
reveal the $\pi$ lines. Characterization is done by comparisons between simulations and the measurements, where 
minimization of the RMS error is sought when varying the linear polarization component $Q$ in the simulation to 
find the value of $Q$ that best reflect the measurements for each direction.

## Temperature profiling investigation
Investigation whether the oxygen line measured with KIMRA is suitable for temperature retrieval is done by retriving
temperature from a simulated spectra. As a reference is the same done for a oxygen line centered at 53 GHz, 
which have been used by colleagues at Bern university for retrieval of temperature since 2013.

The key property considering retrieval of temperature, is how sensitive the spectra is to change in 
temperature. This is calculated during the retrieval process, and come as a matrix, called the Jacobian matrix. By 
comparing the matricies from retrievals on 53 and 235 GHz lines respectively a determination whether the 
235 GHz line is feasible to use for temperature retrievals.

# Results
RMS minimization between measured and simulated spectra provided consistent values for the $Q$ component, 
especially in the northward ($Q=0.87$) and southward ($Q=0.89$) directions, which align with expectations based on 
the line of sight and local magnetic field. Eastward and westward measurements, however, gave $Q=-0.63$ and $Q=-1$. 
While the sign change of $Q$ is expected, the magnitude difference indicates additional influences that warrant 
further investigation.

Temperature profiling analysis, based on Jacobian matrices from the 53 GHz and 235 GHz retrievals, further highlighted 
key findings. The 53 GHz line showed strong sensitivity to temperature variations across most of the atmosphere, 
confirming its reliability for retrievals. In contrast, the 235 GHz line displayed very low sensitivity at all 
pressure levels, making temperature retrievals unfeasible. 

# Conclusion
Minimizing the RMS to estimate the linear polarization component produced reliable results, particularly for northward 
and southward measurements, confirming the method’s robustness. The east–west discrepancies likely stem from two 
sources: geomagnetic disturbances caused by the world’s largest iron ore deposits near Kiruna, and cross-polarization 
leakage from KIMRA’s optics.

The most significant finding of the temperature profiling analysis is that retrievals from the 235 GHz line are 
unfeasible. While the cause lies outside this study’s scope, the most probable explanation is that KIMRA measures a 
rare isotopologue of molecular oxygen, comprising less than 0.4% of atmospheric oxygen.



