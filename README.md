# The Orrery Project: A Vision for User-Centric Computing

## Manifesto: The “Why”

We exist in a digital world built by giants. Our devices, our software, and our data are planets orbiting stars that are not our own—behemoth corporations that define the rules of our digital lives. We are offered a choice between two extremes: the beautifully crafted but rigidly controlled "walled garden," or the chaotic, fragmented "open field" where seamless integration is a distant dream.

What if there was a third way?

Orrery is a new philosophy of computing built on a single, radical principle: **The user is the sun.** Every piece of hardware, every line of code, every interaction should revolve around the user's choice, control, and empowerment. It is not about building another operating system or another phone; it is about fundamentally re-architecting the relationship between people and their technology.

This document is the blueprint for that vision. It is a call to build an ecosystem that is open by default, integrated by design, and powerful by choice. An ecosystem where you decide the depth of your control.

Welcome to Orrery.

## The Core Technology: The Stellar Component Model (SCM)

To achieve true user-centricity, we need a common language that unifies the entire ecosystem. This language is the **Stellar Component Model (SCM)**.

The SCM's core principle is that **everything is a Component**. Whether it's a physical CPU module, a running application, a software driver, or a button in the user interface, the system sees it as a self-contained, understandable block.

Every Component, regardless of its nature, adheres to a universal structure:

- **`Component.ID`**: A unique, human-readable identifier that describes its place in the system (e.g., `hardware.cpu.core0`, `software.process.text_editor`, `gui.window.main.button.save`).
- **`Component.State`**: Its current condition, such as `active`, `idle`, `error`, or `disconnected`. This allows the system to understand and react to the status of any part of itself.
- **`Component.Properties`**: A list of its attributes. For a camera module, this could be `resolution:48MP` or `aperture:f/1.8`. For a software process, it could be `memory_usage:256MB`.
- **`Component.Inputs` & `Component.Outputs`**: Defines the data, signals, or triggers it can accept and produce. This is the key to interoperability, allowing any component to connect to any other compatible component.

The SCM is the technical soul of Orrery. It dissolves the traditional barriers between hardware, software, and the user interface, creating a single, cohesive, and transparent system.

## The Three Levels of Control

The SCM empowers the user to interact with their digital universe at three distinct, yet seamlessly integrated, levels of control. The user chooses their depth.

### Hardware Level: "Celestial Bodies”

This is the physical layer—the atoms of your system. Orrery hardware is built on a philosophy of **modularity and transparency**.

- **How it Works:** Each hardware module (camera, CPU, RAM, storage) is a physical manifestation of a Component. When you physically slot in a new camera module, Orrery OS instantly recognizes a new `hardware.camera` Component. It reads its `Properties` to load the correct driver (itself a Component) and makes its `Inputs` (e.g., `capture_image`) and `Outputs` (e.g., `image_data`) available to the rest of the system.
- **The Experience:** A user doesn't need to buy a whole new device to get a better camera. They buy the "Orrery Pro-Lens Module," click it into place, and the entire system adapts instantly. This is true ownership.

### Shell Level: "Gravity”

This is the ultimate nexus of control. The Orrery shell, named **Gravity**, is not merely a command line; it is a system-wide scripting and automation engine that can directly address any Component.

- **How it Works:** Gravity provides a simple, powerful syntax to query, manipulate, and connect Components.
    - `get-property hardware.cpu.thermal_sensor -> temperature`
    - `connect software.music_player.output -> software.stream_encoder.input`
    - `on-event (get-state software.process.code_editor) == active { set-state smarthome.light.desk -> on }`
- **The Experience:** Gravity provides limitless control. A musician can route audio between applications without complex virtual cables. A researcher can pipe data from a sensor directly into an analysis script. A power user can rebuild their entire workflow around simple, readable commands, automating their digital life in ways previously impossible.

### GUI Level: "Constellations”

This is the most accessible, visual layer. The Orrery GUI, or "Constellation," is simply a beautiful and intuitive visual representation of the underlying Components.

- **How it Works:** Every visual element is a user-friendly interface for a Component or a group of Components. A volume slider is a graphical way to change a `Property` of the `hardware.audio.output` Component. An application icon is a shortcut to activate a `software.application` Component.
- **The Experience:** Personalization is boundless. A user isn't just changing wallpapers; they are building their own desktop experience. A writer can create a "Constellation" with only a minimalist text editor. A video editor can build one that shows system performance graphs, media bins, and a large preview window—all as separate, rearrangeable GUI Components.

## Hardware Design Philosophy: Purpose-Driven Form

Orrery hardware rejects the one-size-fits-all approach. The physical shape of our devices should not be dictated by tradition, but should emerge from the true needs and ideal workflow of its intended user. This is **Purpose-Driven Form**.

We will not launch products in arbitrary "Pro" or "Max" tiers. We will launch purpose-built models for specific archetypes, cutting what isn't needed and perfecting what is.

- **The Canvas (for Artists):** An asymmetrical device with a weighted, curved edge for a comfortable one-handed grip, like a painter's palette. Its form is built for the act of creating art.
- **The Scribe (for Writers/Coders):** A three-part device featuring a vertical e-ink screen for focused writing, a side screen for research, and a fully detachable mechanical keyboard for perfect ergonomics. It is a dedicated, portable writing environment.
- **The Forge (for Gamers/Power Users):** An open, modular frame where airflow and immediate, tool-less access to every component are the primary design drivers, prioritizing function and upgradability above all else.

## Go-to-Market Strategy

Our strategy for bringing Orrery to the world is as deliberate and user-centric as our products.

### Phased Product Rollout

We will de-risk our launch and build trust by releasing products in a logical sequence.

1. **Orrery DIY Kits:** Our first physical product will be a bundle of an Orrery motherboard, CPU, and essential SCM-compatible modules. This empowers the enthusiast and builder community from day one, fostering a core group of technical evangelists.
2. **Simple, Focused Devices:** Our first fully-assembled products will be the least complex, allowing us to perfect our manufacturing. The **Orrery Hub** (a home server) or **The Scribe** are ideal starting points.
3. **Expansion to Complex Devices:** Only after succeeding with simpler forms will we tackle more complex challenges like **The Compass** (the phone), ensuring that every product meets our high standards of quality and philosophical integrity.

### Niche-First Audience Approach

We will not attempt to compete in the mass market initially. Our strength lies in serving groups who are underserved by generic products. We will establish a "beachhead" with users who have clustered requirements.

- **Initial Targets:** Groups like audio engineers, minimalist writers, visual artists, and open-source developers.
- **The Goal:** By creating the perfect tool for a specific niche, we will build a loyal, passionate user base. These "true fans" will provide invaluable feedback and become the foundation for our growth into wider markets.

## The Roadmap: An Invitation

The creation of Orrery is an immense undertaking, one that will unfold over years and will only be possible as a community effort.

- **Phase 1: Foundation.** Build the core community, finalize this White Paper, and develop the first proof-of-concept for the `Gravity` shell.
- **Phase 2: The Open-Source Core.** Release a usable, cross-platform version of the `Gravity` shell and the first alpha of Orrery OS, based on the Linux kernel. Grow the developer community.
- **Phase 3: The First Hardware.** Partner with manufacturers to release the first "Orrery DIY Kits" and our first purpose-built device.
- **Phase 4: The Ecosystem.** Expand the hardware line and fulfill the ultimate vision of a seamlessly integrated home universe, all powered by Orrery.

This is not a promise of a finished product. It is an invitation to an exploration. It is a call to developers, designers, thinkers, and builders who believe in a more open, transparent, and empowering digital future.

If this vision resonates with you, join us. Let's build it together.
