# Sources and attribution

**RETAILERWAY LLC** · Publication branding; third-party attribution is retained.

## Recorded human EEG reference

- Payne, A. and Ting, L., **Perturbation-evoked cortical responses associated
  with balance ability**. [Original Dryad dataset](https://datadryad.org/dataset/doi:10.5061/dryad.qz612jm9x),
  DOI: 10.5061/dryad.qz612jm9x. [Zenodo mirror](https://zenodo.org/records/3898501).
  The provider publishes the dataset under CC0. Raw data are not included here;
  only a reference figure with equally weighted participant means is shared.
- The original file's provider MD5 was verified:
  a3dc9824cf22d6608b0ae98d47d0c29f; 332,111,229 bytes.
  The inspected file contains 20 participants, 962 trials, 2,501 samples per
  trial, and a −0.5 to +2 s time axis. Provider prose described 960 trials
  and a −0.4 s start; the report uses the actual inspected file's dimensions.

## Balance responses and interpretation

- Jalilpour and Müller-Putz (2023), an experiment distinguishing early balance
  perturbation responses from error processing.
  [Primary paper abstract](https://pubmed.ncbi.nlm.nih.gov/36921343/),
  [DOI: 10.1088/1741-2552/acc486](https://doi.org/10.1088/1741-2552/acc486).
  Early N1 responses alone cannot establish error awareness or emotion.
- Official MNE documentation on the
  [EEG forward solution](https://mne.tools/stable/documentation/glossary.html#term-forward-solution),
  [units](https://mne.tools/stable/documentation/implementation.html#internal-representation-units),
  and [resampling](https://mne.tools/stable/auto_tutorials/preprocessing/30_filtering_resampling.html#resampling).
  These describe the source-to-scalp measurement bridge and sampling limits.

## Simulation and anatomy context

- [NVIDIA Isaac Lab](https://github.com/isaac-sim/IsaacLab): embodied-learning
  and simulation infrastructure. The local experiments used release/3.0.0.
- [Newton](https://github.com/newton-physics/newton): physics infrastructure.
- [Unitree G1](https://www.unitree.com/g1): the robot body represented in simulation.
- [Human Connectome Project](https://www.humanconnectome.org/): context for
  human connectivity data. Individual scans, connectivity matrices,
  participant identifiers, and atlas files are not distributed in this archive.

Citing these sources does not establish human-like consciousness, emotion,
or a validated whole-brain model. Third-party software, raw datasets, and robot
asset files are not included in the repository.
