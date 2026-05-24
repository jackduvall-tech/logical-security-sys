# Logic-Based Security System 🔐

A hardware-based intrusion detection system designed using combinational digital logic and discrete electronic components. This project monitors multiple entry points in real time using NOR gate logic and provides immediate visual feedback through dedicated status LEDs.

The project was developed as both a practical security-system proof of concept and an exploration of how real-world systems can be built using fundamental digital hardware principles without relying on software or microcontrollers.

---

## Project Overview ⚙️

This system monitors three simulated entry points:

- Front Door
- Back Door
- Window

Using combinational NOR gate logic, the system determines whether the protected area is secure or breached.

When all monitored entry points are closed:
- The system enters an **ARMED** state
- A dedicated status LED activates

If any entry point is opened:
- The ARMED state is disabled
- A corresponding indicator LED identifies the breached entry point in real time

The project demonstrates how digital logic can be applied to create fast, reliable hardware-based monitoring systems using simple low-cost components.

---

## Project Goals 🎯

- Design a real-time logic-based intrusion detection system
- Apply combinational logic concepts to a physical hardware build
- Translate theoretical circuit behavior into a functioning prototype
- Develop troubleshooting and hardware debugging skills
- Explore scalable security-system design concepts
- Demonstrate practical engineering problem solving using minimal hardware

---

## System Logic 🧠

The circuit is based around NOR gate behavior.

The system only enters the **ARMED** state when all inputs are LOW, meaning all monitored entry points are secure.

If any input changes state:
- The NOR logic immediately drives the output LOW
- The ARMED indicator turns off
- The triggered entry-point indicator activates

This creates a simple real-time monitoring system capable of visually identifying individual breach conditions.

---

## Hardware Components 🔧

### Core Components
- SN74LS02N Quad 2-Input NOR Gate
- SPST Switches
- LEDs
- 1kΩ Resistors
- Breadboard
- Jumper Wires
- 4.5V Battery Supply

### Indicator System
- Green LED → ARMED Status
- Red LED → Front Door
- Yellow LED → Back Door
- Blue LED → Window

---

## Design Workflow 🛠️

The project followed a multi-stage engineering workflow:

1. Initial theoretical logic design
2. Circuit schematic development
3. CircuitLab simulation
4. TinkerCAD layout planning
5. Physical breadboard implementation
6. Incremental debugging and validation
7. System behavior testing

This workflow helped bridge the gap between theoretical digital logic and real-world hardware implementation.

---

## Engineering Challenges 🧩

Some of the primary engineering challenges included:

- Translating theoretical logic into physical breadboard wiring
- Correctly mapping IC pin layouts
- Preventing unintended shared connections
- Debugging unstable or floating inputs
- Managing physical wire organization
- Verifying real-world circuit behavior against simulation results

One major design adaptation involved replacing the intended 3-input NOR gate with a quad 2-input NOR gate due to component availability constraints. The system was redesigned as a proof-of-concept while maintaining the original logical behavior.

---

## Testing & Validation ✅

Testing was performed through both simulation and physical hardware implementation.

Key validation tests included:
- Verifying ARMED state activation when all inputs were closed
- Confirming correct LED response for each triggered entry point
- Testing system reset behavior once all inputs returned to secure conditions
- Validating logic behavior against theoretical truth tables and Boolean expressions

The completed prototype successfully demonstrated the intended intrusion detection logic and system response behavior.

---

## Future Improvements 🚀

Planned future development includes:

- 555 timer integration
- Audible buzzer alarm system
- Delayed alarm activation
- Additional monitored entry points
- Improved PCB layout
- Compact enclosure integration
- Embedded system expansion
- Remote monitoring concepts

---

## Key Takeaways 📚

This project reinforced several important engineering concepts:

- Simulations do not guarantee successful physical implementation
- Hardware debugging is a critical engineering skill
- Organized wiring and incremental testing greatly improve troubleshooting
- Simple digital logic can solve meaningful real-world problems
- Design constraints often require practical engineering compromises

---

## Gallery 📸

### Circuit Schematic

---

### Breadboard Prototype
*Add breadboard image here*

---

### Truth Table & Boolean Logic
*Add truth table image here*

---

## Full Documentation 📄

Detailed project documentation, calculations, schematics, testing procedures, and design analysis are included in the project report.

---

## Tools & Software Used 💻

- CircuitLab
- TinkerCAD
- Breadboarding
- Digital Logic Design
- Boolean Algebra
- Combinational Logic Analysis
