# Robotics Roadmap — Learn Robotics the Easy Way

This repository segment is for students who want to get into robotics for free. You only need:
- A laptop
- An internet connection

Everything else happens online using free tools and simulators.

---

## What you'll learn
- Design — CAD modeling with Onshape
- Electronics — Arduino and circuits with Tinkercad
- Programming — Python or C++ for robotics, AI, and ROS

---

## Quick start

1. Pick a starting track:
   - Design: Onshape (browser-based CAD)
   - Electronics: Tinkercad Circuits (Arduino simulator)
   - Programming: VS Code or PyCharm (Python/C++)

2. Learn the basics from free tutorials and official docs.
3. Build mini‑projects in simulation.
4. Select a project idea, document it, and build it virtually.

---

## Learning tracks

### Design (Onshape CAD)
- Tool: https://www.onshape.com/
- What to learn: sketch planes, constraints, extrude/revolve, assemblies.
- Practice projects: model a simple car/rover, a robotic arm, and a crane/bulldozer.

### Electronics (Tinkercad + Arduino)
- Tool: https://www.tinkercad.com/ (Circuits)
- What to learn: digital I/O, sensor reading, serial monitor, actuators.
- Practice projects: IR sensor with buzzer, ultrasonic sensor driving a motor/LED.

### Programming (Python or C++)
- Tools: https://code.visualstudio.com/ or https://www.jetbrains.com/pycharm/
- Start with fundamentals: variables, loops, conditionals, functions, modules, basic math libraries.
- Choose one path to explore deeper:
  - Computation and simulation
  - Machine learning and computer vision (OpenCV, Kaggle courses)
  - Path planning and robotics frameworks (ROS 2 Humble docs)

---

## Pick and plan your project

Use a short document (Google Doc or README) with:
- Team members (if any)
- Problem statement (clearly defined)
- Proposed solution and how the robot will be used
- Components or tools required (simulated/virtual)
- Milestones and approximate timeline
- References and resources used

---

## Cheatsheets

### Design checklist
- Sketching, constraints, shortcuts
- Extrude/revolve and creating 3D features
- Multi‑part assemblies and constraints

### Electronics checklist
- Transistors, LEDs, switches, pull‑up/pull‑down concepts
- Arduino UNO basics, sensors, and actuators
- Reading data in Serial Monitor and producing outputs

### Programming checklist
- Python/C++ basics: loops, conditionals, functions, modules
- Handling input from keyboard/mouse, simple visualization
- Math/science libraries and small project scripts

---

## Contributing

Have a better tutorial, a project idea, or a fix? Open a pull request or start a discussion. Keep it free, beginner‑friendly, and simulation‑first.

---

## Re‑create the roadmap image (optional)

You can re‑generate the flowchart with Graphviz:

```python
from graphviz import Digraph

dot = Digraph(format="png")
dot.attr(rankdir="LR")
dot.attr("node", shape="box", style="rounded")

dot.node("Start", "Getting Into Robotics\n(Free & Online)")
dot.node("Design", "Design\n(Onshape CAD)")
dot.node("Electronics", "Electronics\n(Tinkercad Circuits + Arduino)")
dot.node("Programming", "Programming\n(Python or C++)")
dot.edge("Start", "Design"); dot.edge("Start", "Electronics"); dot.edge("Start", "Programming")
dot.node("OnshapeSteps", "Learn basics:\n- Sketch\n- Constraints\n- Extrude/Revolve\n- Assemblies")
dot.node("OnshapeProjects", "Practice projects:\n- Car/Rover\n- Robotic Arm\n- Crane/Bulldozer")
dot.edge("Design", "OnshapeSteps"); dot.edge("OnshapeSteps", "OnshapeProjects")
dot.node("TinkercadSteps", "Start with Arduino UNO:\n- LEDs, sensors, motors\n- Serial Monitor")
dot.node("TinkercadProjects", "Practice projects:\n- IR + buzzer\n- Ultrasonic + motor")
dot.edge("Electronics", "TinkercadSteps"); dot.edge("TinkercadSteps", "TinkercadProjects")
dot.node("ProgSteps", "Learn the basics:\n- Loops, conditions\n- Libraries\n- Small programs")
dot.node("ProgBranches", "Explore paths:\n- Computation\n- Machine Learning\n- Path Planning (ROS 2)")
dot.edge("Programming", "ProgSteps"); dot.edge("ProgSteps", "ProgBranches")

dot.render("robotics_roadmap")
```

---

If anything in the roadmap is unclear or you want this adapted for your club's workflow, open an issue with details.
