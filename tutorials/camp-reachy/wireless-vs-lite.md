# Camp Reachy Class Note: Wireless vs Lite

## Lesson Goal

Participants should understand that Reachy Mini Wireless and Reachy Mini Lite share the same visible robot body and many of the same learning ideas, but they differ in where the computer lives and how the robot connects.

## Short Explanation For Teachers

Reachy Mini comes in two main physical versions:

- **Reachy Mini Wireless**: the robot has its own onboard computer, battery, and Wi-Fi.
- **Reachy Mini Lite**: the robot depends on an external computer connected by USB and powered from the wall.

The simplest classroom analogy:

- Wireless is like a small robot with its own brain inside.
- Lite is like a robot body that borrows the laptop's brain.

## Quick Comparison

| Topic | Reachy Mini Wireless | Reachy Mini Lite |
| --- | --- | --- |
| Main role | Autonomous robot | Tethered education/development robot |
| Computer | Built-in Raspberry Pi Compute Module 4 | External Mac or Linux computer |
| Connection | Wi-Fi, plus direct access options | USB-C data cable to computer |
| Power | Internal battery system | Wall power |
| Movement hardware | Head, body, antennas | Head, body, antennas |
| Camera/audio | Camera, mic array, speaker | Camera, mic array, speaker |
| Extra sensor | Includes an accelerometer/IMU | No accelerometer listed |
| Best classroom framing | "Robot with onboard brain" | "Robot body controlled by laptop" |

## What Is The Same?

Both versions are useful for teaching robotics because they keep the same core physical ideas:

- A 6 degree-of-freedom head.
- A rotating body.
- Two animated antennas.
- A wide-angle camera.
- A microphone array and speaker.
- Python SDK control.
- App-based workflows through the Reachy Mini ecosystem.

Teacher explanation: the same program idea can often be taught on either model, but the setup path changes.

## What Is Different?

### Wireless

Wireless has a Raspberry Pi Compute Module 4 inside the robot. That means the robot can run its own software without depending on a laptop for every decision.

Classroom meaning:

- Students can think of the robot as a more independent machine.
- The setup includes Wi-Fi configuration.
- Teachers may need to update the robot's internal system.
- Advanced debugging can involve connecting to the robot over SSH.

### Lite

Lite connects to a computer by USB-C and needs that computer to run its intelligence.

Classroom meaning:

- It is straightforward for development because the code runs on the student's or teacher's computer.
- The robot must stay physically connected.
- It is useful for teaching how software on a laptop controls hardware.

## First Setup Difference

### Wireless First Setup

The official Wireless setup path is:

1. Assemble the robot.
2. Power it on.
3. Use Reachy Mini Control for first-time connection.
4. Connect to the robot's Wi-Fi access point.
5. Configure the robot onto the local Wi-Fi network.
6. Update the robot system before using it deeply.

Teacher note: this is a good moment to explain that networked robots need identity and access, just like laptops or phones joining a school network.

### Lite First Setup

The official Lite setup path is:

1. Assemble the robot.
2. Plug the robot into wall power.
3. Connect USB-C data from the robot to the computer.
4. Download and open Reachy Mini Control.
5. Use the desktop app or Python SDK to control the robot.

Teacher note: this is a good moment to explain that USB carries data, while the wall adapter supplies power.

## Camp Reachy Teaching Script

Ask participants:

> Where is the robot's brain?

Then guide them:

- If the brain is inside the robot, it is the Wireless model.
- If the brain is the laptop, it is the Lite model.

Follow-up question:

> What changes when the brain moves from the laptop into the robot?

Expected answers:

- The robot can be more independent.
- The robot needs Wi-Fi setup.
- The teacher may need to update onboard software.
- Debugging may happen over the network instead of only through a cable.

## Practical Camp Rule

For this camp, assume **Reachy Mini Wireless** unless a lesson says otherwise.

That means teacher instructions should normally include:

- Wi-Fi readiness.
- Reachy Mini Control.
- Robot system updates.
- The address `reachy-mini.local` or the robot's IP address when talking to the robot over the network.

## Student Q&A: What Version Of Raspberry Pi Is Inside?

### Question

What version of Raspberry Pi does Reachy Mini Wireless use?

### Answer

Reachy Mini Wireless uses a **Raspberry Pi Compute Module 4**, specifically listed in the official hardware datasheet as `CM4104016`.

That means:

- Raspberry Pi Compute Module 4.
- Wi-Fi model.
- 4GB RAM.
- 16GB onboard eMMC flash storage.

Teacher explanation: a Compute Module is not the same shape as the usual credit-card-sized Raspberry Pi board. It is an embedded version designed to plug into a custom robot controller board.

## Student Q&A: How Does That Compare To Newer Raspberry Pi Models?

### Question

How does Reachy Mini's Raspberry Pi Compute Module 4 compare to newer Raspberry Pi models?

### Answer

Reachy Mini Wireless uses Pi 4-class embedded hardware. Newer Raspberry Pi 5 and Compute Module 5 hardware is faster and has newer CPU, GPU, memory, and I/O options.

| Model | CPU class | RAM options | Storage style | Classroom summary |
| --- | --- | --- | --- | --- |
| Reachy Mini Wireless CM4 | Cortex-A72, 4-core, 1.5GHz | 4GB in this robot | 16GB onboard eMMC | Solid embedded robot controller |
| Compute Module 5 | Cortex-A76, 4-core, 2.4GHz | Up to 16GB | Up to 64GB onboard eMMC | Newer, faster embedded module |
| Raspberry Pi 5 | Cortex-A76, 4-core, 2.4GHz | Up to 16GB | microSD or SSD options | Newer hobby/development board |

Plain English:

- Reachy Mini Wireless is built around a **Compute Module 4**, which is roughly Raspberry Pi 4-generation hardware.
- Raspberry Pi 5 and Compute Module 5 are newer and can be much faster for heavy computing.
- That does not mean a teacher should plan to swap the robot to a newer Pi.

Teacher caution: the robot is a complete hardware and software system. Its controller board, power design, camera/audio wiring, operating system image, drivers, and Reachy daemon support are built around the CM4 Wireless hardware. A newer Pi module is not automatically a drop-in upgrade.

Teacher explanation: for Camp Reachy, the important lesson is not "newest chip wins." The important lesson is that robots are systems: compute, sensors, motors, power, software, and safety all have to work together.

## Sources

- Reachy Mini README in this repository.
- Official Reachy Mini Wireless setup guide: https://huggingface.co/docs/reachy_mini/platforms/reachy_mini/get_started
- Official Reachy Mini Wireless hardware datasheet: https://huggingface.co/docs/reachy_mini/platforms/reachy_mini/hardware
- Official Reachy Mini Lite setup guide: https://huggingface.co/docs/reachy_mini/platforms/reachy_mini_lite/get_started
- Official Reachy Mini Lite hardware datasheet: https://huggingface.co/docs/reachy_mini/platforms/reachy_mini_lite/hardware
- Raspberry Pi Compute Module 4 specs: https://www.raspberrypi.com/products/compute-module-4/
- Raspberry Pi Compute Module 5 specs: https://www.raspberrypi.com/products/compute-module-5/
- Raspberry Pi 5 specs: https://www.raspberrypi.com/products/raspberry-pi-5/
