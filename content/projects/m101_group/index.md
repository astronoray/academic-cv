---
title: "M101 Group: Galaxy Evolution in a Nearby Laboratory"
date: 2026-08-09
# links:
#   - type: site
#     url: https://github.com/pandas-dev/pandas
authors:
  - me

image:
  caption: 'Image credit: [Davide Casiraghi - Astrobin](https://app.astrobin.com/i/tn5dx5)'

tags:
  - M101
  - NGC 5474
  - galaxy evolution
  - galaxy interactions
  - HII regions
  - abundances
  - stellar populations
  - spiral structure
  - thesis
---

I have focused on the M101 Group since graduate school. Because it is only a few megaparsecs away, this small, isolated galaxy group gives us a detailed look at how spiral galaxies form and change. We can study star formation in individual H&nbsp;<span style='font-size: 0.8em;'>II</span> regions, map chemical abundances across a whole galactic disk, use stellar populations to trace spiral structure and interactions, and examine neighboring galaxies as part of the same dynamic system.

I started studying M101 by asking: how much star formation happens beyond the bright optical disks of galaxies? This question led me to explore how M101 has grown, changed chemically, responded to its surroundings, and interacted with its satellites, especially the unusual galaxy NGC 5474.

In this research, I have used deep, wide-field imaging, long-slit and integral field spectroscopy, nebular abundance measurements, stellar population modeling, and multiwavelength analysis. Each finding led to new questions. The M101 Group has been both a laboratory and a foundation for shaping how I study galaxy evolution.

## Why M101?

M101, or the Pinwheel Galaxy, is a large, nearby spiral galaxy seen face-on. Its disk is noticeably asymmetric, featuring a "big wonky arm." The outer spiral structure looks disturbed, and its largest satellite, NGC 5474, is also unusual, with a bright central bulge that is clearly offset from the center of its underlying disk.

These features have suggested for some time that M101 and NGC 5474 recently interacted. However, the system is puzzling: its shape looks disturbed, but other signs of a strong interaction are unexpectedly subtle.

These questions have motivated much of my research. What effects does a weak tidal interaction have on a large spiral galaxy? Where should we look for its signs: in current star formation, chemical abundances, stellar ages, spiral structure, or satellite dynamics? And how long do these signs last?

{{< figure
    src="m101-group.jpg"
    alt="View of the M101 Group. M101 is at the center, with its asymmetric spiral arms and numerous pink star-forming regions. NGC 5474 is to the bottom left with its offset bulge clearly visible to the north of a face-on spiral disk. Another M101 satellite, NGC 5477, is immediately to the left of M101; a small irregularly shaped galaxy. Numerous other background galaxies and foreground stars dot the image."
    caption="The M101 Group provides a nearby laboratory for studying spiral structure, satellite interactions, chemical evolution, and star formation."
    attr="Image credit: Doublas Rollain - Astrobin"
    attrlink="https://app.astrobin.com/i/580z7j"
>}}

## Searching for Star Formation Beyond the Optical Disk

For my first major M101 project, I used deep, wide-field narrowband imaging from the Burrell Schmidt telescope to search about 6 square degrees around the group for very faint areas of ongoing star formation.

We focused on H&alpha;, H&beta;, and [O&nbsp;<span style='font-size: 0.8em;'>III</span>] emission lines and created a method to distinguish real emission-line sources apart from foreground stars and background galaxies. Our goal was to find isolated H&nbsp;<span style='font-size: 0.8em;'>II</span> regions or new star-forming dwarf galaxies that could mark tidal material from an encounter between M101 and its companions.

The surprising result was largely a null detection. Nearly all of our candidates were associated with the extreme outer disk of M101 rather than a widespread intragroup population. Only two unusual objects were associated with other systems: an outlying H&nbsp;<span style='font-size: 0.8em;'>II</span> region near NGC 5474 and a star-forming object belonging to a background galaxy NGC 5486. 

{{< figure
    src="ngc5474_5486_detail.png"
    alt="A two-by-two grid of images. The top row focuses on NGC 5474 and the bottom row focuses on NGC 5486. The left column shows an H-alpha image and the right column shows a broadband image."
    caption="A zoomed-in view of the detected regions near NGC 5474 (top row) and NGC 5486 (bottom row). Left: the continuum-subtracted H&alpha; image. Right: the broadband *B* image, stretched to show the faint structure of the outer disks. The red circle represents the size of a galaxy mask. The orange circle is an object detected in all three narrowband images, while the green circle is an object detected in the H&alpha; and [O&nbsp;<span style='font-size: 0.8em;'>III</span>] image. "
    attr=" Figure 9 of Garner et al. (2021)"
>}}

