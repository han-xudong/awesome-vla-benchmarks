# Awesome VLA Benchmarks [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of benchmarks for evaluating Vision-Language-Action (VLA) models in robotics and embodied AI.

## Contents

- [Overview](#overview)
- [Manipulation Benchmarks](#manipulation-benchmarks)
- [Navigation Benchmarks](#navigation-benchmarks)
- [Multi-Task Benchmarks](#multi-task-benchmarks)
- [Language-Conditioned Benchmarks](#language-conditioned-benchmarks)
- [Simulation Environments](#simulation-environments)
- [Real-World Benchmarks](#real-world-benchmarks)
- [Leaderboards](#leaderboards)
- [Contributing](#contributing)

## Overview

Vision-Language-Action (VLA) models integrate visual perception, natural language understanding, and action generation to enable robots to follow open-vocabulary instructions. This list collects benchmarks used to evaluate VLA models across various domains.

## Manipulation Benchmarks

- **[BridgeData V2](https://rail-berkeley.github.io/bridgedata/)** - Large-scale robot manipulation dataset collected in a tabletop environment with language annotations.
- **[RLBench](https://github.com/stepjam/RLBench)** - A large-scale benchmark for robot learning with 100+ unique tasks in simulation.
- **[MetaWorld](https://meta-world.github.io/)** - A multi-task benchmark with 50 distinct manipulation tasks designed to evaluate meta-reinforcement learning.
- **[FurnitureBench](https://clvrai.github.io/furniture-bench/)** - A benchmark for furniture assembly tasks requiring long-horizon planning and dexterous manipulation.
- **[LIBERO](https://libero-project.github.io/)** - A benchmark for studying knowledge transfer in robot learning with 130 manipulation tasks.
- **[Calvin](http://calvin.cs.uni-freiburg.de/)** - A benchmark for evaluating long-horizon language-conditioned robot manipulation with 34 tasks.
- **[Open X-Embodiment](https://robotics-transformer-x.github.io/)** - A large-scale cross-embodiment dataset for robot manipulation with over 1M episodes.
- **[DROID](https://droid-dataset.github.io/)** - A large-scale robot manipulation dataset with diverse scenes and tasks collected by multiple institutions.

## Navigation Benchmarks

- **[R2R (Room-to-Room)](https://bringmeaspoon.org/)** - A benchmark for instruction-following navigation in indoor 3D environments.
- **[REVERIE](https://yuankaiqi.github.io/REVERIE_Challenge/)** - Remote Embodied Visual referring Expression task combining navigation and grounding.
- **[SOON](https://scenario-oriented-object-navigation.github.io/)** - A benchmark for scenario-oriented object navigation in 3D indoor environments.
- **[ScanQA](https://github.com/ATR-DBI/ScanQA)** - Spatial question answering benchmark grounded in 3D indoor scenes.
- **[EQA (Embodied Question Answering)](https://embodiedqa.org/)** - A benchmark requiring agents to navigate and answer questions about environments.
- **[ObjectNav](https://aihabitat.org/)** - Object navigation tasks within the Habitat simulator.

## Multi-Task Benchmarks

- **[BabyAI](https://github.com/mila-iqia/babyai)** - A synthetic benchmark for grounded language learning with increasing complexity levels.
- **[ALFWorld](https://alfworld.github.io/)** - A benchmark aligning text and visual environments for household task completion.
- **[VirtualHome](http://virtual-home.org/)** - A simulation platform for multi-step household activity execution from natural language.
- **[Habitat 3.0](https://aihabitat.org/)** - A simulation platform for embodied AI research supporting social navigation and collaboration tasks.
- **[AI2-THOR](https://ai2thor.allenai.org/)** - An interactive 3D simulation environment with physics-based interactions for diverse household tasks.
- **[ThreeDWorld](https://www.threedworld.org/)** - A 3D platform for multi-modal physical simulation supporting manipulation, navigation, and interaction.

## Language-Conditioned Benchmarks

- **[CLIP-Fields](https://mahis.life/clip-fields/)** - Weakly supervised semantic fields for robot navigation using natural language.
- **[SayCan](https://say-can.github.io/)** - A framework grounding language model planning in robot affordances; includes a 551-task evaluation suite.
- **[RT-2](https://robotics-transformer2.github.io/)** - Robotic Transformer 2 evaluation over 700+ tasks combining vision-language models with robot control.
- **[VIMA-BENCH](https://vimalabs.github.io/)** - A multimodal robot simulation benchmark with 17 tasks specified via interleaved text and image prompts.
- **[Octo](https://octo-models.github.io/)** - A generalist robot policy trained on Open X-Embodiment with evaluations across multiple platforms.

## Simulation Environments

- **[IsaacGym](https://developer.nvidia.com/isaac-gym)** - NVIDIA's physics simulation platform enabling GPU-accelerated reinforcement learning for dexterous manipulation.
- **[MuJoCo](https://mujoco.org/)** - A physics engine widely used for locomotion and manipulation benchmarks.
- **[PyBullet](https://pybullet.org/)** - Open-source physics simulation widely used in robot learning research.
- **[Genesis](https://genesis-world.readthedocs.io/)** - A generative simulation engine for robot learning with high-fidelity physics and rendering.
- **[SAPIEN](https://sapien.ucsd.edu/)** - A simulation environment with articulated objects for manipulation research.
- **[Robosuite](https://robosuite.ai/)** - A modular simulation framework for robot learning built on MuJoCo.

## Real-World Benchmarks

- **[ALOHA](https://tonyzhaozh.github.io/aloha/)** - A low-cost bimanual teleoperation system with benchmark tasks for imitation learning.
- **[LEROBOT](https://huggingface.co/lerobot)** - HuggingFace's real-world robot learning benchmark with standardized hardware and datasets.
- **[BridgeData](https://sites.google.com/view/bridgedata)** - Real-world tabletop manipulation dataset collected across multiple environments.
- **[RoboAgent](https://robopen.github.io/)** - Generalizable robot manipulation using semantic augmentations and semantic primitives.

## Leaderboards

- **[EvalAI](https://eval.ai/)** - A cloud-based platform hosting multiple embodied AI challenge leaderboards.
- **[Hugging Face Open VLA Leaderboard](https://huggingface.co/spaces/lerobot/eval_real_world_vla)** - Community leaderboard tracking VLA model performance on real-world tasks.
- **[LIBERO Leaderboard](https://libero-project.github.io/main.html)** - Official leaderboard for the LIBERO manipulation benchmark suite.

## Contributing

Contributions are welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

To add a benchmark:
1. Fork this repository.
2. Add the benchmark to the appropriate section in `README.md` following the existing format.
3. Submit a pull request.

Please ensure that:
- The benchmark is relevant to VLA model evaluation.
- You provide a link to the benchmark's official website or paper.
- The description is concise (one sentence).

---

If you find this list helpful, please consider giving it a ⭐!
