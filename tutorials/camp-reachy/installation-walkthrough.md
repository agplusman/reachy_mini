# Camp Reachy Installation Walkthrough

This walkthrough adapts the official Reachy Mini SDK installation guide for Camp Reachy teachers and participants.

Official source: https://huggingface.co/docs/reachy_mini/SDK/installation

## Lesson Goal

Teachers and participants should finish with a working Python environment that can import the Reachy Mini SDK and run the Reachy Mini app assistant.

## What We Installed On The Teacher Machine

- `uv` for Python environment and package management.
- Python 3.12 inside a virtual environment.
- Git LFS for large repository assets.
- Reachy Mini SDK from this local repository checkout.

## Important Version Note

The official docs list Python **3.10 to 3.12** as supported for Reachy Mini. Even though this computer also has Python 3.13, the Camp Reachy environment uses Python 3.12 so it stays inside the supported range.

Teacher explanation: the newest Python version is not always the best choice for robotics libraries. Hardware, media, and driver packages often support a narrower version range.

## Step 1: Verify `uv`

Command:

```bash
uv --version
```

Expected result on this machine:

```text
uv 0.11.7
```

Why this matters: `uv` creates virtual environments and installs Python packages quickly.

## Step 2: Install Git LFS

Command:

```bash
brew install git-lfs
git lfs install
git lfs version
```

Expected result on this machine:

```text
git-lfs/3.7.1
```

Why this matters: Git LFS handles large files that normal Git repositories do not store efficiently. Robotics projects often include assets, models, media, or binary files.

Teacher explanation: Git stores code well. Git LFS extends Git for larger files.

## Step 3: Create The Virtual Environment

From the repository folder:

```bash
cd /Users/malcolms/Documents/reachy_mini
uv venv reachy_mini_env --python 3.12
```

Expected result on this machine:

```text
Using CPython 3.12.9 interpreter
Creating virtual environment at: reachy_mini_env
Activate with: source reachy_mini_env/bin/activate
```

Why this matters: a virtual environment keeps Reachy Mini packages separate from the rest of the computer.

Teacher explanation: this is like giving Camp Reachy its own toolbox so it does not mix tools with other projects.

## Step 4: Activate The Environment

For an interactive lesson, activate the environment:

```bash
source reachy_mini_env/bin/activate
```

Expected result:

```text
(reachy_mini_env)
```

The environment name should appear at the start of the terminal prompt.

## Step 5: Install Reachy Mini From This Repository

For this teacher machine, we installed from the local checkout so our Camp Reachy fork and docs stay connected to the working SDK source:

```bash
uv pip install --python reachy_mini_env/bin/python -e .
```

Why this command is explicit: `uv` automatically detects virtual environments named `.venv`, but the official docs use `reachy_mini_env`. Passing `--python reachy_mini_env/bin/python` tells `uv` exactly which environment to install into.

Expected result:

```text
Installed 81 packages
reachy-mini==1.7.0
```

Teacher explanation: `-e .` means "install this folder as the package." Edits to the local source can be reflected without reinstalling from PyPI.

## Alternate Participant Install From PyPI

For participants who only need to control the robot and do not need to edit the SDK source, the official docs recommend:

```bash
uv pip install "reachy-mini"
```

If they are using a named environment like `reachy_mini_env`, use:

```bash
uv pip install --python reachy_mini_env/bin/python "reachy-mini"
```

For simulation support:

```bash
uv pip install --python reachy_mini_env/bin/python "reachy-mini[mujoco]"
```

## Step 6: Verify The SDK Imports

Command:

```bash
reachy_mini_env/bin/python -c "import sys; from reachy_mini import ReachyMini; print(sys.version.split()[0]); print('SDK installed successfully')"
```

Verified result on this machine:

```text
3.12.9
SDK installed successfully
```

Why this matters: importing `ReachyMini` proves Python can find the installed SDK.

## Step 7: Verify The App Assistant

Command:

```bash
reachy_mini_env/bin/reachy-mini-app-assistant --help
```

Verified result on this machine:

```text
usage: reachy-mini-app-assistant [-h] {create,check,publish} ...

App creation and publishing assistant for Reachy Mini.
```

Why this matters: this tool is the official path for creating Python Reachy Mini apps. Camp app projects should use it instead of manually inventing app folders.

## What Took Time

The SDK install downloaded the media stack, including GStreamer packages. On macOS this is normal because camera and audio support require larger dependencies.

Teacher explanation: robots are not just code. Camera, microphone, speaker, motors, USB, and networking all add supporting software.

## Troubleshooting Notes

### `uv` says no virtual environment was found

Symptom:

```text
error: No virtual environment found
```

Cause: the environment is named `reachy_mini_env`, not `.venv`.

Fix:

```bash
uv pip install --python reachy_mini_env/bin/python -e .
```

### Python 3.13 is installed, but docs recommend 3.12

Use Python 3.12 for Reachy Mini until the official docs say otherwise.

### Git LFS is missing

Symptom:

```text
git: 'lfs' is not a git command
```

Fix on macOS:

```bash
brew install git-lfs
git lfs install
```

## Completion Checklist

- `uv --version` works.
- `git lfs version` works.
- `reachy_mini_env` exists.
- The environment uses Python 3.12.
- `from reachy_mini import ReachyMini` succeeds.
- `reachy-mini-app-assistant --help` works.

## Next Lesson

After installation, continue to the official quickstart:

https://huggingface.co/docs/reachy_mini/SDK/quickstart
