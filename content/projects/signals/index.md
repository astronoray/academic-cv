---
title: "Resolved HII Regions with SIGNALS"
date: 2026-10-08
# links:
#   - type: site
#     url: https://github.com/pandas-dev/pandas
authors:
  - me

image:
  caption: 'The Phantom Galaxy, NGC 628, as seen through SITELLE.'

tags:
  - HII regions
  - SIGNALS
  - iFTS
  - chemical abundances
  - ionization parameter
  - stellar feedback
  - photoionization modeling
  - gas kinematics
  - spatially resolved
---

Nebular emission lines are some of our most powerful tools for studying galaxies. From a handful of bright lines, we routinely estimate properties of star-forming regions (and whole galaxies) such as chemical abundances, ionization parameters, densities, temperatures, dust extinctions, and the source of ionizing radiation. But every one of those estimations depends on assumptions. 

We often assume a geometry for the ionized gas, a relationship between the gas and its ionizing stars, a chemical abundance pattern, or that a spectrum integrated over an H&nbsp;<span style='font-size: 0.8em;'>II</span> region adequately represents everything inside it. Those assumptions become especially important when the same diagnostics are applied to galaxies too distant to resolve. 

My work with the **Star-formation, Ionized Gas, and Nebular Abundances Legacy Survey (SIGNALS)** attempts to answer the question: *What physical information do these lines provide, and when do our assumptions about these diagnostics break down?* 

SIGNALS uses an instrument called SITELLE, a wide-field imaging Fourier transform spectrometer at the Canada-France-Hawaii Telescope (CFHT) to obtain spatially resolved spectroscopy across nearby galaxies. In my mind, SITELLE is the halfway point between narrowband photometry and true integral-field spectroscopy. We take images in particular wavelength ranges (usually targeting bright emission lines), but inside each of those images, we have spectral information. SITELLE's combination of a large field of view and its high spatial resolution makes it possible to study multiple things at once: individual H&nbsp;<span style='font-size: 0.8em;'>II</span> regions, populations of H&nbsp;<span style='font-size: 0.8em;'>II</span> regions across a galaxy, and the larger galactic environments in which those regions form. 

{{< figure
    src="intspec.png"
    alt="A scientific plot showing a spectrum with flux on the vertical axis and wavelength on the horizontal axis. The wavelength increases from left to right with jumps in wavelength where there is no data. The left panel shows one emission line, the middle panel shows three emission lines, and the right panel shows five emission lines. Each line is pointed with jagged wiggles on either side of it."
    caption="An example of a SITELLE spectrum. SITELLE collects data in three filters, targeting the strong optical emission lines. Because it is an imaging Fourier transform spectrometer, SITELLE spectra have a characteristic shape described by a *sincgauss* function rather than a standard Gaussian. Figure 2 in Garner et al. (2026)."
    attrlink=""
>}}

My involvement in SIGNALS has likewise spanned several scales. I have led projects on H&nbsp;<span style='font-size: 0.8em;'>II</span> region diagnostics and giant H&nbsp;<span style='font-size: 0.8em;'>II</span> region structure, contributed methods and analyses to studies as a co-author, obtained new SITELLE observations to pursue my own questions, and participated in the broader scientific organization of the collaboration. 

## Testing the Assumptions Behind Nebular Diagnostics 

Metallicity and ionization parameter are two of the most important quantities used to describe an H&nbsp;<span style='font-size: 0.8em;'>II</span> region. Both strongly affect its emission-line spectrum, and they are often thought to be anti-correlated: as the oxygen abundance increases, the ionization parameter decreases. Yet, numerous investigations have found either no correlation or a positive correlation, sparking renewed interest in how these properties are related. As if to make things worse, published calibrations of the ionization parameter can disagree substantially because they are derived from photoionization models containing different assumptions about stellar populations, chemical abundances, dust, density, and nebular geometry. 

