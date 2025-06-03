---
title: G-nom Plugins
summary: Documentation of G-nom plug-ins.
authors:
    - Lucas Koch
date: 2025-06-03
---
# Overview
G-nom core can be expanded by plug-ins available for both front- and backend. There are two types of plugi-ns:

1. Core plug-ins: These plug-ins are provided with G-nom and enabled by default. They can be disabled using feature flags in your configuration files.
2. Community plug-ins: These plug-ins are maintained by contributors from the G-nom community of the G-nom core team. They are not bundled with G-nom Core and need to be installed separately.

# Core plug-ins
| Name | Description | Integrates | Status |
| ----------- | ----------- | ----------- |  ----------- |
| taXaminer dashboard | Adds functionality to import and store assembly-level analyses produced by taXaminer. Adds a new section to the assembly page embedding the [taXaminer dashboard](https://github.com/BIONF/taxaminer-dashboard). | Genomic annotation, genome browser | ✅ stable |
| taXsun | Adds functionality to link taxSun information from taXaminer analyses and display them on the assembly overview page. | Taxonomy | under development |
