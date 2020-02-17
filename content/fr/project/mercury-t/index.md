---
title: Mercury-T
summary: Un code pour étudier les systèmes multi-planétaires en évolution constante.
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

Mercury-T est basé sur le code à N corps Mercury [(Chambers 1999)](https://ui.adsabs.harvard.edu/abs/1999MNRAS.304..793C/abstract). Grâce à Christophe Cossou, il est disponible en fortran 90 [(Mercury in f90)](https://mercury-90.googlecode.com/archive/master.tar.gz)

{{% figure src="mercury-t.jpg" caption="" class="figure-img img-fluid img-thumbnail border-0 float-right" width="300px" %}}

Il nous permet de calculer l'évolution de l'axe semi-majeur, l'excentricité, l'inclinaison, la période de rotation et l'obliquité des planètes ainsi que l'évolution de la période de rotation du corps hôte.

Ce code est flexible dans la mesure où il permet de calculer l'évolution des marées des systèmes en orbite autour de tout objet non évolutif (à condition de connaître sa masse, son rayon, son facteur de dissipation et sa période de rotation), mais aussi les naines brunes évolutives (BD) de masse entre 0,01 et 0,08 M⊙, une naine M évolutive de 0,1 M⊙, une étoile semblable au Soleil en évolution et un Jupiter en évolution.

Les traces d'évolution de ces corps proviennent des travaux de [Leconte et al. (2011)](https://ui.adsabs.harvard.edu/abs/2011A%26A...528A..41L/abstract) pour les naines brunes, [Chabrier & Baraffe (1997)](https://ui.adsabs.harvard.edu/abs/1997A%26A...327.1039C/abstract); [Baraffe et al. (1998)](https://ui.adsabs.harvard.edu/abs/1998A%26A...337..403B/abstract) pour la naine M de 0,1 M⊙, et [Leconte & Chabrier (2013)](https://ui.adsabs.harvard.edu/abs/2013NatGe...6..347L/abstract) pour Jupiter.


