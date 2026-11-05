# Methods and limitations

**RETAILERWAY LLC**

## Experimental setup

The virtual body is Unitree G1, the environment uses NVIDIA Isaac Lab / Newton,
and motor learning uses PPO. A 360-region connectivity-informed activity model
responds to body motion, projected gravity, and movement commands. Regional
features enter the motor policy. The matrix remains fixed; this publication
does not establish a learned human brain or a physiological joint-to-region
mapping.

The primary monitoring run and the video run are separate continuations from
the same partially trained policy. Each contains 32 environments, 60 additional
updates, and 46,080 environment steps. Each run's 921.6 aggregate simulation
seconds do not represent one body walking continuously for that duration.

## Recording and controls

- Regional E/I states were captured at 50 Hz after physics and observation
  updates, before automatic episode reset.
- Torso-contact terminations were counted separately from timeouts.
- The primary analysis used one-second pre-event and post-event windows,
  required uninterrupted prehistory, and excluded nearby additional falls.
- Baseline-relative changes used the interval from −1 to −0.6 seconds.
- Non-fall controls matched the exact episode age. Events were averaged
  within environments before environments were weighted equally.
- Video frames and activity samples share the same control steps. The short
  clip is explicitly labeled 0.5×; the full capture plays at 1×.

Controls were not matched on kinematics or stochastic policy actions. The
three primary events came from one seed and one continuation. No confidence
interval, emotion classification, or human-similarity score was produced.

## Reset and physical recovery

After a fall, the environment and regional state restart. All three primary
events have next-step initial E=I=0.1. This software intervention is not a
measurement of biological suppression, unconsciousness, or post-impact emotion.

The offline recalculation omits neural resets while using recorded body inputs,
which still contain the actual physical reset. It does not calculate an
alternative physical future or a stand-up motion.

## Missing EEG and affect measurement bridge

Model states are dimensionless; scalp EEG measures physical voltage. A valid
comparison needs a justified source-to-sensor observation model, biological
time calibration, compatible tasks and event definitions, compatible
preprocessing, and human evaluation data held separate from calibration.

The 50 Hz simulation recording has a 25 Hz Nyquist limit in simulation-clock
units. Upsampling cannot restore missing rapid fluctuations. Without
biological-time calibration, slower model fluctuations cannot automatically
be labeled as human EEG bands either.

Emotional similarity additionally requires independent affect measurements
and an explicit hypothesis. A balance response alone is not evidence of fear
or pain. The human reference is a support-surface perturbation, rather than
the same torso-contact event.

## Media revision and verification

English figures were regenerated from the same recorded numerical data, and
English video overlays were rebuilt from the original capture and telemetry.
RETAILERWAY LLC stamps identify this publication's branding; the human dataset
and simulation-tool credits remain intact. Branding does not turn the human
reference into a company-owned measurement or a validation of the model.

Frame counts, event times, playback speeds, and reported results are preserved.
The full learning video's published copy includes a branding footer.
Published-file hashes, durations, dimensions, and frame counts can be checked.
Private traces and project source are not distributed, so training, regional
analysis, and human EEG extraction cannot be reproduced from this repository
alone.

The original local software checks passed 91 tests, with 7 optional tests
skipped in that environment. A separate simulation environment passed 28 tests,
including those 7. This is 98 unique tests across environments, rather than
91+28 independent tests. These checks concern software measurement, not
biological validity. The media revision is checked separately for file
integrity, successful decoding, and preserved frame timing.

[Sources](sources.md) · [Publication scope](../PUBLICATION.md)
