---
title: Posidonius
summary: A faster, more reliable, more generic code to study tidally evolving multi-planet systems.
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

Posidonius is a N-body code for simulating planetary and/or binary systems which implements the WHFAST integrator [(Rein & Tamayo 2015)](https://ui.adsabs.harvard.edu/abs/2015MNRAS.452..376R/abstract) and the tidal model used in Mercury-T [(Bolmont et al. 2015)](https://ui.adsabs.harvard.edu/abs/2015A%26A...583A.116B/abstract).

{{% figure src="posidonius.jpg" caption="" class="figure-img img-fluid img-thumbnail border-0 float-right" width="200px" %}}

# Physics


Similarly to [Mercury-T](/project/mercury-t/), the bodies in the simulation can be static or follow predefined evolutionary models matching FGKML stars and gaseous planets. The simulations can account for several different effects:

- Tidal forces
- Rotationnal-flattening effects
- General Relativity corrections

Posidonius has a better spin integration than Mercury-T, it's more than six times faster, it conserves the total angular momentum of the system one order of magnitude better and the spin to rotational-fattening evolution five orders of magnitude better.

It also allows a wider variety of configurations. For instance, it can simulate the evolution of evolving binary stars with planets, or an evolving Jupiter mass planet around an evolving star.


# Technology

The N-body code is written in Rust, a systems programming language that runs as fast as Fortran/C, prevents segmentation faults, and guarantees thread safety. Its main characteristics are:

- Zero-cost abstractions
- Guaranteed memory safety
- Threads without data races

Rust benefits for the astronomical community were already exposed in [Blanco-Cuaresma & Bolmont 2017](https://ui.adsabs.harvard.edu/abs/2017IAUS..325..341B/abstract). Posidonius also provides a Python package to easily define simulation cases in JSON format, which can be read by the Posidonius integrator and ensures reproducibility.