Rather than adopting one of these calibrations, I constructed a custom grid of Cloudy photoionization models and used NebulaBayes to infer oxygen abundance and ionization parameter simultaneously for more than 1,500 H&nbsp;<span style='font-size: 0.8em;'>II</span> regions across the nearby face-on spiral galaxy NGC 628. 

I recovered the expected anti-correlation between oxygen abundance and ionization parameter, but the more important result was how strongly the inferred relationship depended on the assumptions built into the models. The correlation also showed substantial intrinsic scatter, with dust extinction emerging as one secondary variable related to both quantities. 

{{< figure
    src="logU-OH_correlation.png"
    alt="A scientific chart in three panels. The left two panels plot small black points and larger black points with errorbars. There is a black line through most of the larger black points decreasing in slope from left to right with a shaded black band around it. There are other colored lines on the plot also going from left to right of various decreasing slopes. The rightmost panel shows a colorful grid from orange through red to light blue indicating high to low values. Most of the orange grid squares are towards the top of the panel with the blue grid squares at the bottom."
    caption="The ionization parameter (log U) - oxygen abundance (12 + log(O/H)) relation. The left panel shows all H&nbsp;<span style='font-size: 0.8em;'>II</span> regions regardless of signal-to-noise. The middle panel selects only those with a signal-to-noise of at least 15. The right panel shows how the signal-to-noise varies across the plot. The small points are the raw data analyzed through NebulaBayes, which are binned into the larger black points. The black line is a fit to the binned data. Other correlations from the literature are also plotted. Figure 9 in Garner et al. (2025)."
    attrlink=""
>}}

The larger lesson was that a commonly-used diagnostic should not be treated as a black box simply because it has become standard in the literature. Understanding how a calibration was constructed, and whether its assumptions match the observations, is part of making the measurement itself. 

### Developing a Methodology

This combination of a custom Cloudy grid and Bayesian inference was subsequently adapted within SIGNALS to address very different scientific questions. 

In NGC 6946, Bresolin[+Garner] et al. (2025) used this methodology to derive oxygen and nitrogen abundances for hundreds of H&nbsp;<span style='font-size: 0.8em;'>II</span> regions and investigate azimuthal abundance structures across the galaxy. We found an azimuthal variation across one of its spiral arms, together with comparable spatial correlation scales for oxygen and nitrogen. 

{{< figure
    src="bresolin.jpeg"
    alt="A scientific plot showing a black-and-white image of a multi-armed spiral galaxy. On top of the image are dashed black lines outlining the positions of the arms and a circular radial grid. Colored points are scattered around some of the arms, going from red (high abundance) to purple (low abundance)."
    caption="Oxygen abundance variations across the spiral arms of NGC 6946. Along the top left arm, the oxygen abundances grow more metal poor as you move from one side of the arm to the other. Figure 7 in Bresolin et al. (2025)."
    attrlink=""
>}}

This methodology has now also been extended again by González-Koda[+Garner] et al. to investigate the N/O-O/H relation for galaxies occupying different parts of the cosmic large-scale structure. 

#### Related Publications

- [NGC 628 in SIGNALS: Explaining the Abundance-Ionization Correlation in H&nbsp;<span style='font-size: 0.8em;'>II</span> Regions](../../publications/garner2025_signals/)
- [SIGNALS on the mixing of oxygen and nitrogen in the spiral galaxy NGC 6946](../../publications/bresolin2025/)
- [The N/O-O/H relation across different large-scale environments](../../publications/gonzalezkoda2026/)

## Spatially-Resolved H&nbsp;<span style='font-size: 0.8em;'>II</span> Regions

My next lead SIGNALS project approached the same problem from the opposite direction: rather than study thousands of H&nbsp;<span style='font-size: 0.8em;'>II</span> regions as individual objects, I asked what happened when we resolve one H&nbsp;<span style='font-size: 0.8em;'>II</span> region internally. 

