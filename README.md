# ReachQuest

A webcam-based **seated reach-to-target game** for upper-limb rehabilitation,
built for a *Principles of Rehabilitation* (occupational therapy) course project.

The patient sits facing a webcam and reaches toward on-screen targets in three
directions (forward/up, out to the side, and across the body). The game measures
active range of motion (AROM) via pose tracking, counts quality repetitions,
flags trunk-lean compensation, and gives encouraging, patient-centered feedback —
all wrapped in a motivating game with customizable avatars, themed worlds, music,
scoring, and a per-session progress roadmap.

> This repository hosts the **downloadable build** only. The source code lives in
> a separate private repository.

## Download & run (Windows)

1. Go to the [**Releases**](../../releases) page and download
   `ReachQuest_portable.zip`.
2. Unzip it anywhere.
3. Open the `ReachQuest` folder and run **`ReachQuest.exe`**.

No installation needed — Python and all dependencies (including the MediaPipe
models) are bundled. The app starts full-screen (press **F11** to toggle
windowed). A webcam is required; if the camera doesn't start, open **Settings**
and pick the right camera (and check Windows camera privacy settings).

In-game keys: `Esc`/`P` pause, `F11` fullscreen, `M` mute, `V` camera/avatar,
`K` cycle avatar.

## Features

- Three trained movements: shoulder **flexion**, **abduction**, and cross-body
  reach, with plain-language names and demonstrations.
- Clinical metrics: shoulder/elbow angles, max AROM, hysteresis rep counting,
  trunk-lean compensation, hold time.
- Goal ROM via **mirror** mode (healthy arm) or **clinician** mode (typed
  degrees, for bilateral patients), with four graded levels and patient-centered
  adaptive difficulty.
- **Six customizable avatars** (skeleton, robot, alien, ninja, wizard, cat) that
  mirror your movements, each with its own themed world and music.
- Score, combos, particle effects, and a **progress roadmap** (start → now →
  goal) after each set.
- **Two-arm (bilateral) mode**, a settings screen (volume / camera / difficulty),
  and a therapist report with charts (exportable to PDF).
- Local SQLite storage of patient progress (data stays on the machine).

## Disclaimer

This is an educational/training tool, **not** a medical device or a goniometer
replacement. The clinical thresholds are reasoned starting defaults, not
validated constants, and should be tuned by a qualified clinician.
