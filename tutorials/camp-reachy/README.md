# Camp Reachy

Camp Reachy is a school and camp program for learning robotics with Reachy Mini. This tutorial folder documents every setup step, decision, and planned activity so teachers can explain the process and repeat it with participants.

## Goals

- Help participants understand robotics through visible, hands-on steps.
- Give teachers a repeatable path from laptop setup to running robot activities.
- Keep every command, outcome, and troubleshooting note in one place.
- Build toward sessions where students create small robot behaviors and apps.

## Work Completed So Far

### 1. Cloned the Reachy Mini Repository

We cloned the official Reachy Mini repository into the Documents folder:

```bash
cd /Users/malcolms/Documents
git clone https://github.com/pollen-robotics/reachy_mini.git
cd reachy_mini
```

Why this matters: the repository contains the Reachy Mini SDK, examples, documentation, app tools, and the agent instructions we use when building camp material.

Expected outcome: a local folder exists at `/Users/malcolms/Documents/reachy_mini`.

### 2. Read the Repository Agent Guide

We checked `AGENTS.md` and followed its first instruction: look for `agents.local.md`.

Why this matters: the project guide explains how Reachy Mini apps should be created, how to choose between Python and browser apps, and how to document plans before coding.

Expected outcome: future work follows the repo's own process instead of inventing a separate workflow.

### 3. Recorded the Robot Type

The camp setup is being prepared for a Reachy Mini Wireless.

Why this matters: Wireless Reachy Mini runs onboard with a Raspberry Pi CM4 and connects by WiFi, so some setup and lesson steps will differ from the Lite USB model.

Expected outcome: future instructions should assume Wireless unless a session explicitly targets simulation or Lite.

### 4. Upgraded the Shell Python Path

The system Python was too old for this repository, which requires Python 3.10 or newer. Homebrew Python 3.13.5 was already installed, so the shell path was updated to prefer it:

```bash
python --version
python3 --version
```

Expected outcome:

```text
Python 3.13.5
```

Why this matters: participants and teachers need a Python version that can install and run the Reachy Mini tools.

### 5. Installed `uv` For Faster Python Setup

We installed `uv` with Homebrew:

```bash
brew install uv
uv --version
```

Expected outcome:

```text
uv 0.11.7
```

Why this matters: `uv` creates virtual environments and installs Python packages much faster than plain `pip`. Reachy Mini tools can fall back to `pip`, but `uv` makes repeated camp setup faster and more reliable.

Teacher note: explain that `uv` is not the robot SDK itself. It is the tool that helps install the SDK and its dependencies quickly.

### 6. Created a Fork Workflow

The local Git repository now uses two remotes:

```bash
origin   https://github.com/agplusman/reachy_mini.git
upstream https://github.com/pollen-robotics/reachy_mini.git
```

Why this matters: `upstream` receives official updates from Pollen Robotics, while `origin` is the working fork where camp-specific changes can be saved.

To get official updates:

```bash
git fetch upstream
git merge upstream/main
git push origin main
```

To start camp-specific work:

```bash
git checkout -b codex/camp-reachy-topic
git push -u origin codex/camp-reachy-topic
```

Expected outcome: teachers can keep the code current while preserving Camp Reachy material in the fork.

## Planned Tutorial Sequence

Supporting class notes:

- [Wireless vs Lite](wireless-vs-lite.md): teacher-ready explanation of the two Reachy Mini versions and how their setup differs.
- [Reachy Mini docs map](reachy-mini-docs-map.md): crawled map of the official docs, organized for Camp Reachy lessons.

### Session 0: Teacher Setup

Purpose: prepare the instructor laptop before students arrive.

Planned steps:

- Confirm Python 3.10 or newer.
- Install or verify `uv`.
- Create a virtual environment.
- Install the Reachy Mini SDK.
- Clone reference apps and examples.
- Verify imports work.
- Confirm Git remotes are correct.

### Session 1: Meet Reachy Mini

Purpose: introduce the robot, safety basics, and the difference between Wireless, Lite, and simulation.

Planned steps:

- Identify robot parts: head, body, antennas, camera, microphone, speaker.
- Explain safe movement and why torque matters.
- Show how software commands become physical motion.

### Session 2: First Connection

Purpose: connect to the Wireless robot and confirm that the development environment works.

Planned steps:

- Power on the robot.
- Confirm network connection.
- Start or find the dashboard.
- Run a minimal SDK connection test.
- Record common connection problems and fixes.

### Session 3: First Movement

Purpose: teach basic robot motion using safe, slow commands.

Planned steps:

- Move the head with `goto_target()`.
- Move antennas.
- Return to a neutral pose.
- Explain why smooth interpolation is safer than sudden movement.

### Session 4: Build a Tiny Behavior

Purpose: combine motion, timing, and expression into a small routine.

Planned steps:

- Create a simple greeting behavior.
- Add comments explaining each command.
- Test and adjust motion timing.
- Discuss how behavior design affects personality.

### Session 5: Create a Camp App

Purpose: turn a behavior into a repeatable app.

Planned steps:

- Choose Python app or Live/Web/JS app.
- Write `plan.md` before coding.
- Scaffold using the official Reachy app assistant when building Python apps.
- Document controls, expected behavior, and troubleshooting.

## Documentation Rules For This Folder

- Every session gets its own markdown file.
- Every command must include its purpose and expected outcome.
- Teacher notes should explain what to say, not just what to type.
- Participant steps should be short, visible, and testable.
- Troubleshooting notes should describe symptoms and fixes.
- Keep examples safe for a classroom or camp setting.
