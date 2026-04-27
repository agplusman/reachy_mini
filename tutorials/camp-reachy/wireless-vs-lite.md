# Camp Reachy Class Note: Wireless vs Lite

## Lesson Goal

Participants should understand that Reachy Mini Wireless and Reachy Mini Lite share the same visible robot body and many of the same learning ideas, but they differ in where the computer lives and how the robot connects.

## Lesson Plan: Teaching The Hardware Difference

### Audience

Use this lesson with beginner robotics students before they write robot code. It works best after students have seen the robot, but before they connect to it.

### Time

30 to 40 minutes.

### Materials

- Reachy Mini Wireless if available.
- Reachy Mini Lite if available, or photos/spec sheets if not.
- A laptop.
- USB-C cable and wall power adapter for explaining Lite.
- A whiteboard or shared screen.

### Learning Outcomes

By the end, participants should be able to explain:

- Where the robot's computer is.
- How the robot gets power.
- How the robot connects to the teacher's or student's computer.
- What motors create the body, antenna, and head movement.
- What camera and microphone hardware let the robot sense the room.
- What the controller board connects together inside the robot.
- Why Wireless setup includes Wi-Fi.
- Why Lite setup includes USB and wall power.
- Why newer hardware is not automatically a better robot upgrade.

### Teacher Opening

Start with one simple question:

> If a robot moves, sees, hears, and reacts, where does the thinking happen?

Let students answer before introducing the two versions. The point is to separate the visible robot body from the computer that controls it.

### Teaching Flow

1. **Show the shared robot body**

   Point to the head, body, antennas, camera, microphone, and speaker.

   Teacher language: "Both versions can move, look, listen, and speak. The visible robot is mostly the same learning object: same size, same materials, same movement structure, and same sensing ideas."

2. **Introduce the brain location**

   Draw two boxes on the board:

   - Wireless: robot body plus onboard computer.
   - Lite: robot body plus laptop computer.

   Teacher language: "Wireless carries its computer inside. Lite borrows the laptop's computer through a cable."

3. **Introduce power**

   Explain that Wireless has an internal battery system, while Lite uses wall power.

   Teacher language: "Power is not the same as data. Power wakes the motors and electronics; data tells the robot what to do."

4. **Introduce connection**

   Explain that Wireless joins Wi-Fi, while Lite connects with USB-C data.

   Teacher language: "Wireless needs a network conversation. Lite needs a direct cable conversation."

5. **Connect to real setup steps**

   Ask students to predict the first setup steps for each model.

   Expected Wireless predictions:

   - Turn it on.
   - Find its Wi-Fi or connect it to Wi-Fi.
   - Use Reachy Mini Control.
   - Update the onboard system.

   Expected Lite predictions:

   - Plug in wall power.
   - Connect USB-C to the computer.
   - Open Reachy Mini Control.
   - Run code from the laptop.

6. **Discuss the Raspberry Pi Compute Module 4**

   Explain that Wireless uses a Raspberry Pi Compute Module 4.

   Teacher language: "This is not a normal desktop computer, but it is a real computer. It runs software inside the robot."

7. **Name the actuators**

   Explain that the robot's movement is built from Dynamixel motors:

   - 1 custom Dynamixel motor in the base.
   - 2 Dynamixel motors for the antennas.
   - 6 Dynamixel motors in the Stewart platform for the head.

   Teacher language: "The robot does not move because of one big motor. Different motors work together to create body rotation, antenna motion, and expressive head motion."

8. **Name the sensors and media hardware**

   Explain that the robot senses and communicates through camera, microphones, and speaker:

   - 120 degree wide-angle 12MP autofocus camera.
   - 4 digital microphones in a microphone array.
   - 5W speaker.

   Teacher language: "Seeing, hearing, and speaking are hardware features before they become software features."

9. **Explain the controller board**

   Explain that the controller board is the internal hub. It connects power, motors, camera, microphones, USB, and either onboard compute or laptop control.

   Teacher language: "The controller board is where many separate robot systems meet."

10. **Close with system thinking**

   Compare the robot to a team: computer, motors, sensors, power, network, and software.

   Teacher language: "A robot is not only a motor or only a computer. A robot works when every part of the system agrees."

### Participant Activity: Sort The Cards

Give students a list of cards or board labels and ask them to place each under Wireless, Lite, or Both.

Cards:

- Built-in Raspberry Pi Compute Module 4.
- Laptop runs the robot code.
- Controller board.
- Dynamixel motor TTL connection.
- Wi-Fi setup.
- USB-C data cable.
- Wall power.
- Internal battery.
- Head movement.
- Antennas.
- Camera.
- Microphone and speaker.
- 4 PDM MEMS digital microphones.
- 5W speaker.
- Python SDK.
- Reachy Mini Control.
- Onboard software update.

Expected sorting:

| Wireless | Lite | Both |
| --- | --- | --- |
| Built-in Raspberry Pi Compute Module 4 | Laptop runs the robot code | Head movement |
| Wi-Fi setup | USB-C data cable | Antennas |
| Internal battery | Wall power | Camera |
| Onboard software update |  | Microphone and speaker |
|  |  | Controller board |
|  |  | Dynamixel motor TTL connection |
|  |  | 4 PDM MEMS digital microphones |
|  |  | 5W speaker |
|  |  | Python SDK |
|  |  | Reachy Mini Control |

### Checks For Understanding

Ask:

1. Which model has the computer inside the robot?
2. Which model depends on the laptop as its computer?
3. Why does Wireless need Wi-Fi setup?
4. Why does Lite need USB?
5. What motors create the three main movement systems?
6. What hardware lets Reachy see, hear, and speak?
7. Why should we not assume a newer Raspberry Pi can simply replace the robot's current computer?

Strong answers:

- Wireless has the onboard computer.
- Lite uses the laptop as the main computer.
- Wireless needs Wi-Fi so the teacher's computer and robot can talk over the network.
- Lite needs USB so the laptop can send data directly to the robot.
- The base, antennas, and Stewart platform each have their own Dynamixel motor setup.
- Reachy sees with a wide-angle 12MP autofocus camera, hears with a 4-mic array, and speaks through a 5W speaker.
- The robot is a complete system, so the board, power, drivers, OS image, camera/audio, daemon, and safety behavior all need to match.

### Teacher Wrap-Up

End with:

> In Camp Reachy, we are using the Wireless path. That means we treat the robot as a small computer on the network, not just a device plugged into a laptop.

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
| Mass | 1.475 kg | 1.350 kg |
| Movement hardware | Head, body, antennas | Head, body, antennas |
| Camera/audio | Camera, mic array, speaker | Camera, mic array, speaker |
| Extra sensor | Includes an accelerometer/IMU | No accelerometer listed |
| Best classroom framing | "Robot with onboard brain" | "Robot body controlled by laptop" |

## Hardware Datasheet Details For Class

### Shared Physical Structure

Both versions have the same overall size and mechanical teaching value:

- Dimensions: 30 x 20 x 15.5 cm when extended.
- Materials: ABS, PC, aluminium, and steel.
- Head: 6 degrees of freedom.
- Body: 1 rotation.
- Antennas: 1 rotation each, for 2 antennas.
- Power input voltage: 6.8 to 7.6V.

Teacher explanation: degrees of freedom describe the different ways a robot part can move. A 6 DOF head can make much richer expressions than a single hinge.

### Shared Motors

Both versions list the same motor layout:

- Base: 1 custom Dynamixel XC330-M288-PG.
- Antennas: 2 Dynamixel XL330-M077-T motors.
- Stewart platform: 6 Dynamixel XL330-M288-T motors.

Teacher explanation: the head uses a Stewart platform, which means several motors cooperate to create smooth multi-direction movement.

### Shared Camera And Audio

Both versions list:

- Camera: Raspberry Pi Camera Module 3 wide angle.
- Camera sensor: Sony IMX708.
- Camera resolution: 12MP.
- Camera behavior: autofocus.
- Camera field of view: 120 degrees.
- Microphone board: 4 PDM MEMS digital microphones.
- Microphone board basis: Seeed Studio reSpeaker XMOS XVF3800.
- Audio sample rate: 16 kHz max.
- Microphone sensitivity: -26 dB FS.
- Signal-to-noise ratio: 64 dBA SNR.
- Speaker: 5W at 4 Ohms.

Teacher explanation: the camera and microphone array are why the robot can be used for perception lessons, not only movement lessons.

### Wireless-Specific Electronics

Reachy Mini Wireless adds onboard compute and battery detail:

- Control: Raspberry Pi Compute Module 4.
- CM4 part listed: CM4104016.
- CM4 configuration: Wi-Fi, 4GB RAM, 16GB flash.
- Battery: LiFePO4, 2000mAh, 6.4V, 12.8Wh.
- Battery protections: over-charge, over-discharge, over-current, short protection, and temperature sensor.
- Wi-Fi antenna: 2.4-5GHz dual-band patch antenna, 2.79 dBi, omnidirectional.
- CM4 controller board supply: 6.8 to 7.6V from the power board.
- CM4 controller board connections: Dynamixel Motor TTL, camera CSI, microphone array, USB-C output.

Teacher explanation: Wireless has more onboard responsibility. It carries compute, battery, Wi-Fi, and the software stack needed to behave as a networked robot.

### Lite-Specific Electronics

Reachy Mini Lite keeps the robot hardware but moves the main compute role to an external computer:

- Control: USB-C connection for the computer interface.
- Lite controller board supply: 6.8 to 7.6V from the power board.
- Lite controller board connections: Dynamixel Motor TTL, camera CSI, microphone array, USB-C input.
- The USB-C port is for data, not charging.
- The robot is described as a device plugged into a computer.

Teacher explanation: Lite is not "less robotics." It is a different architecture: the robot body is tethered to the computer that runs the control software.

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