NGC 604 in M33 is the most luminous H&nbsp;<span style='font-size: 0.8em;'>II</span> region in that galaxy and one of the largest star-forming complexes in the Local Group. At the distance of M33, the SIGNALS observations provide a physical resolution of only a few parsecs. At that scale, the assumptions behind integrated nebular diagnostics can be examined directly. 

{{< figure
    src="pretty_images_ann.png"
    alt="A three-panel scientific image showing a nebula. In the left panel, stars dot the image with the nebula in colors of white and purple. The middle panel has no stars, with just the nebula in darker purple. The right panel is the same as the left but with red drawings and white annotations marking particular features. Several loops, bubbles, and filaments can be seen."
    caption="The giant H&nbsp;<span style='font-size: 0.8em;'>II</span> region NGC 604 as seen through SITELLE. The left panel shows the deep image formed by summing all three filters together. The middle panel shows an RGB image of the gas emission lines H&alpha;, [O&nbsp;<span style='font-size: 0.8em;'>III</span>], and [O&nbsp;<span style='font-size: 0.8em;'>II</span>]. The right panel is the same as the middle, but with particular features annotated, including four known bubbles (A-D), and the locations of a supernova remnant and planetary nebula. Figure 1 in Garner et al. (2026)."
    attrlink=""
>}}

I mapped the principal optical emission-line rations across the entire nebula and found enormous spatial variations in diagnostics normally used to infer ionization parameter and chemical abundance. Those variations do not primarily trace chemical inhomogeneities. Instead, they closely follow the positions of the massive stellar populations and the shells, cavities, and filaments that those stars have carved into the surrounding gas. 

In other words, applying an integrated H&nbsp;<span style='font-size: 0.8em;'>II</span> region calibration pixel-by-pixel can return apparently dramatic changes in "metallicity" that are actually changes in ionization structure and geometry. 

The resolved data also revealed sources that effectively disappear when the nebula is integrated into one spectrum, including a known supernova remnant and a previously unidentified planetary nebula. 

The basic problem is therefore not simply spatial resolution for its own sake. It is understanding what information survives when complex physical structure is compressed into the single spectrum we usually observe. 

#### Related Publications

- [SIGNALS of Giant H&nbsp;<span style='font-size: 0.8em;'>II</span> Regions: A Spatially Resolved Analysis of NGC 604](../../publications/garner2026_n604/)

## Stellar Feedback Kinematics

The original SITELLE data were excellent for mapping excitation and ionization, but the H&alpha; profiles showed evidence that multiple kinematic components were unresolved. That immediately suggested a next observation: observe the same nebula at substantially higher spectral resolution. 

I led a successful CFHT proposal for new SITELLE SN4 observations at *R* &#8764; 10,000, designed specifically to resolve the ionized gas kinematics of NGC 604. 

{{< figure
    src="NGC604-Doppler.jpg"
    alt="A color image of a nebula. Parts of the nebula are in blue and orange. Numerous loops, bubbles, and filamentary structures can be seen. "
    caption="The giant H&nbsp;<span style='font-size: 0.8em;'>II</span> region NGC 604 in high-resolution. This is a *Doppler image*, meaning the blue colors correspond to blueshifted velocities (i.e., gas moving toward us), and the orange colors correspond to redshifted velocities (i.e., gas moving away from us). Courtesy of Laurent Drissen."
    attrlink=""
>}}

The new spectra allow me to fit multiple velocity components across the nebula and construct maps of velocity, velocity dispersion, and kinematic complexity. After removing the large-scale rotation of M33, the residual velocity field contains coherent structures associated with the nebula itself. I am now asking how those gas motions relate to the ionization structure measured in the original SIGNALS observations. 

To do this, I have used structure functions, spatial correlation measurements, and cross-comparisons of the resolved maps to quantify characterstic spatial scales. The velocity residuals and velocity dispersion show structure on smaller scales than several ionization-sensitive line ratios, suggesting that the morphology of the radiation field and the motions of the gas do not simply trace one another. 

