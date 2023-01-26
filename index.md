---
title: "Fetal CMR"
tagline: "resources"
layout: single
header:
  overlay_image: /assets/images/fetal_whole_body_and_heart_render.jpg
  image_description: "transparent rendering of fetal body and heart"
  caption: "image courtesy DFA Lloyd, A Davidson, T Zhang. [ifindproject](http://www.ifindproject.com/)"
  actions:
    - label: "contribute"
      url: "#contribute"
toc: true
toc_sticky: true
sidebar:
  - title: "Fetal CMR Resources"
    text: "a list of technical resources for fetal cardiac magnetic resonance imaging put together by the [SCMR Fetal CMR and CMR in Pregnancy Special Interest Group](https://scmr.org/members/group.aspx?id=210568)"
last_modified_at: 2021-04-23T22:00:00-04:00
---

## Webinars

**SCMR Fetal CMR and CMR Pregnancy Special Interest Group**

Apr 9, 2021 – [Fetal Cardiac MRI: Center Specific Experience](https://www.youtube.com/watch?v=UhfaYKHAAk0)  

Oct 8, 2021 – [Fetal CMR: “What’s in my exam card?” A practical guide to acquisition and post-processing methods](youtube.com/watch?v=xkbEyGDhR08)  

**Northh Medical**

2023 Webinar Series – [Fetal Cardiac Imaging Using MRI](https://www.northh.de/webinar-registration)  



## MOG

MOG – metric optimized gating

<img src="https://avatars.githubusercontent.com/u/6586743" alt="MOG logo" title="MOG" class="align-right" style="height:auto;max-height:25vh;max-width:40vh;"  />

[github.com/metricOptimizedGating](https://github.com/metricOptimizedGating)

_retrospective image-based cardiac gating for segmented acquisitions using entropy-based metrics to guide data consistency in reconstructed balanced steady state free precession (bSSFP) and phase contrast (PC) MR images_

**2D Cartesian cine bSSFP and PC MR**

[metricoptimizedgating.github.io/MOG-Public](http://metricoptimizedgating.github.io/MOG-Public/)

* anatomical and cine imaging using standard vendor 2D phase contrast MR sequences
* MOG algorithm adjusts timing of each measurement (k-space line) according to metric optimized heart rate
* read±write of [Siemens TWIX (.dat)](https://github.com/MetricOptimizedGating/MOG-Public#-2) and [Philips (.data/.list)](https://github.com/jfpva/MOG-Philips) raw data implemented

**2D radial PC MR**

* golden angle radial 2D PC MR sequence available via [Siemens C<sup>2</sup>P Exchange](https://webclient.ca.api.teamplay.siemens.com/#/c2p)
* ICE tools included with sequence to generate time-averaged magnitude image on the scanner console
* offline tools to perform motion-corrected, time-resolved MOG reconstruction to be open source in future; currently available on request

**2D radial Cine bSSFP**

* tiny golden angle radial 2D SSFP sequence available via [Siemens C<sup>2</sup>P Exchange](https://webclient.ca.api.teamplay.siemens.com/#/c2p)
* ICE tools generate time-averaged magnitude image for each slice in stack
* offline tools to perform motion-corrected, time-resolved MOG reconstruction to be open source in future; currently available on request

## Smart-Sync

_smart-sync_ – Doppler ultrasound gating device

<img src="https://static.wixstatic.com/media/a1f87e_05a156cf02fe4491be0da164ffd8c613~mv2.png" alt="northh smart-sync Doppler ultrasound gating device sensor box display" title="northh smart-sync device" class="align-right" style="height:auto;max-height:25vh;max-width:40vh;"  />

[northh.de](https://www.northh.de/)

_MR-compatible Doppler ultrasound system for synchronization of image acquisition with the fetal cardiac cycle_

* enables the use of standard cardiac-gated MR sequences for assessment of anatomy and function
* compatible with Siemens, GE and Philips 1.5T and 3T MR systems

## SVRTK

SVRTK – slice-to-volume reconstruction toolkit

<img src="https://svrtk.github.io/SVRTKlogo.png" alt="SVRTK logo" title="SVRTK" class="align-right" style="height:auto;max-height:25vh;max-width:40vh;"  />

[svrtk.github.io](https://svrtk.github.io/)

_slice-to-volume reconstruction package for fetal MRI motion correction and volumetric super-resolution reconstruction from stacks of 2D MR images_

* includes
    * SVR – original method using rigid slice-to-volume registration
    * DSVR – deformable slice-to-volume registration
    * 4D SVR – volumetric reconstruction resolved for cardiac phase (cine)
    * 4D Flow SVR – cine cardiovascular anatomy and flow volume reconstruction
* features
    * MITK-based graphical user interface
    * Docker image of compiled toolkit
    * automated segmentation and localization
* related repos
    * fetal whole-heart 4D magnitude and flow cine reconstruction using multiple real-time non-coplanar balanced SSFP stacks – [github.com/mriphysics/fetal_cmr_4d](https://github.com/mriphysics/fetal_cmr_4d)


## Blood Oximetry

_quantification of blood oxygen saturation using MRI-based T1 and T2 measurements_

* magnetization-prepared 2D balanced SSFP sequence for quantification of T1 and T2 of blood in large vessels available via [Siemens C<sup>2</sup>P Exchange](https://webclient.ca.api.teamplay.siemens.com/#/c2p)
* a series of T1- or T2-weighted images are generated on the scanner, which can then be used to fit for the relaxation time


## Contribute

This page is maintained by Joshua van Amerom, Thomas Roberts and Eric Schrauben.

To contribute content or suggest changes, please <a href='mailto:joshua.vanamerom@sickkids.ca,t.roberts@kcl.ac.uk,e.m.schrauben@amsterdamumc.nl?subject=Fetal%20CMR%20Resources%20fetalcmr.github.io'>email us</a> or submit a pull request to [this git repo](https://github.com/fetalcmr/fetalcmr.github.io/blob/main/CONTRIBUTING.md).
