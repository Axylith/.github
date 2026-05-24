<p align="center">
  <img src="../assets/banner.svg" alt="Axylith" width="100%"/>
</p>

<p align="center">
  <a href="https://axylith.com"><b>axylith.com</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/Axylith/axle"><b>axle (editor)</b></a>
  &nbsp;·&nbsp;
  <a href="mailto:hi@axylith.com"><b>contact</b></a>
</p>

---

<p align="center">
  <img src="../assets/thesis.svg" alt="The thesis" width="100%"/>
</p>

---

<p align="center">
  <img src="../assets/projects.svg" alt="Projects" width="100%"/>
</p>

---

### Why this exists

Existing research tools were built for the workflows of the late 2000s. Jupyter assumes you have a Python kernel and a browser. MATLAB assumes you have a license server. Obsidian assumes prose and code are different things. None of them assume that the most powerful collaborator on your work might be an AI that needs structured access to all of it at once.

Axylith starts from a different assumption: that a researcher's workflow is one continuous activity &mdash; reading, writing, computing, visualizing, thinking &mdash; and the tool should reflect that continuity. One binary. One file format. One AI layer with structured access to everything in scope.

The current build is the substrate: a native text editor with a custom binary format, MTSDF text rendering through Vulkan 1.3, full CI matrix with sanitizers, and 79 unit-test assertions. The integration thesis is in active development.

### How this is being built

- **C++20 throughout.** Sub-millisecond input latency is part of the product. The editor measures and displays its own latency in the HUD.
- **Zero external runtime dependencies.** No Electron, no JavaScript runtime, no bundled browser. The binary is the binary.
- **Custom file format.** `.axl` is plain UTF-8 behind a small binary header in V1, structured pages and blocks in V2. Specified in C++ structs with `static_assert`-pinned layouts.
- **Linux-first.** X11 is the current target; Wayland is in scope for V1. Cross-platform comes after the architecture stabilizes.
- **Open source foundation, commercial extensions.** The editor is AGPL v3 with a commercial dual-license. The hosted AI sync and inference layers are proprietary paid tiers. Basic local functionality is never gated.

### Contributing

Axylith is a small project, currently in active solo development. Contributions are welcome but the architecture is still in flux; opening an issue before significant work is the way to ensure it fits the direction.

Each repository has its own CONTRIBUTING file. The general expectation is that contributions are typed (no LLM-generated PRs without disclosure), tested, and discussed before they're submitted.

### Get involved

- **Star the editor repository** if you want to follow development
- **Open issues** on bugs, design questions, or feature requests
- **Email** for partnerships, research collaborations, or licensing inquiries

<p align="center">
  <sub><sub>&middot;</sub></sub>
</p>

<p align="center">
  <sub>Built in Calgary, Canada.</sub>
</p>