This work has developed into a collaboration with researchers at Aix-Marseille Université, where we can compare NGC 604 with SITELLE observations of Milky Way H&nbsp;<span style='font-size: 0.8em;'>II</span> regions at still finer physical resolution. We are attempting to answer the question: *What happens to the physics we infer as an H&nbsp;<span style='font-size: 0.8em;'>II</span> region moves from sub-parsec resolution to a few parsecs?* 

## Galactic Dynamics

I have also led a successful SITELLE proposal targeting NGC 5474, the peculiar dwarf satellite of M101. 

NGC 5474 is scientifically quite different from NGC 604. Instead of resolving one giant H&nbsp;<span style='font-size: 0.8em;'>II</span> region, these observations allow me to investigate ionized gas across a galaxy with an unusual dynamical history, asymmetric structure, and an extended low surface brightness disk. 

{{< figure
    src="NGC5474.png"
    alt="A color image of a galaxy. The galaxy shows a faint white featureless disk on top of which are numerous red clumps of light. There is also a featureless white circular bulge towards the top of the faint white disk."
    caption="The peculiar dwarf galaxy NGC 5474. Reddish light indicates star-forming regions. Courtesy of Laurent Drissen."
    attrlink=""
>}}

My goal is to use the ionized gas kinematics and H&nbsp;<span style='font-size: 0.8em;'>II</span> region population to ask how the gas responded to both the peculiar offset bulge of NGC 5474 and its interaction history with M101. The wide SITELLE field is also particularly valuable for tracing emission into the galaxy's low surface brightness outskirts. 

## Science in a Collaboration

SIGNALS has also been important to me because it is my first experience with a large collaborative group. 

The survey brings together people studying H&nbsp;<span style='font-size: 0.8em;'>II</span> regions, chemical evolution, diffuse ionized gas, stellar feedback, supernova remnants, planetary nebulae, galactic dynamics, and other features we can trace with ionized gas in nearby galaxies. Working within that environment has allowed me to grow as a researcher. 

In addition to the NGC 6946 and large-scale environment abundance studies, I am a co-author on SIGNALS work examining AGN-ISM interactions in NGC 4258, where spatially resolved excitation and kinematics reveal how the galaxy's jet interacts with the surrounding gas. 

Several additionall projects are currently moving through the publication process, including: 
- a large H&nbsp;<span style='font-size: 0.8em;'>II</span> region catalog for M33 (led by Emma Jarvis); 
- a comparison of H&nbsp;<span style='font-size: 0.8em;'>II</span> region structure using PHANGS-MUSE observations (led by Lorena Aragüete Riesco); 
- and work on the filling factor and dust-filament structure of H&nbsp;<span style='font-size: 0.8em;'>II</span> regions in NGC 628 (also led by Lorena Aragüete Riesco). 

These projects span substantially different science questions, but they share a common need: understanding how resolved nebular structure affects the physical quantities we infer from emission lines. 

## The Broad Picture

The individual projects above address different objects and different physical questions, but they have increasingly converged on the same underlying theme. 
- In NGC 628, I found that even measurements of integrated H&nbsp;<span style='font-size: 0.8em;'>II</span> regions depend strongly on the assumptions used to translate emission-line ratios into physical properties. 
- In NGC 604, I showed that diagnostics that are meaningful for an integrated nebula can become physically misleading when applied to individual pixels. 
- The new NGC 604 observations push this one step further by asking how ionization and gas kinematics are related across physical scales. 
- The broader SIGNALS collaboration then provides populations of H&nbsp;<span style='font-size: 0.8em;'>II</span> regions across many galactic environments with which those ideas can be tested. 

Together, these projects allow me to answer *What physical structure produced this line ratio, and what information survives in the way I have observed it?*

## Methods and Expertise

My work within SIGNALS has developed and demonstrated expertise across several interconnected areas: 