Instead of being disappointing, this result changed my perspective on the group. If M101’s obvious asymmetries came from a recent encounter, it seems that event did not spread much star-forming gas into the surrounding area. Or, if it did, the H&alpha; signals we looked for had already faded.

#### What This Work Demonstrated

Through this project, I gained experience with deep optical imaging, careful continuum subtraction, detecting low surface brightness sources, emission-line photometry, building catalogs, rejecting contaminants, following up with spectroscopy, and interpreting null results.

It also taught me an important lesson that has guided my research: not finding an expected signal can still tell us something physical. The lack of intragroup star formation helped narrow down possible interaction histories for the system and encouraged me to search for more subtle signs within the galaxies.

#### Related Publications

- [A Deep Census of Outlying Star Formation in the M101 Group](../../publications/garner2021/)
- [Spectroscopic Follow-up of Two Star-forming Objects in the M101 Field](../../publications//garner2023_rnaas/)


## Chemical Evolution Across M101

If the interaction had not produced large numbers of isolated star-forming regions, perhaps its signature could instead be found in the chemical structure of M101's disk. 

Using an expanded Burrell Schmidt dataset including H&alpha;, H&beta;, [O&nbsp;<span style='font-size: 0.8em;'>III</span>], and [O&nbsp;<span style='font-size: 0.8em;'>II</span>], I measured strong-line oxygen abundances for 720 H&nbsp;<span style='font-size: 0.8em;'>II</span> regions across M101, NGC 5474, and NGC 5477. 

M101 shows the usual drop in metallicity as you move farther from the center, but the full two-dimensional data revealed a more complex situation. The gradient flattens in the outer disk, and H&nbsp;<span style='font-size: 0.8em;'>II</span> regions there show clear azimuthal abundance patterns. These differences from a simple radial gradient mostly appear in parts of the disk that may have been shaped by M101’s interactions with NGC 5474.

{{< figure
    src="m101_break_kk04.png"
    alt="A plot showing a radial trend in HII regions. There is a cluster of points going from the top left at high abundance, low radius to the bottom right at low abundance, high radius."
    caption="The Kobulnicky & Kewley (2004) oxygen abundances of M101 fitted with a simple exponential (dashed black line) and a broken exponential (solid black line). Regions in the turn-around region (orange circles), upper branch (blue triangles), and lower branch (green inverted triangles) are distinguished. Outside 1.3*R*<sub>23</sub>, we display both the upper- and lower-branch solutions connected by a dotted line for each individual H&nbsp;<span style='font-size: 0.8em;'>II</span> region."
    attr=" Figure 10 of Garner et al. (2022)"
>}}

#### What This Work Demonstrated

This project expanded my expertise in nebular astrophysics and chemical evolution, including reddening corrections, emission-line ratios, strong-line abundance diagnostics, metallicity gradients, uncertainty propagation, and spatial statistics. 

More broadly, it taught me to connect local and global views of galaxies. Individual H&nbsp;<span style='font-size: 0.8em;'>II</span> regions show local conditions, but hundreds of these measurements can reveal patterns in chemical enrichment and mixing across kiloparsec scales. Linking the physics of single nebulae to the evolution of their host galaxies became a key theme in my later work.

#### Related Publications

- [Deep Narrowband Photometry of the M101 Group: Strong-line Abundances of 720 HII Regions](../../publications/garner2022/)


## Spiral Dynamics Through Stellar Populations

The same narrowband dataset also held information I had not planned to use. Besides nebular emission, some filters captured age-sensitive stellar absorption features, like Balmer absorption and changes in the continuum near the Balmer and 4000 Å breaks. By comparing these measurements to stellar population models, I developed a way to estimate stellar ages across M101’s disk.

The resulting maps showed the expected trend: younger stars are found farther from the center, which fits with inside-out growth. More interestingly, the stellar ages change in a regular way across spiral arms. In the mostly undisturbed inner disk, these age patterns match what we expect from large-scale spiral shocks. Surprisingly, similar patterns also show up farther out, beyond the expected corotation radius of the main inner spiral.

I saw these results as evidence that M101’s seemingly organized structure may come from several dynamically linked spiral patterns, not just one rigidly rotating spiral density wave.

{{< figure
    src="inner_env.png"
    alt="A plot showing three clusters of colored points, red, green, and blue."
    caption="The equivalent width through the H&beta; filters (*W*<sub>H&beta;</sub>) and [O&nbsp;<span style='font-size: 0.8em;'>II</span>] filters (*W*<sub>3746</sub>) for all pixels in the main disk of M101 distinguished by environment: the inner disk in red, spiral arms in blue, and interarm regions in green."
    attr="Figure 9 of Garner et al. (2024)"
>}}

#### What This Work Demonstrated

For this project, I had to use an observational dataset for a new question it was not meant to answer. I developed techniques for modeling stellar populations, linked narrowband observations to synthetic spectra, made spatial age maps, and interpreted these results in terms of spiral dynamics.

This work expanded my research from studying present-day ionized gas to looking at the stellar fossil record. Gas emission shows what a galaxy is doing now, while stellar populations hold clues about its past. By combining both, we get a much clearer picture of galaxy evolution than by using either one alone.

#### Related Publications

- [A Dynamic Galaxy: Stellar Age Patterns across the Disk of M101](../../publications/garner2024/)


## NGC 5474: A Hidden Galaxy in Plain Sight

My dissertation led me to another question: if an encounter with NGC 5474 helped reshape M101, what happened to NGC 5474 itself?

NGC 5474 has a strange shape. Its bright central part, usually called its 'bulge,' is about a kiloparsec away from the center of its star-forming disk. Some have suggested that this part is not a bulge, but actually a separate dwarf galaxy seen in front of NGC 5474.

With PINGS PPak integral field spectroscopy, I measured the velocity of the stars in the supposed bulge and compared it to the ionized gas velocity in the surrounding disk. The two are offset by about 24 km/s, which gives kinematic evidence that they are separate systems.

{{< figure
    src="n5474_real_v3.jpg"
    alt="An image showing NGC 5474. There is a bright circular region at the center of the image, with a faint spiral disk offset below it."
    caption="An RGB color image of NGC 5474."
    attr="Figure 1 of Garner et al. (2025)"
>}}

This idea was supported by work I supervised with undergraduate researcher Liv Moody, who used the narrowband data to study stellar populations across NGC 5474. The offset bulge is made up mostly of old stars and is different from the surrounding disk. The galaxy’s outer stellar populations also show extra spatial structure that may relate to its interaction history.

This part of the project also marked a change in my role as a researcher. I moved from doing the analysis myself to designing research questions, developing methods, and mentoring another researcher through an independent project.

#### Related Publications

- [When Is a Bulge Not a Bulge? Revealing the Satellite Nature of NGC 5474's Bulge](../../publications/garner2025_5474/)
- [Peculiar Stellar Ages of the Peculiar Dwarf Galaxy NGC 5474](../../publications/moody2025/)

## Returning to M101 with HETDEX

My current work brings me back to M101, but with a very different dataset. The Hobby-Eberly Telescope Dark Energy Experiment (HETDEX) observed M101 using the VIRUS integral field spectrograph, giving us complete spectroscopic coverage of M101’s disk for the first time.

I am using these spectra along with multiwavelength photometry to map the galaxy’s stellar ages, metallicities, star formation history, and both stellar and gas kinematics. This work brings my M101 research full circle. My first projects used individual H&nbsp;<span style='font-size: 0.8em;'>II</span> regions to study the galaxy’s current state. Now, HETDEX lets me compare those signs to the history recorded in the overall stellar population.

#### Related Publications

- [Mapping the Stellar Fossil Record of M101 with HETDEX: Spatially Resolved Ages and Metallicities](../../publications/garner2026_hetdex/)

## The Broad Picture

Taken together, these projects show that galaxy interactions do not always leave just one clear observational sign.

In the M101 Group, signs of dynamical evolution look different depending on which tracer you study:
- The surrounding group contains little widespread intragroup star formation; 
- The disk of M101 contains chemical structure beyond a simple radial gradient;
- Its stellar populations encode both inside-out growth and complex spiral dynamics;
- NGC 5474 contains a dynamically distinct central component and unusual stellar populations;
- The stellar fossil record provides a way to connect these present-day signatures to longer evolutionary timescales. 

This is one of the main lessons I have learned from these projects. Galaxy evolution is complex and happens on many scales and timescales. Features like shape, ionized gas, chemical abundances, stellar populations, and kinematics do not all react to an interaction in the same way or keep its signature for the same length of time. The M101 Group is especially valuable because its closeness lets us study all these tracers together.

## Methods and Expertise

My work on the M101 Group has developed and demonstrated expertise across several areas of observational astronomy: 

**Observational Techniques**:
Deep wide-field imaging &middot; Narrowband imaging &middot; Long-slit spectroscopy &middot; Integral field spectroscopy &middot; Multiwavelength photometry

**Galaxy Evolution**:
Star formation &middot; Galaxy interactions &middot; Spiral structure &middot; Stellar populations &middot; Chemical evolution

**Nebular Astrophysics**:
H&nbsp;<span style='font-size: 0.8em;'>II</span> region identification &middot; Emission-line photometry &middot; Reddening corrections &middot; Strong-line abundances &middot; Metallicity gradients 

**Stellar Populations**:
Synthetic stellar population modeling &middot; Age-sensitive spectral features &middot; Full spectral fitting &middot; Star formation histories &middot; Stellar metallicities

**Data Analysis**:
Python &middot; Astropy &middot; CIGALE &middot; pPXF &middot; Spectral fitting &middot; Image analysis &middot; Catalog construction &middot; Spatially resolved mapping &middot; Statistical modeling 

## Selected Publications

#### First Author Work

- **Garner et al. 2026**: [Mapping the Stellar Fossil Record of M101 with HETDEX: Spatially Resolved Ages and Metallicities](../../publications/garner2026_hetdex/) <br> Spatially resolved stellar ages and metallicities from HETDEX spectroscopy.
- **Garner et al. 2025**: [When Is a Bulge Not a Bulge? Revealing the Satellite Nature of NGC 5474's Bulge](../../publications/garner2025_5474/) <br> Kinematic evidence that the offset bulge of NGC 5474 is a distance stellar system.
- **Garner et al. 2024**: [A Dynamic Galaxy: Stellar Age Patterns across the Disk of M101](../../publications/garner2024/) <br> Using age-sensitive narrowband measurements to trace disk growth and spiral dynamics. 
- **Garner et al. 2023**: [Spectroscopic Follow-up of Two Star-forming Objects in the M101 Field](../../publications//garner2023_rnaas/) <br> Spectroscopic confirmation and interpretation of unusual objects discovered in the original narrowband survey.
- **Garner et al. 2022**: [Deep Narrowband Photometry of the M101 Group: Strong-line Abundances of 720 HII Regions](../../publications/garner2022/) <br> Spatially resolved chemical abundances across M101 and its major satellites.
- **Garner et al. 2021**: [A Deep Census of Outlying Star Formation in the M101 Group](../../publications/garner2021/) <br> Deep search for star formation and low-luminosity galaxies throughout the M101 Group.

#### Collaborative & Mentored Work

- **Moody & Garner 2025**: [Peculiar Stellar Ages of the Peculiar Dwarf Galaxy NGC 5474](../../publications/moody2025/) <br> Undergraduate-led project extending my stellar population methodology to NGC 5474. I mentored the project and contributed to the analysis and physical interpretation. 
- **Watkins et al. 2024**: [Implications on star formation rate indicators from HII regions and diffuse ionized gas in the M101 Group](../../publications/watkins2024/) <br> Collaborative investigation of the origin of diffuse ionized gas using the same deep imaging dataset together with ultraviolet observations and photoionization modeling.

#### Dissertation

- [Investigating the Galactic Evolution of M101 with Deep Narrowband Imaging](../../publications/garner_thesis/) <br> My PhD dissertation brought together the originaly outlying star-formation, chemical abundances, and stellar population studies into a unified investigation of M101 and its group environment. 

## Where This Work Is Going

The M101 Group is still a key part of my research because it lets me connect physical processes measured on many different scales. The methods I developed here can be used beyond M101. Studying nearby galaxies allows us to link detailed nebular physics, stellar populations, chemical abundances, and galactic dynamics in ways we cannot with more distant galaxies. These local relationships can then help us understand galaxies across cosmic time.
