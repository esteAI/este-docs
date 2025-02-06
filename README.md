# What is ESTÉ?

**ESTÉ** is an artificial life simulation tool based on a specialized 2D particle engine in CUDA for soft bodies and fluid-like media. Each simulated body consists of a network of particles that can be enriched with higher-level functions, ranging from pure information processing capabilities to physical equipment (such as sensors, muscles, weapons, constructors, etc.) whose executions are orchestrated by a signaling system. The bodies can be thought of as agents or digital organisms operating in a common environment.

What characterizes the simulator:

* Two-layered particle engine: The bottom layer simulates the thermo-mechanical behavior of soft bodies and their surrounding fluids, while a powerful information processing and action processor operates on the top layer.
* Vector graphics engine: The rendering is completely decoupled from the simulation engine. Sections of the simulated world are rendered as vector graphics and post-processed using shaders. The level of detail is adjusted with the zoom level. At a lower zoom level only the nodes are displayed, whereas at a higher levels, edges, information flows and (optionally) internal states are also visible.
* Particle editor: The properties and function of each particle can be modified. For example, editing windows can be pinned to several particles and even updated while the simulation is running. An embedded programming environment is provided for particles that are intended to perform computational operations.
* World editor: Parts of existing bodies can be easily disassembled, rearranged and connected just by using the mouse. The graphs of new bodies can be created as geometric shapes or freehand drawings. Mass and scaling operations facilitate the creation of large worlds.
* Extensive capabilities to control simulation parameters: It is possible to define different simulation parameters in spatial zones as well as to fluctuate them in time.

The main design goals:

* Utilization of CUDA and OpenGL for simulation and rendering to support large worlds with millions of particles.
* No hard-coded behavior patterns. Everything should emerge from the interaction of particles.
* An enjoyable user interface in spite of the high complexity of the simulation model and the wide range of adjustment options.
* Visually appealing post-processing of the rendered simulation data.
