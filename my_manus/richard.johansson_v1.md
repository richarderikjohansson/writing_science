---
disable-header-and-footer: true
bibliography: refs.bib
csl: ieee.csl
link-citations: true
footnoes-pretty: true
header-includes:
    - \usepackage{caption}
    - \captionsetup{font=footnotesize}
---

# Introduction
The Zeeman effect occurs when atmospheric molecules interact with Earth’s
magnetic field, causing their emission lines to split into multiple components.
[@zeeman1897]. One of the molecules that is affected by this is molecular
oxygen, measured with the KIruna Microwave RAdiometer(KIMRA) at the Swedish
Institute of Space Physics(IRF) at the 235 GHz oxygen line since 2023.

Until KIMRA's measurements, no high-latitude instrument had ever detected this
effect in Earth’s atmosphere, marking the first successful ground-based
observation of the phenomenon from the Arctic region. 

For decades, microwave measurements of molecular oxygen have been used to
retrieve altitude-dependent temperature profiles in Earth’s atmosphere. In this
study, we investigate whether oxygen observations from KIMRA also can be used
for temperature retrievals, as previously proposed in past studies [@pardo].

The novelty of this work lies in characterizing the Zeeman effect in oxygen
emissions at 235 GHz, something that has never been done from high latitudes
measurements. Furthermore, exploring temperature retrievals from this oxygen
line may unlock new research opportunities using KIMRA data, offering valuable
insights into atmospheric dynamics and temperature variations in the context of
a changing climate.

# Method and data
Radiation from molecules affected by the Zeeman effect is polarized along the
geomagnetic field lines, circularly [@zeeman1897]. While the emission is
intrinsically circularly polarized along magnetic field lines, it appears
linearly polarized in the perpendicular plane: horizontally for the
$\sigma_{\pm}$ lines and vertically (parallel to the field) for $\pi$
lines. 

Stokes formalism can be used to mathematically describe the polarized
emission, represented by the Stokes vector, $\bar{I_\nu} = \begin{bmatrix}I, Q,
U, V \end{bmatrix}^{T}$. Here, $I$, denotes the total intensity, $Q$ and $U$
corresponds to components of linear polarization and $V$ is corresponds to
circular polarization.

## Characterization of sub lines
A central goal of this study is the characterization of sub-lines observed with
KIMRA. For the 235 GHz oxygen line, the emission is split into four
$\sigma_{\pm}$ components and two $\pi$ components due to the Zeeman effect
[@pardo]. To capture this, four KIMRA measurements were carried out along the
cardinal directions on January 4, 2024.

Considering the polarization geometry and the fact that KIMRA can measure only
linear polarization, observation of $\sigma_{\pm}$ lines are expected when
pointing KIMRA North or South, and $\pi$ lines when pointing East or West.

To characterize the Zeeman effect observed in the KIMRA measurements,
simulations are performed in which the linear polarization component Q is
varied. For each cardinal direction, the simulated spectra are compared with
the measurements, and the value of Q that minimizes the Root Mean Square (RMS)
error is determined, representing the observed spectra most accurately.

## Temperature profiling investigation
A second goal in this study is to investigate whether the oxygen line measured
with KIMRA would be suitable for temperature retrievals. This is evaluated
through retrievals of simulated spectra of the oxygen line KIMRA observe. For
comparison, the same procedure be applied to the well-established oxygen line
centered at 53 GHz, which has been used for temperature retrievals for more
than a decade by colleagues at the University of Bern [@bern].

A key factor in temperature retrieval is the sensitivity of the spectral line
to changes in temperature. This sensitivity is quantified during the retrieval
process through the Jacobian matrix, which describes how variations in
temperature affect the observed spectra. By comparing the Jacobian matrices
derived from the 53 GHz and 235 GHz lines, it is possible to assess whether the
235 GHz line is suitable for reliable temperature retrievals.
 
# Results
RMS minimization between measured and simulated spectra provided consistent
values for the $Q$ component, especially in the northward ($Q=0.87$) and
southward ($Q=0.89$) directions, which align with expectations based on the
line of sight of KIMRA and local magnetic field. Eastward and westward
measurements, however, yielded $Q=-0.63$ and $Q=-1$. Although the sign change
of $Q$ is expected, the magnitude difference between eastward and the westward
directions indicates additional influences that warrant further investigation.

Analysis of Jacobian matrices from the 53 GHz and 235 GHz retrievals
highlighted key differences. The 53 GHz line exhibited strong sensitivity to
temperature variations across most of the atmosphere, confirming its
reliability for temperature retrievals. In contrast, the 235 GHz line displayed
very low sensitivity at all pressure levels, making temperature retrievals
unfeasible. Although the cause of this low sensitivity lies beyond the scope of
this study, the finding highlights a noteworthy scientific observation. 

# Conclusion
Minimizing the RMS to estimate the linear polarization component produced
reliable results, particularly for northward and southward measurements,
confirming the method’s robustness. The east- and westward discrepancies likely
stem from two sources: geomagnetic disturbances caused by the world’s largest
iron ore deposits near Kiruna, and cross-polarization leakage from KIMRA’s
optics.

The most striking outcome of the temperature profiling analysis is the
infeasibility of retrieving temperatures from the oxygen line KIMRA is
measuring. While the underlying cause is outside this study’s scope, one
plausible explanation is that KIMRA measures a rare isotopologue of molecular
oxygen, which constitutes less than 0.4% of atmospheric oxygen. This finding
warrants further study to fully understand the underlying reasons and
highlights the unexpected challenges of extending retrievals to
higher-frequency lines.



\newpage
# References



