# Camp Reachy Assembly Lesson

This lesson turns the official Reachy Mini assembly material into a camp-ready teaching plan.

Primary official sources:

- Wireless setup guide: https://huggingface.co/docs/reachy_mini/platforms/reachy_mini/get_started
- Wireless interactive assembly guide: https://huggingface.co/spaces/pollen-robotics/Reachy_Mini_Assembly_Guide
- Full assembly video: https://www.youtube.com/watch?v=WeKKdnuXca4
- Lite setup guide: https://huggingface.co/docs/reachy_mini/platforms/reachy_mini_lite/get_started

## Lesson Goal

Participants should understand that assembly is not just "putting parts together." It is the first robotics systems lesson: power, compute, motors, cables, sensors, structure, and safety all have to work together.

## Time

Plan for **2 to 3 hours**. The official docs give the same estimate.

For a camp session, split it into checkpoints rather than trying to rush:

- 15 minutes: parts orientation and safety.
- 45 minutes: base, power, and motor foundations.
- 45 minutes: head platform and internal routing.
- 45 minutes: head shell, sensors, antennas, and final connections.
- 15 minutes: first power-on and reflection.

## Materials

- Reachy Mini kit.
- Included tools from the box.
- Paper manual.
- A laptop or large display with the interactive guide open.
- The full assembly video open as backup.
- Clear table space.
- Small trays or labeled areas for screws and subassemblies.

Teacher note: the official docs say everything needed is included in the box, but classroom management still matters. Use trays so small parts do not disappear.

## Teacher Preparation

Before participants arrive:

1. Open the interactive assembly guide.
2. Open the full YouTube video.
3. Confirm internet access.
4. Clear a large table.
5. Prepare a "do not force it" rule.
6. Decide whether students build directly or observe while one teacher handles delicate cable steps.

Teacher language:

> Today we are building a robot, but the real lesson is how a robot becomes a system. Every screw, cable, motor, board, and sensor has a job.

## Safety And Handling Rules

- Do not force connectors.
- Do not pull on flexible printed cables.
- Keep screws sorted.
- Keep liquids away from the table.
- Ask before powering anything.
- Rotate parts gently when checking motion.
- Stop if a cable seems too short, twisted, or pinched.

Teacher explanation: many robot problems come from assembly mistakes that are small at the time: a pinched cable, a loose connector, or a motor cable routed badly.

## Assembly Phases

The official Wireless interactive guide has 51 steps. For teaching, group them into these phases.

### Phase 1: Parts, Foot Pads, And Base Preparation

What happens:

- Students identify the parts.
- Foot pads are applied.
- USB extension cable and protective sleeve are positioned.

What to teach:

- Robots need mechanical stability before they can move safely.
- Cable routing starts early; cables are not an afterthought.

Teacher checkpoint:

- The base sits flat.
- The USB extension path is clear.
- Students can point to where power and data will eventually travel.

### Phase 2: Power Board And Battery

What happens:

- The power board is inserted and fixed.
- The battery is connected.
- Power cables are connected to the power board.

What to teach:

- The power board distributes energy safely.
- The Wireless model has an internal battery system.
- Battery protection matters: over-charge, over-discharge, over-current, short protection, and temperature sensing are part of the robot's safety system.

Teacher checkpoint:

- No cable is stretched.
- Power board is fixed.
- Battery connection is secure.
- No power-on happens yet unless the official guide says so.

### Phase 3: Bottom Assembly And Base Motor

What happens:

- The bottom assembly is positioned.
- The foot assembly is fixed to the bottom assembly.
- The foot motor is connected.

What to teach:

- The base motor gives the robot body rotation.
- Mechanical alignment matters because software assumes the body can rotate cleanly.

Teacher checkpoint:

- The base assembly is secure.
- The motor cable is connected and not pinched.
- Students can explain which movement the base motor controls.

### Phase 4: Stewart Platform Motors And Link Rods

What happens:

- Link rods are screwed onto motor arms.
- Six head-platform motors are connected in sequence.
- The motors are inserted into the bottom assembly.
- Motor cables are clipped and routed.

What to teach:

- The head uses a Stewart platform.
- Six motors cooperate to create expressive head movement.
- Cable routing protects motion range.

Teacher checkpoint:

- Link rods are attached without cross-threading.
- Motor cables follow the guide path.
- Students can explain why the head needs several motors instead of one.

### Phase 5: Tricap, Rotation Check, And Bottom Head

What happens:

- The tricap is positioned and screwed.
- Cable routing is checked.
- Rotation is checked.
- The bottom head is attached to the link rods.

