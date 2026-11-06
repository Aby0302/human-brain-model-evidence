# Figure and video catalog

**RETAILERWAY LLC** · All current media use English labels and company stamps.

## Supported human-body recovery — November 6

| Recording | Duration / speed | Interpretation |
| --- | --- | --- |
| [Full prone recovery](../videos/supported-prone-recovery.mp4) | 16 s; 30 fps; 1× | Learned PPO residual + engineered measured-COM balance; seed47 body0 passes; primary48/48 |
| [Crouch to stand](../videos/crouch-to-stand.mp4) | 16 s; 30 fps; 1× | Separate later-start lesson, NOT full prone recovery; primary48/48 |

GIF excerpts preserve 1× timing: full recovery seconds1–13, crouch lesson1–8.
The standalone sequences and measurements also identify the hybrid controller.
[Results and matched zero-residual control](supported-getup.md) ·
[Derived numerical summaries](../metadata/supported-getup.json).

## Articulated human experiment — November 6

| Recording | Duration / speed | Interpretation |
| --- | --- | --- |
| [Human walking prototype](../videos/human-walking-prototype.mp4) | 16 s; 30 fps; 1× | Actuator-only saved-policy replay, seed 47 body 0; full attempt FAIL |
| [Human recovery prototype](../videos/human-recovery-prototype.mp4) | 16 s; 30 fps; 1× | Actual settling and attempted getup, no resets/pose writes; FAIL |
| [Authored getup target](../videos/human-getup-reference.mp4) | 11 s; 30 fps; 1× | Prescribed poses, NOT learned physics or motion capture |

The first two pair actual frames with the same body's physical measurements
and regional E/I activity at each control step. Their GIF previews show
seconds 1–9 at 1×, with rounded GIF delays. The reference preview is labeled
separately. [Results and limits](human-motion.md) ·
[Derived numerical summaries](../metadata/human-motion.json).

## Actual falls during learning

| File | Duration / speed | Provenance |
| --- | --- | --- |
| [Fall + synchronized regional activity](../videos/fall-with-activity.mp4) | 6.04 s; 25 frames/s; 0.5× | Separate video learning run; environment 8; matched frame and E/I control steps. |
| [Full learning capture](../videos/fall-learning-raw.mp4) | 28.8 s; 50 frames/s; 1× | Same run and visible body; branding/context footer added to the capture. |
| [GIF preview](../previews/fall-activity.gif) | Approximately 6.07 s; 0.5× | Derived from the short video; GIF frame delays are rounded. |
| [Fall-event frame](../images/fall-frame.png) | Control step 1061 | Same event as the video; simulation time 21.22 s. |

This run contains 6 falls overall and 1 in the visible body. It is not footage
of the primary analysis's three falls. Counts from the two runs are not pooled.

## Re-executions of saved walking policies

| File | Duration / speed | Description |
| --- | --- | --- |
| [Early and final policies, side by side](../videos/walking-comparison.mp4) | 10 s; 25 frames/s; 1× | Early policy on the left, final policy on the right; different training budgets. |
| [Early policy](../videos/walking-early.mp4) | 10 s; 25 frames/s; 1× | 8 falls in the visible body. |
| [Final policy](../videos/walking-trained.mp4) | 20 s; 25 frames/s; 1× | No visible-body falls; mean forward speed 0.3533 m/s. |
| [Walking preview](../previews/walking.gif) | Approximately 6 s; 1× | An excerpt from the final-policy replay. |
| [Four time points](../images/walking-frames.png) | Approximately 1 / 6 / 12 / 19 s | A frame sheet from the final-policy video. |

These recordings were captured after original training by re-running saved
policies. Motion comes from physics and policy outputs. The grid, camera,
English information overlays, and company stamp are presentation elements.
Automatic episode resets remain in the recordings. The comparison does not
isolate the connectivity-informed model's independent contribution.

## Scientific figures

| File | Contents |
| --- | --- |
| [Activity across 360 regions around falls](../images/fall-activity.png) | The 3 primary events, controls, neural reset, and dimensionless E changes. |
| [Recorded human EEG reference](../images/human-eeg-reference.png) | 20 participants, 962 trials, Cz in µV; support-surface perturbation response. |
| [Walking training progress](../images/training-progress.png) | Recorded training reward and fall-termination ratio; not held-out evaluation. |

[Downloadable release](https://github.com/Aby0302/human-brain-model-evidence/releases/tag/evidence-2026-11-05-en)
· [SHA-256 and video properties](../metadata/media-manifest.json)
· [Experiment report](experiment-report.md)


## Motor skill recordings — RETAILERWAY LLC

| Recording | Duration | Frame rate | Interpretation |
| --- | --- | --- | --- |
| [Running](../videos/running-with-activity.mp4) | 20 s | 50 fps | Saved-policy condition, visible body passes; batch 14/16 |
| [Stairs](../videos/stairs-with-activity.mp4) | 20 s | 50 fps | Four 8 cm risers; visible body passes; batch 14/16 |
| [Prone-to-standing](../videos/recovery-with-activity.mp4) | 16 s | 50 fps | 1 s settling + 15 s evaluation; batch 16/16 |
| [Continuous fall recovery](../videos/continuous-fall-recovery.mp4) | 18 s | 50 fps | One externally disturbed integration episode; 0 resets |

All four retain 1× timing and carry English labels and RETAILERWAY LLC branding.
GIF excerpts: running seconds 4–10, stairs 1–7, recovery 1–7, continuous episode 2.5–7.5.
[Methods, results and limitations](motor-skills.md).
