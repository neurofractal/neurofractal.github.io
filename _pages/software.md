---
layout: archive
title: "Software"
permalink: /software/
author_profile: true
---

{% include base_path %}

## CamKit3D (Python)
[https://github.com/neurofractal/camkit3D](https://github.com/neurofractal/camkit3D)

**Markerless multi-camera 3D motion capture for naturalistic behavioural and neuroscience research.**

CamKit3D turns a handful of ordinary USB webcams into a markerless motion-capture system — no markers, bodysuits or specialist camera hardware required. It covers the full path from raw video to analysed 3D skeleton data:

1. **Record** – capture synchronised video from multiple USB webcams
2. **Synchronise** – align frames across cameras to a common timing grid
3. **2D pose** – extract body keypoints per frame with MediaPipe Pose
4. **3D pose** – triangulate 2D keypoints into 3D world coordinates
5. **Analyse** – orient, plot and animate the 3D skeleton data, or explore it interactively in the browser

CamKit3D runs stand-alone, but can also be synchronised with wearable brain imaging (e.g. OPM-MEG) for naturalistic neuroscience and social interaction research.

```bash
pip install camkit3d
```

See the [documentation](https://github.com/neurofractal/camkit3D/tree/main/docs) for hardware notes, a calibration guide and an end-to-end walkthrough.

## OPM-MEG Tutorials in osl-ephys (Python)
[https://github.com/neurofractal/OPM-oxford/tree/main/tutorials](https://github.com/neurofractal/OPM-oxford/tree/main/tutorials#opm-meg-tutorials-in-osl-ephys)

A step-by-step OPM-MEG analysis pipeline in [osl-ephys](https://github.com/OHBA-analysis/osl-ephys) and MNE-Python, using data from the Oxford OPM-MEG lab (Cerca Magnetics Neuro-1, 64 sensor locations / 192 channels).

**The Four-Motor Task:** the participant hears an audio cue instructing them to move their right arm, left arm, right leg or left leg. Each movement lasts 4 seconds, followed by a variable inter-stimulus interval.

- Data: download from OSF ([osf.io/xh9b6](https://osf.io/xh9b6/)) — see [00_download_data.ipynb](https://github.com/neurofractal/OPM-oxford/blob/main/tutorials/00_download_data.ipynb)
- Note: the tutorials use homogeneous field correction, so please use up-to-date versions of MNE and osl-ephys.

| # | Tutorial | Notebook | Markdown |
|---|----------|----------|----------|
| 1 | Preprocessing | [ipynb](https://github.com/neurofractal/OPM-oxford/blob/main/tutorials/01_OPM_preprocessing.ipynb) | [md](https://github.com/neurofractal/OPM-oxford/blob/main/tutorials/01_OPM_preprocessing.md) |
| 2 | Sensor-level time-frequency analysis | [ipynb](https://github.com/neurofractal/OPM-oxford/blob/main/tutorials/02_sensor_level_TFR.ipynb) | [md](https://github.com/neurofractal/OPM-oxford/blob/main/tutorials/02_sensor_level_TFR.md) |
| 3 | Coregistration (RHINO) | [ipynb](https://github.com/neurofractal/OPM-oxford/blob/main/tutorials/03_rhino_coreg.ipynb) | [md](https://github.com/neurofractal/OPM-oxford/blob/main/tutorials/03_rhino_coreg.md) |
| 4 | Source localisation (LCMV beamformer) | [ipynb](https://github.com/neurofractal/OPM-oxford/blob/main/tutorials/04_OPM_beamforming.ipynb) | [md](https://github.com/neurofractal/OPM-oxford/blob/main/tutorials/04_OPM_beamforming.md) |
| 5 | Parcellation (resting-state data, eyes open/closed) | [ipynb](https://github.com/neurofractal/OPM-oxford/blob/main/tutorials/05_parcellation.ipynb) | [md](https://github.com/neurofractal/OPM-oxford/blob/main/tutorials/05_parcellation.md) |

## OPM Data Analysis Tutorials (MATLAB)
[https://github.com/FIL-OPMEG/tutorials_interference](https://github.com/FIL-OPMEG/tutorials_interference)

Tutorial scripts accompanying [Seymour et al. (2022), *NeuroImage*](https://doi.org/10.1016/j.neuroimage.2021.118834).

1. Auditory evoked field paradigm during participant movement
- Data: [https://doi.org/10.5281/zenodo.5539414](https://doi.org/10.5281/zenodo.5539414)
- Script: [pipeline_tutorial_1.m](https://github.com/FIL-OPMEG/tutorials_interference/blob/main/pipeline_tutorial_1.m)

2. Motor-beta power changes during a finger-tapping paradigm
- Data: [https://doi.org/10.5281/zenodo.5539414](https://doi.org/10.5281/zenodo.5539414)
- Script: [pipeline_tutorial_2.m](https://github.com/FIL-OPMEG/tutorials_interference/blob/main/pipeline_tutorial_2.m)

3. Auditory evoked field paradigm when the participant is sitting still
- Data: [osf.io/vy5n6](https://osf.io/vy5n6/)
- Script: [stationary_AEF.m](https://github.com/FIL-OPMEG/tutorials_interference/blob/main/stationary_AEF.m)

## fBOSC
[https://github.com/neurofractal/fBOSC](https://github.com/neurofractal/fBOSC)

A repository for the robust detection of oscillations at the single-trial level. See [Seymour et al. (2022), *European Journal of Neuroscience*](https://doi.org/10.1111/ejn.15829).

## PACmeg
[https://github.com/neurofractal/pacmeg](https://github.com/neurofractal/pacmeg)

MATLAB scripts for detecting and validating phase amplitude coupling (PAC) in electrophysiological data. See [Seymour et al. (2017), *Frontiers in Neuroscience*](https://doi.org/10.3389/fnins.2017.00487).

## analyse_OPMEG (MATLAB)
[https://github.com/neurofractal/analyse_OPMEG](https://github.com/neurofractal/analyse_OPMEG)

A lair of scripts to analyse OPM data produced in collaboration with Dr. Nic Alexander.
