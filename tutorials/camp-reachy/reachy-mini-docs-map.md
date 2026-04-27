# Camp Reachy Reference: Reachy Mini Docs Map

This map was built from the Hugging Face Reachy Mini documentation index so teachers can quickly find the right official page for each camp topic.

Source index: https://huggingface.co/docs/reachy_mini/index

## How Teachers Should Use This

- Use this as a navigation guide, not as a replacement for the official docs.
- Link students to the official page when they need screenshots, videos, or exact setup instructions.
- For Camp Reachy, start with Wireless setup, then SDK installation, then quickstart movement.
- Keep notes in this tutorial folder when we adapt an official doc into a camp lesson.

## Best First Path For Camp Reachy

1. [Reachy Mini index](https://huggingface.co/docs/reachy_mini/index)
2. [Wireless setup](https://huggingface.co/docs/reachy_mini/platforms/reachy_mini/get_started)
3. [Wireless usage](https://huggingface.co/docs/reachy_mini/platforms/reachy_mini/usage)
4. [SDK installation](https://huggingface.co/docs/reachy_mini/SDK/installation)
5. [SDK quickstart](https://huggingface.co/docs/reachy_mini/SDK/quickstart)
6. [Core concepts](https://huggingface.co/docs/reachy_mini/SDK/core-concept)
7. [Python SDK](https://huggingface.co/docs/reachy_mini/SDK/python-sdk)
8. [Building and publishing apps](https://huggingface.co/docs/reachy_mini/SDK/apps)

## Get Started

| Page | Use In Camp |
| --- | --- |
| [Reachy Mini index](https://huggingface.co/docs/reachy_mini/index) | Top-level orientation for teachers and students. |
| [SDK tutorials](https://huggingface.co/docs/reachy_mini/sdk-tutorials) | Notebook-based lessons for first connection, movement, camera, and audio. |

## Reachy Mini Wireless

| Page | Main Sections Found | Use In Camp |
| --- | --- | --- |
| [Wireless setup](https://huggingface.co/docs/reachy_mini/platforms/reachy_mini/get_started) | Assembly; first boot and Wi-Fi; update system; SSH; troubleshooting | Primary setup guide for this camp. |
| [Wireless hardware](https://huggingface.co/docs/reachy_mini/platforms/reachy_mini/hardware) | Global description; specific components | Explain the robot body, CM4 controller, camera, audio, motors, and battery. |
| [Wireless usage](https://huggingface.co/docs/reachy_mini/platforms/reachy_mini/usage) | Reachy Mini Control; applications; coding quickstart | First day robot operation after setup. |
| [Wireless media advanced controls](https://huggingface.co/docs/reachy_mini/platforms/reachy_mini/media_advanced_controls) | Camera; microphones and speakers | Later lesson for camera/audio experiments. |
| [Wireless reset](https://huggingface.co/docs/reachy_mini/platforms/reachy_mini/reset) | Bluetooth dashboard; nRF Connect; sending commands | Teacher troubleshooting reference, not a beginner lesson. |
| [Install daemon from branch](https://huggingface.co/docs/reachy_mini/platforms/reachy_mini/install_daemon_from_branch) | Prerequisites; local development; system-wide install; rollback | Advanced instructor/developer reference. |
| [Wireless development workflow](https://huggingface.co/docs/reachy_mini/platforms/reachy_mini/development_workflow) | Clone on robot; edit locally; override installed app sources | Advanced workflow for custom camp development. |
| [Reflash Raspberry Pi OS image](https://huggingface.co/docs/reachy_mini/platforms/reachy_mini/reflash_the_rpi_ISO) | Download image; rpiboot; flashing tool; restore boot mode | Emergency recovery or advanced maintenance only. |

## Reachy Mini Lite

| Page | Main Sections Found | Use In Camp |
| --- | --- | --- |
| [Lite setup](https://huggingface.co/docs/reachy_mini/platforms/reachy_mini_lite/get_started) | Assembly; connection; Reachy Mini Control; next step | Compare with Wireless and support Lite-specific sessions. |
| [Lite hardware](https://huggingface.co/docs/reachy_mini/platforms/reachy_mini_lite/hardware) | Global description; specific components | Explain what changes when the laptop is the robot brain. |
| [Lite usage](https://huggingface.co/docs/reachy_mini/platforms/reachy_mini_lite/usage) | Desktop control; applications; coding quickstart | Useful if a session uses a tethered unit. |
| [Lite media advanced controls](https://huggingface.co/docs/reachy_mini/platforms/reachy_mini_lite/media_advanced_controls) | Camera; microphones and speakers | Camera/audio reference for Lite. |
| [Dynamixel Wizard for Lite](https://huggingface.co/docs/reachy_mini/platforms/reachy_mini_lite/wizard) | Install wizard; connect; read motor parameters | Teacher troubleshooting and motor diagnostics. |

## Simulation

| Page | Use In Camp |
| --- | --- |
| [Simulation setup](https://huggingface.co/docs/reachy_mini/platforms/simulation/get_started) | Run lessons before hardware arrives or let more students practice when there are fewer robots. |

## SDK And Software Guide

| Page | Main Sections Found | Use In Camp |
| --- | --- | --- |
| [SDK readme](https://huggingface.co/docs/reachy_mini/SDK/readme) | Quick look; get started; examples; AI-assisted development | Short overview for teachers. |
| [Installation](https://huggingface.co/docs/reachy_mini/SDK/installation) | Prerequisites; virtual environment; install Reachy Mini; troubleshooting | Teacher setup and participant laptop setup. |
| [Core concepts](https://huggingface.co/docs/reachy_mini/SDK/core-concept) | Software architecture; coordinate systems; safety limits; motor modes | Must-read before movement lessons. |
| [Quickstart](https://huggingface.co/docs/reachy_mini/SDK/quickstart) | Daemon; first script; troubleshooting; AI coding agent | First coding lesson. |
| [Python SDK](https://huggingface.co/docs/reachy_mini/SDK/python-sdk) | Movement; sensors and media; media backends; recorded moves | Main reference for Python robot behaviors. |
| [AI integrations](https://huggingface.co/docs/reachy_mini/SDK/integration) | Building apps; JavaScript apps; HTTP and WebSocket API; AI tips | Later lessons for LLM and app projects. |
| [Building and publishing apps](https://huggingface.co/docs/reachy_mini/SDK/apps) | App lifecycle; app creation; app contract; web UI; testing; publishing | Camp app creation module. |
| [REST API](https://huggingface.co/docs/reachy_mini/API/rest-api) | Endpoint overview; full reference; complex apps | Advanced app/control lessons. |
| [JavaScript SDK and web apps](https://huggingface.co/docs/reachy_mini/SDK/javascript-sdk) | Why web apps; architecture; quick start | Browser-based app lessons. |
| [Media architecture](https://huggingface.co/docs/reachy_mini/SDK/media-architecture) | Unified architecture; media hardware access; advanced controls | Teacher reference for camera/audio behavior. |
| [GStreamer installation](https://huggingface.co/docs/reachy_mini/SDK/gstreamer-installation) | Install plugins; verify install; troubleshooting | Media troubleshooting, especially for camera/audio lessons. |

## Troubleshooting And Maintenance

| Page | Use In Camp |
| --- | --- |
| [Troubleshooting FAQ](https://huggingface.co/docs/reachy_mini/troubleshooting) | First stop for connection, movement, SDK, apps, and hardware issues. |
| [Motors diagnosis](https://huggingface.co/docs/reachy_mini/troubleshooting/motors_diagnosis) | Teacher-only motor troubleshooting path. |
| [Change microphone FPC cable](https://huggingface.co/docs/reachy_mini/troubleshooting/change_mic_fpc_cable) | Hardware repair reference, not a student activity. |
| [Spherical joints maintenance](https://huggingface.co/docs/reachy_mini/troubleshooting/spherical_joints_maintenance) | Maintenance reference for teachers. |

## Examples

| Page | Use In Camp |
| --- | --- |
| [Minimal demo](https://huggingface.co/docs/reachy_mini/examples/minimal_demo) | First safe robot behavior. |
| [Look at image](https://huggingface.co/docs/reachy_mini/examples/look_at) | Vision and attention lesson. |
| [Sequence](https://huggingface.co/docs/reachy_mini/examples/sequence) | Choreographed movement lesson. |
| [Goto interpolation playground](https://huggingface.co/docs/reachy_mini/examples/goto_interpolation_playground) | Smooth movement and timing lesson. |
| [IMU](https://huggingface.co/docs/reachy_mini/examples/imu) | Wireless sensor lesson. |
| [Compliant mode demo](https://huggingface.co/docs/reachy_mini/examples/reachy_compliant_demo) | Motor modes and physical interaction lesson. |
| [Recorded moves](https://huggingface.co/docs/reachy_mini/examples/recorded_moves) | Record and replay behavior. |
| [Rerun viewer](https://huggingface.co/docs/reachy_mini/examples/rerun_viewer) | Visualization lesson for advanced students. |
| [Take picture](https://huggingface.co/docs/reachy_mini/examples/take_picture) | Camera introduction. |
| [Joystick controller](https://huggingface.co/docs/reachy_mini/examples/joy_controller) | Human control interface lesson. |
| [Head position GUI](https://huggingface.co/docs/reachy_mini/examples/mini_head_position_gui) | UI control lesson. |
| [Custom media manager](https://huggingface.co/docs/reachy_mini/examples/custom_media_manager) | Advanced media customization. |
| [Sound recording](https://huggingface.co/docs/reachy_mini/examples/sound_record) | Audio input lesson. |
| [Sound playback](https://huggingface.co/docs/reachy_mini/examples/sound_play) | Audio output lesson. |
| [Sound direction of arrival](https://huggingface.co/docs/reachy_mini/examples/sound_doa) | Microphone array and sensing lesson. |

## API Reference

| Page | Use In Camp |
| --- | --- |
| [ReachyMini API](https://huggingface.co/docs/reachy_mini/API/reachymini) | Main class reference for advanced participants. |
| [Apps API](https://huggingface.co/docs/reachy_mini/API/apps) | App classes and app management reference. |
| [Media API](https://huggingface.co/docs/reachy_mini/API/media) | Camera and audio programming reference. |
| [Motion API](https://huggingface.co/docs/reachy_mini/API/motion) | Movement, goto moves, and recorded moves reference. |
| [Tools API](https://huggingface.co/docs/reachy_mini/API/tools) | Motor setup, scanning, and reflashing tools. |
| [Utils API](https://huggingface.co/docs/reachy_mini/API/utils) | Helpers for interpolation, hardware config, and visualization. |
| [Daemon API](https://huggingface.co/docs/reachy_mini/API/daemon) | Teacher/developer reference for app locking and daemon behavior. |

## Crawl Notes

- Crawl date: 2026-04-27.
- Pages found: 53.
- The crawl used the official Hugging Face docs index and followed Reachy Mini documentation links only.
- Static build assets were excluded.
- Full page contents were not copied into this repository; this file is a course navigation map.