**Nebular astrophysics**
H&nbsp;<span style='font-size: 0.8em;'>II</span> region physics &middot; chemical abundances &middot; ionization parameter &middot; excitation diagnostics &middot; stellar feedback

**Physical modeling**
Cloudy &middot; NebulaBayes &middot; PyNeb

**Spectroscopy**
CFHT/SITELLE &middot; ORCS &middot; multi-component kinematics 

**Spatial analysis**
Resolved emission-line maps &middot; velocity fields &middot; structure functions &middot; correlation lengths

**Statistical methods**
Bayesian inference &middot; Monte Carlo uncertainty propagation

**Research development**
Observing proposal design &middot; collaboration across institutions &middot; mentoring and collaborative analysis

## Selected Publications

#### First Author Work

- **Garner et al. (2026)**: [SIGNALS of Giant H&nbsp;<span style='font-size: 0.8em;'>II</span> Regions: A Spatially Resolved Analysis of NGC 604](../../publications/garner2026_n604) <br> Resolved excitation, ionization, abundance diagnostics, and gas kinematics across one of the Local Group's most luminous H&nbsp;<span style='font-size: 0.8em;'>II</span> regions. 
- **Garner et al. (2025)**: [NGC 628 in SIGNALS: Explaining the Abundance-Ionization Parameter Correlation in H&nbsp;<span style='font-size: 0.8em;'>II</span> Regions](../../publications/garner2025_signals/) <br> A self-consistent photoionization model analysis of more than 1,500 H&nbsp;<span style='font-size: 0.8em;'>II</span> regions, testing both the physical O/H-logU relation and the assumptions behind common calibrations. 

#### Collaborative Work

- **González-Koda et al. (2026)**: [The N/O-O/H relation across different large-scale environments](../../publications/gonzalezkoda2026/) <br> N/O-O/H across cluster, filament, and void environments, extending my photoionization methodology to galaxy environments. 
- **Aragüete Riesco et al. (2026)**: [H&nbsp;<span style='font-size: 0.8em;'>II</span> Region Filling Factors in NGC 628: Luminosity-Size Relation and Connection with PAH Emission](../../publications/aragueteriesco2026/) <br> Investigating the internal gas and dust structure of H&nbsp;<span style='font-size: 0.8em;'>II</span> regions. 
- **Fernández-Arenas et al. (2025)**: [Ionized gas in NGC 4258: Exploring the AGN - Star formation connection](../../publications/fernandezarenas2025/) <br> SIGNALS study of the spatially resolved excitation and kinematics associated with the galaxy's anomalous arms and jet-ISM interaction.
- **Bresolin et al. (2025)**: [SIGNALS on the mixing of oxygen and nitrogen in the spiral galaxy NGC 6946](../../publications/bresolin2025/) <br> The Cloudy + NebulaBayes methodology adapted to study azimuthal abundance variations and metal mixing across NGC 6946. 

## Where This Work Is Going

My long-term goal is to turn the extraordinary spatial information available in nearby H&nbsp;<span style='font-size: 0.8em;'>II</span> regions into a better physical foundation for interpreting nebular spectra everywhere else. 

High-resolution kinematics can determine how stellar feedback structures the gas and whether the characteristic scales of motion correspond to those seen in ionization diagnostics. Comparisons among Milky Way, Local Group, and more distant H&nbsp;<span style='font-size: 0.8em;'>II</span> regions can quantify exactly what information disappears as spatial resolution worsens. 

Broader-wavelength spectroscopy can provide a particularly important test. Direct measurements of temperature-sensitive auroral lines across resolved giant H&nbsp;<span style='font-size: 0.8em;'>II</span> regions would allow the apparent abundance variations predicted by strong-line diagnostics to be compared against the actual temperature and abundance structure of the gas. 

At the same time, the larger SIGNALS sample makes it possible to ask how all of these relationships change with galactic environment: spiral structure, metallicity, star formation rates, interaction history, and location within the host galaxy. 




