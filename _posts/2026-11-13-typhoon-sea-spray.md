---
layout: post
title: "Typhoon Generated Sea Spray (Numerical Model, Python)"
author: "Brandon Kerns"
categories: GIS,Modeling
tags: [example,winds,map,gis,modeling]
image: mspr_3d_with_wind.2025092318.png
---
# Typhoon generated sea spray

![Alt text describing the animation]({{ '/assets/img/mspr_3d_with_wind.ANIM.gif' | relative_url }})

## Why care?

Offshore energy infrastructure, in particular wind farms, are exposed to salt from sea spray, and this is corrosive to the materials used to construct the infrastructure. It is not practical to fully protect the infrastructure from this. Often, assumptions of sea spray load are made using seasonal statistics. However, severe storms like typhoons and strong winter cold waves can increase the load beyond what is expected during a typical season. Therefore, direct prediction of sea spray can help optimize the maintenance of these offshore facilities.

## Data used

- Model initial and boundary conditions:
  - ERA-5 analysis
  - Copernicus Mercator ocean analysis
  - Offshore wind turbine coordinates from Open Street Maps

## Tools used

- UWIN-CM, a Coupled atmosphere-wave-ocean model with an interactive sea spray module.
- Offshore wind turibine locations were aggregated into wind farms using Python.
- Python to generate plots.
- Imagemagick to generate animations using the static images.
