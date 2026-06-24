# RobOtter

> Open-source biologically-inspired robotic companions for search & rescue, environmental survey, and the children who need them most.

---

## What Is This

RobOtter is an open-source robotics platform built around two biological models — the otter and the raccoon — chosen deliberately for what they represent mechanically and emotionally.

Otters are amphibious. They navigate water, debris, and tight spaces without complaint. Their forelimbs are manipulators first, locomotion second. Their silhouette reads as curious and non-threatening to a child in the dark.

Raccoons have near-primate finger independence and exceptional wrist mobility. They can feel inside a space they cannot see. They can open things. They can assess by touch.

Neither animal has ever been used to blow a door off its hinges. That is not an accident. That is the design philosophy.

---

## Platform Variants

### AR-01 — RobOtter
The primary platform. Otter-bodied, amphibious, mission-capable.

- Amphibious locomotion — rubble, water, wetland, confined space
- Dexterous forelimb manipulation — handles, valves, doors
- Onboard mapping and route charting for first responder handoff
- Victim location, communication relay, and sentinel hold
- Environmental sensing — spills, hazards, atmospheric conditions
- Companion mode — household object handling, communication, presence

### AR-02 — RingtailBot
Raccoon-influenced variant. Higher dexterity emphasis, optimized for manipulation tasks in structured environments.

- Raccoon facial geometry — expressive, legible, approachable
- Enhanced wrist and digit articulation
- Optimized for companion and domestic assist roles
- Shares core platform architecture with AR-01

---

## Why Not a Dog

The quadruped dog-form robot market is established, well-funded, and heavily oriented toward defense and industrial inspection applications. We have no interest in that space.

RobOtter is smaller. It goes places dogs cannot. It has hands. It does not have weapon hardpoints. Unlocking a door is more capable than breaching one, and considerably more useful in the contexts we care about.

---

## Core Architecture

### Shoulder — Magnetic Arc Platform
The defining mechanical innovation of the RobOtter platform.

A floating scapular platform driven by differential magnetic ring actuation. Two partial-arc magnet rings positioned at the endpoints of the biological scapular motion arc pull a central peg through its travel range via PWM differential. The peg position — and therefore the platform and attached limb — is commanded by field weight, not mechanical linkage.

The result is a shoulder assembly with no gears, no pivot pins, no mechanical binding, and inherent compliance. The natural fail state is center. The motion envelope is defined by the ring geometry and mirrors the biological scapular arc of the actual otter.

### Forelimb
Tendon-driven with proximal motor placement. Motors live in the torso, cables transmit force distally. Keeps the limb light and inertially appropriate for the platform scale.

### Sensing
- Dual-lens optical cameras with infrared — eye-position mounted
- LiDAR for mapping and obstacle characterization
- Microphone array — whisker-position acoustic sensing
- Hall effect position feedback on shoulder platform
- Environmental sensors — atmospheric, thermal, chemical (variant dependent)

### Control
- RP2040-based distributed joint control
- PWM shoulder actuation with Hall effect closed loop
- Onboard AI navigation and mapping processor
- Redundant communication arrays

### Exterior
- Synthetic fur layer with embedded heating elements
- Waterproof membrane
- Shock-absorbing polymer chassis
- Designed to be touched by a child and trusted by one

---

## Project Status

Early architecture and concept phase. Core shoulder mechanism under active design development. Animatronic proof-of-concept is the immediate build target.

This is an open project. Take it somewhere.

---

## License

Open source. Details in LICENSE.
