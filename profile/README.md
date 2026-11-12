## 🧠🍳 neuro-kitchen

**Research software you can read, run and trust.**

neuro-kitchen is a growing open-source toolkit for research: GPU signal processing and spike
sorting, image analysis for histology, data conversion and paper management. The apps share one
frame and work with the agents you already use. Everything is free and open source: MIT or
Apache-2.0 (quire: AGPL-3.0).

🌐 **[neuro-kitchen.github.io](https://neuro-kitchen.github.io)**

### 🥘 What's on the menu

| Project | What it does |
|---|---|
| [**dsp-kitchen**](https://github.com/neuro-kitchen/dsp-kitchen) | Multi-channel signal processing and spike sorting on any GPU (Vulkan, Metal, CUDA, ROCm) or the CPU: a desktop app, Rust crates, `pip install dspk` and a command line |
| **lumen** *(coming soon)* | A GPU workstation for histology and microscopy: whole-slide and OME-Zarr images, annotation, pipelines and measurement tables |
| [**kitchen**](https://github.com/neuro-kitchen/kitchen) | What the apps share: one look, one frame, one list of actions for people and agents (`cargo add kitchen-ui`) |
| [**neuro-convert**](https://github.com/neuro-kitchen/neuro-convert) | Convert neuroscience data between formats |
| **quire** *(coming soon)* | A local-first reference manager for collecting, reading and citing papers, on desktop and mobile |

<!-- Keep this list in sync with src/data/tools.ts in neuro-kitchen.github.io. -->

### 🧩 One frame, many tools

- **Any GPU, or the CPU:** the heavy work is written once in CubeCL and runs on Vulkan, Metal,
  CUDA or ROCm, or on the CPU, from the app, Python or the command line.
- **One list of actions:** menus, keys, search and agents use the same commands, so none drifts.
- **Agents you already use:** the apps serve their actions to agents over MCP and run your own
  agent in their chat. No API keys in the apps; every action an agent takes is shown and recorded.
- **An episodic memory of the work:** a timeline of what you and the agent did, and where each
  result came from.

Some of these are still in progress; the [website](https://neuro-kitchen.github.io/#platform)
says which.

### 💖 Support the work

If these tools help your research:

- ⭐ **Star** the repos you use, so other researchers can find them
- 💖 **[Sponsor on GitHub](https://github.com/sponsors/neuro-kitchen)**, one-time or monthly
- 📄 **Cite** the software in your papers (each repo has a "Cite this repository" button)
- 🏛️ **Labs and institutions:** need an invoice? Open an issue or get in touch

### 🤝 Get involved

Bug reports, feature ideas, and pull requests are welcome. See the
[contributing guide](https://github.com/neuro-kitchen/.github/blob/main/CONTRIBUTING.md) to get started,
or join the [discussions](https://github.com/orgs/neuro-kitchen/discussions).
