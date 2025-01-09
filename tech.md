---
layout: document
---

{% assign cacheBust = site.time | date:'?v=%s' %}

# [HexTrack](/)<br>Technical Documentation
{: .no_toc}

![Image]({{ "/images/hextrack-3D_blender_angled.png" | absolute_url | append: cacheBust }})

<!-- [![ZMK Build](https://github.com/tmshader/hextrack/actions/workflows/build.yml/badge.svg)](https://github.com/tmshader/hextrack/actions/workflows/build.yml)

[![Pages Build](https://github.com/tmshader/hextrack/actions/workflows/kibot.yml/badge.svg)](https://github.com/tmshader/hextrack/actions/workflows/kibot.yml)

[![GitHub last commit](https://img.shields.io/github/last-commit/tmshader/hextrack)](https://github.com/tmshader/hextrack) -->

## Table of contents
{: .no_toc}

* TOC
{:toc}

---

## Renders

### Render Angled

![Image]({{ "/images/hextrack-3D_blender_angled.png" | absolute_url | append: cacheBust }})

### Render Top

![Image]({{ "/images/hextrack-3D_blender_top.png" | absolute_url | append: cacheBust }})

### Render Bottom

![Image]({{ "/images/hextrack-3D_blender_bottom.png" | absolute_url | append: cacheBust }})

## Schematic

### Monochrome

- [Schematic Monochrome PDF]({{ "/documents/hextrack-schematic-mono.pdf" | absolute_url | append: cacheBust }})

### Light

- [Schematic Light PDF]({{ "/documents/hextrack-schematic-default.pdf" | absolute_url | append: cacheBust }})

## Assembly

### Assembly document

- [Assembly PDF]({{ "/documents/hextrack-assembly.pdf" | absolute_url | append: cacheBust }})

### Fabrication document

- [Fabrication PDF]({{ "/documents/hextrack-fabrication.pdf" | absolute_url | append: cacheBust }})

## Gerber viewer on tracespace.io

- [JLCPCB Gerber](https://tracespace.io/view/?boardUrl={{ "export/hextrack-JLCPCB.zip" | absolute_url | append: cacheBust }})

## Interactive BOM

Check component locations by hovering over a specific component.
The visual elements might not be precise enough for pcb review but can be very useful since it's possible to pan and zoom.

[IBOM HTML]({{ "/export/hextrack-ibom.html" | absolute_url | append: cacheBust }})

## Downloads

### JLCPCB

- [JLCPCB Zip]({{ "export/hextrack-JLCPCB.zip" | absolute_url | append: cacheBust }})
- [JLCPCB BOM CSV]({{ "export/hextrack_bom_jlc.csv" | absolute_url | append: cacheBust }})
- [JLCPCB CPL CSV]({{ "export/hextrack_cpl_jlc.csv" | absolute_url | append: cacheBust }})


### 3D Step

- [3D Step]({{ "/hextrack-3D.step" | absolute_url | append: cacheBust }})

## Report

### ERC

{% include_relative hextrack-erc_validation.md %}

### DRC

{% include_relative hextrack-drc_validation.md %}

{% include_relative hextrack-report.md %}