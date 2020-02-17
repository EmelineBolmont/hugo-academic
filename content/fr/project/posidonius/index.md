---
title: Posidonius
summary: Un code plus rapide, plus fiable et plus générique pour étudier les systèmes multi-planétaires en évolution constante.
tags:
- N-Body code
date: "2020-02-17T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Posidonius
  focal_point: Smart
  preview_only: True
  
links:
- icon: ads
  icon_pack: ai
  name: Blanco-Cuaresma & Bolmont 2017
  url: https://ui.adsabs.harvard.edu/abs/2017ewas.confE...8B/abstract
url_project: "https://www.blancocuaresma.com/s/posidonius"
url_code: "https://github.com/marblestation/posidonius"
url_pdf: ""
url_slides: ""
url_video: ""

---

Posidonius est un code à N corps pour simuler des systèmes planétaires et / ou binaires qui implémente l'intégrateur WHFAST [(Rein & Tamayo 2015)](https://ui.adsabs.harvard.edu/abs/2015MNRAS.452..376R/abstract) et le modèle de marée utilisé dans Mercury-T [(Bolmont et al. 2015)](https://ui.adsabs.harvard.edu/abs/2015A%26A...583A.116B/abstract).

{{% figure src="posidonius.jpg" caption="" class="figure-img img-fluid img-thumbnail border-0 float-right" width="200px" %}}


# La Physique

Comme pour Mercury-T, les corps de la simulation peuvent être statiques ou suivre des modèles évolutifs prédéfinis correspondant aux étoiles FGKML et aux planètes gazeuses. Les simulations peuvent représenter plusieurs effets différents:

- Forces de marée
- Effets d'aplatissement rotationnel
- Corrections générales de la relativité
- Posidonius a une meilleure intégration de spin que Mercury-T, il est plus de six fois plus rapide, il conserve le moment angulaire total du système un ordre de grandeur mieux et le spin à l'évolution d'engraissement par rotation cinq ordres de grandeur mieux.

Il permet également une plus grande variété de configurations. Par exemple, il peut simuler l'évolution d'étoiles binaires en évolution avec des planètes ou une planète de masse Jupiter en évolution autour d'une étoile en évolution.

# La Technologie
 
Le code N-body est écrit en Rust, un langage de programmation système qui fonctionne aussi vite que Fortran / C, empêche les erreurs de segmentation et garantit la sécurité des threads. Ses principales caractéristiques sont:

- Abstractions à coût nul
- Sécurité de la mémoire garantie
- Threads sans data races

Les avantages de Rust pour la communauté astronomique ont déjà été exposés dans [Blanco-Cuaresma & Bolmont 2017](https://ui.adsabs.harvard.edu/abs/2017IAUS..325..341B/abstract). Posidonius fournit également un package Python pour définir facilement des cas de simulation au format JSON, qui peut être lu par l'intégrateur Posidonius et garantit la reproductibilité.