What to teach:

- Mechanical checks happen before the shell closes.
- A rotation check is a safety checkpoint, not a decoration.

Teacher checkpoint:

- Motion feels smooth.
- Nothing scrapes or catches.
- Cables are visible where expected and hidden where required.

### Phase 6: Head PCB, Wi-Fi Antenna, Fan, And Camera Cable Routing

What happens:

- Wi-Fi antenna and fan cable are routed.
- Camera flexible cable routing is handled.
- Cables pass through the head PCB area.
- The head PCB is screwed in.

What to teach:

- Wireless needs radio hardware, not just software Wi-Fi settings.
- Flexible cables are delicate.
- The camera and head PCB connect sensing to compute.

Teacher checkpoint:

- The Wi-Fi antenna path follows the guide.
- Flexible cable is not bent sharply.
- Head PCB is seated and fixed.

### Phase 7: Top Shell, Glasses, And Front Head Assembly

What happens:

- Top shell is positioned and screwed.
- Lenses and fisheye parts are placed.
- Glasses assembly is attached to the front head shell.

What to teach:

- The robot's appearance also protects and positions sensors.
- Lens placement affects the camera's view and the robot's expression.

Teacher checkpoint:

- Shell pieces align without force.
- Lenses sit correctly.
- Students can explain why a camera needs a clean view.

### Phase 8: Antenna Motors And Back Head

What happens:

- Antenna motor cases are attached.
- Antenna assembly is fixed to the back head shell.
- Antenna motors are connected.
- Back head assembly slides onto the body and is screwed.

What to teach:

- Antennas are actuated robot parts, not decoration.
- Small expressive motions help humans read the robot's behavior.

Teacher checkpoint:

- Antenna motor cables are connected.
- Antenna assembly is secure.
- Nothing blocks the back head from closing cleanly.

### Phase 9: Final Internal Connections

What happens:

- Cable holder is fixed.
- Speaker, fan, and motor cables are connected.
- Power and USB extension cables are connected.
- Wi-Fi antenna is stuck in place.

What to teach:

- This is the system integration phase.
- Speaker, fan, motors, USB, power, and Wi-Fi are all different subsystems.

Teacher checkpoint:

- Each connector has a named purpose.
- Students can identify at least three subsystems now connected inside the robot.

### Phase 10: Front Head, Antennas, And First Power-On

What happens:

- Top head assembly slides onto the back head.
- Flexible printed cable and camera cable are connected.
- Front head is fixed.
- Antennas are fixed.
- Reachy Mini is turned on.

What to teach:

- Final assembly closes the system, so cable checks before closing matter.
- Power-on is a milestone, not the end of setup.
- Wireless setup continues with Wi-Fi configuration and system update.

Teacher checkpoint:

- Front head is secure.
- Antennas are attached.
- No cable is visibly pinched.
- Teacher controls the first power-on.

## Participant Roles

Use roles so more students participate without crowding the robot:

- Builder: handles the current physical step.
- Reader: reads the official guide aloud.
- Checker: confirms the checkpoint before moving on.
- Parts manager: keeps screws and parts organized.
- Systems reporter: explains what subsystem was just added.

Rotate roles every phase.

## Reflection Questions

Ask after assembly:

1. Which part gave the robot power?
2. Which parts gave the robot movement?
3. Which parts gave the robot sensing?
4. Which parts helped communication?
5. What would happen if a cable was routed through a moving area?
6. Why do we update the robot after assembly?

Strong answers:

- Battery and power board manage power.
- Dynamixel motors move the base, head platform, and antennas.
- Camera and microphone array provide sensing.
- Wi-Fi antenna, USB, and onboard computer support communication.
- A badly routed cable can block movement, get damaged, or cause unreliable behavior.
- Updates make sure the onboard software is current before use.

## After Assembly

Do not jump straight to Python code. Continue in order:

1. First boot and Wi-Fi configuration.
2. Reachy Mini Control connection.
3. System update.
4. Basic usage lesson.
5. SDK quickstart.

Official next step: https://huggingface.co/docs/reachy_mini/platforms/reachy_mini/get_started

## Teacher Notes For Camp Reachy

- We are primarily preparing for **Reachy Mini Wireless**.
- Lite assembly is similar at the kit level, but the post-assembly connection path differs.
- Wireless continues with Wi-Fi and onboard updates.
- Lite continues with wall power, USB data, and desktop control from the connected computer.
- Document any real camp build issues in this folder so future sessions can avoid them.

