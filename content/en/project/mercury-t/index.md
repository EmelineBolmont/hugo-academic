---
title: Mercury-T
summary: A code to study tidally evolving multi-planet systems.
tags:
- N-Body code
date: "2020-02-17T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Mercury-T
  focal_point: Smart
  preview_only: True

links:
- icon: ads
  icon_pack: ai
  name: Bolmont et al. 2015
  url: https://ui.adsabs.harvard.edu/abs/2015A%26A...583A.116B/abstract
url_code: "https://github.com/EmelineBolmont/mercury-90/archive/tides.zip"
url_pdf: "https://www.dropbox.com/s/3sj64x6g28r9ub7/Mercury_manual.pdf?dl=0"
url_slides: ""
url_video: ""

---

Mercury-T is based on the N-body code Mercury [(Chambers 1999)](https://ui.adsabs.harvard.edu/abs/1999MNRAS.304..793C/abstract). Thanks to Christophe Cossou, it is now in fortran 90 [(Mercury in f90)](https://mercury-90.googlecode.com/archive/master.tar.gz).

{{% figure src="mercury-t.jpg" caption="" class="figure-img img-fluid img-thumbnail border-0 float-right" width="300px" %}}

It allows us to calculate the evolution of semi-major axis, eccentricity, inclination, rotation period and obliquity of the planets as well as the rotation period evolution of the host body. 

This code is flexible in so far as it allows to compute the tidal evolution of systems orbiting any non-evolving object (provided we know its mass, radius, dissipation factor and rotation period), but also evolving brown dwarfs (BDs) of mass between 0.01 and 0.08 M⊙, an evolving M-dwarf of 0.1 M⊙, an evolving Sun-like star, and an evolving Jupiter. 

The evolution tracks of these bodies come from the works of [Leconte et al. (2011)](https://ui.adsabs.harvard.edu/abs/2011A%26A...528A..41L/abstract) for brown dwarfs, [Chabrier & Baraffe (1997)](https://ui.adsabs.harvard.edu/abs/1997A%26A...327.1039C/abstract); [Baraffe et al. (1998)](https://ui.adsabs.harvard.edu/abs/1998A%26A...337..403B/abstract) for the M-dwarf of 0.1 M⊙, and [Leconte & Chabrier (2013)](https://ui.adsabs.harvard.edu/abs/2013NatGe...6..347L/abstract) for Jupiter. 
