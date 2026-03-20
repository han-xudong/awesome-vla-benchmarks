# Awesome VLA Benchmarks [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/han-xudong/awesome-vla-benchmarks/pulls)
[![GitHub Stars](https://img.shields.io/github/stars/han-xudong/awesome-vla-benchmarks?style=social)](https://github.com/han-xudong/awesome-vla-benchmarks/stargazers)
[![Last Commit](https://img.shields.io/github/last-commit/han-xudong/awesome-vla-benchmarks)](https://github.com/han-xudong/awesome-vla-benchmarks/commits)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

> If you find this list helpful, please consider giving it a ⭐ — it helps others discover the resource!

A curated list of benchmarks for evaluating **Vision-Language-Action (VLA)** models — systems that unify visual perception, language understanding, and executable action generation. Covers all major evaluation domains: embodied robotics, autonomous driving, GUI agents, game environments, egocentric video, and multimodal perception.

## Contents

- [Embodied Robotics](#embodied-robotics)
  - [Robot Manipulation](#robot-manipulation)
  - [Dexterous Manipulation & Locomotion](#dexterous-manipulation--locomotion)
  - [Embodied Navigation](#embodied-navigation)
  - [Embodied Multi-Task & Household](#embodied-multi-task--household)
  - [Social & Human-Robot Interaction](#social--human-robot-interaction)
- [Autonomous Driving](#autonomous-driving)
- [GUI & Computer-Use Agents](#gui--computer-use-agents)
- [Game & Interactive Environments](#game--interactive-environments)
- [Multimodal Perception & Understanding](#multimodal-perception--understanding)
  - [General Multimodal](#general-multimodal)
  - [Video & Temporal Understanding](#video--temporal-understanding)
  - [Egocentric & Activity](#egocentric--activity)
  - [3D Scene Understanding](#3d-scene-understanding)
  - [Language-Grounded Perception](#language-grounded-perception)
- [Infrastructure & Resources](#infrastructure--resources)
  - [Simulation Environments & Platforms](#simulation-environments--platforms)
  - [Large-Scale Datasets & Model Hubs](#large-scale-datasets--model-hubs)
  - [Leaderboards & Evaluation Platforms](#leaderboards--evaluation-platforms)
- [Contributing](#contributing)
- [License](#license)

---

## Embodied Robotics

Benchmarks for physical or simulated robots that must perceive, reason, and act in the real or virtual world.

### Robot Manipulation

Benchmarks focused on language-conditioned robot arm or bimanual manipulation tasks.

| Name | Highlights | References |
|------|-----------|------------|
| [Open X-Embodiment (OXE)](https://robotics-transformer-x.github.io/) | [ICRA 2024] Cross-embodiment dataset with 1M+ robot episodes from 22 institutions and 22 robot types | [arXiv](https://arxiv.org/abs/2310.08864) · [GitHub](https://github.com/google-deepmind/open_x_embodiment) · [Website](https://robotics-transformer-x.github.io/) |
| [DROID](https://droid-dataset.github.io/) | [RSS 2024] 76k demonstrations across diverse real-world environments for scalable VLA training | [arXiv](https://arxiv.org/abs/2403.12945) · [GitHub](https://github.com/droid-dataset/droid) · [Website](https://droid-dataset.github.io/) |
| [ManiSkill3](https://maniskill.ai/) | [NeurIPS 2024] GPU-parallelized simulation with richer tasks and improved evaluation protocols | [arXiv](https://arxiv.org/abs/2410.00425) · [GitHub](https://github.com/haosulab/ManiSkill) · [Website](https://maniskill.ai/) |
| [RoboCasa](https://robocasa.ai/) | [RSS 2024] 100+ kitchen manipulation tasks in photorealistic MuJoCo-based environments | [arXiv](https://arxiv.org/abs/2406.02523) · [GitHub](https://github.com/robocasa/robocasa) · [Website](https://robocasa.ai/) |
| [SimplerEnv](https://simpler-env.github.io/) | [CoRL 2024] Simulation evaluation framework designed to correlate with real-world VLA performance | [arXiv](https://arxiv.org/abs/2405.05941) · [GitHub](https://github.com/simpler-env/SimplerEnv) · [Website](https://simpler-env.github.io/) |
| [Mobile ALOHA](https://mobile-aloha.github.io/) | [CoRL 2024] Extends ALOHA to a mobile whole-body platform for real-world household tasks | [arXiv](https://arxiv.org/abs/2401.02117) · [GitHub](https://github.com/MarkFzp/mobile-aloha) · [Website](https://mobile-aloha.github.io/) |
| [RoboAgent](https://robopen.github.io/) | [ICRA 2024] Generalizable manipulation via semantic augmentations evaluated on 12 real-world tasks | [arXiv](https://arxiv.org/abs/2309.01918) · [GitHub](https://github.com/robopen/roboagent) · [Website](https://robopen.github.io/) |
| [Octo](https://octo-models.github.io/) | [RSS 2024] Generalist robot policy trained on OXE data, evaluated across BridgeV2 and Franka | [arXiv](https://arxiv.org/abs/2405.12213) · [GitHub](https://github.com/octo-models/octo) · [HF](https://huggingface.co/rail-berkeley/octo-base) · [Website](https://octo-models.github.io/) |
| [GR-1](https://github.com/bytedance/GR-1) | [ICLR 2024] ByteDance's generalist manipulation policy evaluated on CALVIN and real-world tasks | [arXiv](https://arxiv.org/abs/2312.13139) · [GitHub](https://github.com/bytedance/GR-1) |
| [OpenVLA](https://openvla.github.io/) | [CoRL 2024] Open-source 7B VLA model evaluated on BridgeV2 and OXE tasks | [arXiv](https://arxiv.org/abs/2406.09246) · [GitHub](https://github.com/openvla/openvla) · [HF](https://huggingface.co/openvla/openvla-7b) · [Website](https://openvla.github.io/) |
| [LIBERO](https://libero-project.github.io/) | [NeurIPS 2023] Knowledge transfer across 130 language-conditioned tasks in 4 structured suites | [arXiv](https://arxiv.org/abs/2306.03310) · [GitHub](https://github.com/Lifelong-Robot-Learning/LIBERO) · [Website](https://libero-project.github.io/) |
| [VIMA-BENCH](https://vimalabs.github.io/) | [ICML 2023] 17 task types specified via interleaved text-and-image prompts for multimodal manipulation | [arXiv](https://arxiv.org/abs/2210.03094) · [GitHub](https://github.com/vimalabs/VIMA) · [Website](https://vimalabs.github.io/) |
| [FurnitureBench](https://clvrai.github.io/furniture-bench/) | [RSS 2023] Real and simulated furniture assembly requiring long-horizon dexterous manipulation | [arXiv](https://arxiv.org/abs/2305.11959) · [GitHub](https://github.com/clvrai/furniture-bench) · [Website](https://clvrai.github.io/furniture-bench/) |
| [BridgeData V2](https://rail-berkeley.github.io/bridgedata/) | [CoRL 2023] Large-scale tabletop manipulation with language annotations across diverse kitchen scenes | [arXiv](https://arxiv.org/abs/2308.12952) · [GitHub](https://github.com/rail-berkeley/bridge_data_v2) · [Website](https://rail-berkeley.github.io/bridgedata/) |
| [ManiSkill2](https://maniskill2.github.io/) | [ICLR 2023] 20 task families with rigid/soft-body physics for generalizable manipulation skill evaluation | [arXiv](https://arxiv.org/abs/2302.04659) · [GitHub](https://github.com/haosulab/ManiSkill2) · [Website](https://maniskill2.github.io/) |
| [ALOHA / ACT](https://tonyzhaozh.github.io/aloha/) | [RSS 2023] Low-cost bimanual teleoperation with imitation learning demonstrations | [arXiv](https://arxiv.org/abs/2304.13705) · [GitHub](https://github.com/tonyzhaozh/act) · [Website](https://tonyzhaozh.github.io/aloha/) |
| [RT-1](https://robotics-transformer1.github.io/) | [RSS 2023] Google's Robotics Transformer trained on 700+ real-world manipulation tasks | [arXiv](https://arxiv.org/abs/2212.06817) · [Website](https://robotics-transformer1.github.io/) |
| [RT-2](https://robotics-transformer2.github.io/) | [CoRL 2023] Combines internet-scale VLM pretraining with robot control for emergent generalization | [arXiv](https://arxiv.org/abs/2307.15818) · [Website](https://robotics-transformer2.github.io/) |
| [CALVIN](http://calvin.cs.uni-freiburg.de/) | [RA-L 2022] Long-horizon manipulation requiring chaining up to 5 language-conditioned tasks in a row | [arXiv](https://arxiv.org/abs/2112.03227) · [GitHub](https://github.com/mees/calvin) · [Website](http://calvin.cs.uni-freiburg.de/) |
| [RoboMimic](https://robomimic.github.io/) | [CoRL 2021] Standardized demonstration datasets and algorithm baselines for robot learning | [arXiv](https://arxiv.org/abs/2108.03298) · [GitHub](https://github.com/ARISE-Initiative/robomimic) · [Website](https://robomimic.github.io/) |
| [RLBench](https://github.com/stepjam/RLBench) | [RA-L 2020] 100+ unique language-conditioned tasks in CoppeliaSim simulator | [arXiv](https://arxiv.org/abs/1909.12271) · [GitHub](https://github.com/stepjam/RLBench) |
| [MetaWorld](https://meta-world.github.io/) | [CoRL 2020] 50 distinct tabletop manipulation tasks for multi-task and meta-RL | [arXiv](https://arxiv.org/abs/1910.10897) · [GitHub](https://github.com/Farama-Foundation/Metaworld) · [Website](https://meta-world.github.io/) |
| [Franka Kitchen](https://github.com/google-research/relay-policy-learning) | [CoRL 2019] Multi-task kitchen manipulation with a Franka Panda robot across 7 compound subtasks | [arXiv](https://arxiv.org/abs/1910.11956) · [GitHub](https://github.com/google-research/relay-policy-learning) |
| [SpatialBench](https://github.com/kahnchana/spatial_bench) | Evaluates spatial reasoning capabilities of VLMs in manipulation contexts | [GitHub](https://github.com/kahnchana/spatial_bench) |
| [π0 (pi-zero)](https://www.physicalintelligence.company/blog/pi0) | Physical Intelligence's large robot foundation model for diverse dexterous tasks | [arXiv](https://arxiv.org/abs/2410.24164) · [Website](https://www.physicalintelligence.company/blog/pi0) |
| [VLABench](https://vlabench.github.io/) | [ICCV 2025] Large-scale benchmark for language-conditioned manipulation with long-horizon reasoning across 100 tasks and multiple dimensions | [arXiv](https://arxiv.org/abs/2412.18194) · [GitHub](https://github.com/OpenMOSS/VLABench) · [HF](https://huggingface.co/VLABench) · [Website](https://vlabench.github.io/) |
| [RoboVerse](https://roboverseorg.github.io/) | [RSS 2025] Unified platform, dataset, and benchmark for scalable and generalizable robot learning across 5000+ tasks | [arXiv](https://arxiv.org/abs/2504.18904) · [GitHub](https://github.com/RoboVerseOrg/RoboVerse) · [Website](https://roboverseorg.github.io/) |
| [MIKASA-Robo](https://sites.google.com/view/memorybenchrobots/) | [ICLR 2026] Benchmark for robotic tabletop manipulation with 32 memory-intensive tasks covering object, spatial, sequential, and capacity memory | [arXiv](https://arxiv.org/abs/2502.10550) · [GitHub](https://github.com/CognitiveAISystems/MIKASA-Robo) · [Website](https://sites.google.com/view/memorybenchrobots/) |
| [RoboVLMs](https://robovlms.github.io/) | Comprehensive evaluation of VLMs as robot policy foundation models across manipulation tasks | [GitHub](https://github.com/Robot-VLAs/RoboVLMs) · [Website](https://robovlms.github.io/) |
| [RoboTwin](https://robottwin.github.io/) | [CVPR 2025] Dual-arm robot benchmark with generative digital twins for automated data collection across 50 diverse bimanual manipulation tasks | [arXiv](https://arxiv.org/abs/2409.02920) · [GitHub](https://github.com/Tele-AI/RoboTwin) · [Website](https://robottwin.github.io/) |
| [BiGym](https://chernyadev.github.io/bigym/) | Demo-driven mobile bi-manual manipulation benchmark with 40 novel household tasks spanning easy to extremely difficult difficulty levels | [arXiv](https://arxiv.org/abs/2407.07788) · [GitHub](https://github.com/chernyadev/bigym) · [Website](https://chernyadev.github.io/bigym/) |

### Dexterous Manipulation & Locomotion

Benchmarks for fine motor skills, multi-fingered hands, and legged/mobile robots.

| Name | Highlights | References |
|------|-----------|------------|
| [HumanoidBench](https://humanoid-bench.github.io/) | [NeurIPS 2024] 27 diverse whole-body tasks for humanoid robot control evaluation | [arXiv](https://arxiv.org/abs/2403.10506) · [GitHub](https://github.com/carlosferrazza/humanoid-bench) · [Website](https://humanoid-bench.github.io/) |
| [DexArt](https://www.chenbao.tech/dexart/) | [CVPR 2023] 4 complex dexterous tasks for articulated object manipulation with a multi-fingered hand | [arXiv](https://arxiv.org/abs/2305.05706) · [GitHub](https://github.com/Kami-code/dexart-release) · [Website](https://www.chenbao.tech/dexart/) |
| [DexDeform](https://github.com/sizhe-li/DexDeform) | [ICLR 2023] 5 dexterous deformable object manipulation tasks for learning contact-rich policies | [arXiv](https://arxiv.org/abs/2304.03223) · [GitHub](https://github.com/sizhe-li/DexDeform) |
| [LEAP Hand](https://leaphand.com/) | [CoRL 2023] Low-cost dexterous hand platform with benchmark tasks for in-hand manipulation | [arXiv](https://arxiv.org/abs/2309.06440) · [Website](https://leaphand.com/) |
| [MyoSuite](https://sites.google.com/view/myosuite) | [NeurIPS 2022] Musculoskeletal simulation for physiologically accurate hand and arm control | [arXiv](https://arxiv.org/abs/2205.13600) · [GitHub](https://github.com/MyoHub/myosuite) · [Website](https://sites.google.com/view/myosuite) |
| [IsaacGym Benchmark](https://developer.nvidia.com/isaac-gym) | [NeurIPS 2021] GPU-accelerated dexterous benchmarks including in-hand cube reorientation and pen spinning | [arXiv](https://arxiv.org/abs/2108.10470) · [Website](https://developer.nvidia.com/isaac-gym) |
| [D4RL](https://github.com/Farama-Foundation/D4RL) | [NeurIPS 2020] Offline RL benchmark covering locomotion, manipulation, and navigation with standardized datasets | [arXiv](https://arxiv.org/abs/2004.07219) · [GitHub](https://github.com/Farama-Foundation/D4RL) |
| [DeepMind Control Suite](https://github.com/google-deepmind/dm_control) | [JMLR 2020] Continuous control tasks for locomotion and manipulation used as standard RL/VLA baselines | [arXiv](https://arxiv.org/abs/2006.12983) · [GitHub](https://github.com/google-deepmind/dm_control) |
| [Adroit](https://github.com/aravindr93/hand_dapg) | [RSS 2018] 24-DoF anthropomorphic hand benchmark for pen, door, hammer, and relocate tasks | [arXiv](https://arxiv.org/abs/1709.10087) · [GitHub](https://github.com/aravindr93/hand_dapg) |

### Embodied Navigation

Benchmarks requiring agents to navigate in 3D environments guided by language or vision.

| Name | Highlights | References |
|------|-----------|------------|
| [GOAT-Bench](https://mukulkhanna.github.io/goat-bench/) | [CVPR 2024] Multi-modal lifelong navigation benchmark with sequential object goals specified by category, language, or image in open-vocabulary settings | [GitHub](https://github.com/Ram81/goat-bench) · [Website](https://mukulkhanna.github.io/goat-bench/) |
| [OpenEQA](https://open-eqa.github.io/) | [CVPR 2024] Embodied Question Answering in the era of foundation models with 1600+ questions spanning spatial, object, and functional understanding | [arXiv](https://arxiv.org/abs/2402.07351) · [GitHub](https://github.com/facebookresearch/open-eqa) · [Website](https://open-eqa.github.io/) |
| [ScanQA](https://github.com/ATR-DBI/ScanQA) | [CVPR 2022] Spatial question answering grounded in 3D indoor point cloud environments | [arXiv](https://arxiv.org/abs/2112.10482) · [GitHub](https://github.com/ATR-DBI/ScanQA) |
| [SOON](https://scenario-oriented-object-navigation.github.io/) | [CVPR 2021] Scenario-oriented object navigation requiring reasoning about object-scene relations | [arXiv](https://arxiv.org/abs/2103.17138) · [Website](https://scenario-oriented-object-navigation.github.io/) |
| [ImageNav](https://github.com/facebookresearch/image-goal-nav-dataset) | [ICCV 2021] Navigation to a goal specified by an image rather than a category label | [GitHub](https://github.com/facebookresearch/image-goal-nav-dataset) |
| [VLN-BERT / HAMT](https://github.com/cshizhe/VLN-BERT) | [CVPR 2021] BERT-based and history-aware transformer approaches evaluated on R2R and REVERIE | [arXiv](https://arxiv.org/abs/2011.13922) · [GitHub](https://github.com/cshizhe/VLN-BERT) |
| [MultiON](https://multinav.github.io/) | [CVPR 2021] Multi-object navigation requiring sequential finding of multiple target objects | [arXiv](https://arxiv.org/abs/2012.03912) · [Website](https://multinav.github.io/) |
| [RxR (Room-Across-Rooms)](https://github.com/google-research-datasets/RxR) | [EMNLP 2020] Multilingual navigation in 3 languages with denser annotations than R2R | [arXiv](https://arxiv.org/abs/2010.07954) · [GitHub](https://github.com/google-research-datasets/RxR) |
| [REVERIE](https://yuankaiqi.github.io/REVERIE_Challenge/) | [CVPR 2020] Combines long-horizon navigation with object grounding via referring expressions | [arXiv](https://arxiv.org/abs/1904.10151) · [GitHub](https://github.com/YuankaiQi/REVERIE) · [Website](https://yuankaiqi.github.io/REVERIE_Challenge/) |
| [ObjectNav (Habitat)](https://aihabitat.org/) | [NeurIPS 2020] Navigate to a specified object category in novel photorealistic environments | [arXiv](https://arxiv.org/abs/2006.13171) · [Website](https://aihabitat.org/) |
| [VLN-CE](https://github.com/jacobkrantz/VLN-CE) | [EMNLP 2020] Continuous-environment R2R in Habitat without discrete viewpoint teleportation | [arXiv](https://arxiv.org/abs/2004.02857) · [GitHub](https://github.com/jacobkrantz/VLN-CE) |
| [CVDN](https://github.com/mmurray/cvdn) | [CVPR 2019] Cooperative multi-turn dialogue navigation where a helper guides an agent to a target | [arXiv](https://arxiv.org/abs/1907.04957) · [GitHub](https://github.com/mmurray/cvdn) |
| [TOUCHDOWN](https://github.com/lil-lab/touchdown) | [CVPR 2019] Street-view navigation in real-world NYC following natural language descriptions | [arXiv](https://arxiv.org/abs/1811.12354) · [GitHub](https://github.com/lil-lab/touchdown) |
| [R2R (Room-to-Room)](https://bringmeaspoon.org/) | [CVPR 2018] Foundational VLN benchmark for instruction-following navigation in Matterport3D | [arXiv](https://arxiv.org/abs/1711.07280) · [GitHub](https://github.com/peteanderson80/Matterport3DSimulator) · [Website](https://bringmeaspoon.org/) |
| [EQA (Embodied Question Answering)](https://embodiedqa.org/) | [CVPR 2018] Agents navigate and answer visual questions about indoor environments | [arXiv](https://arxiv.org/abs/1711.11543) · [Website](https://embodiedqa.org/) |
| [MP3D (Matterport3D)](https://niessner.github.io/Matterport/) | [CVPR 2017] Large-scale RGB-D indoor dataset widely used as a navigation substrate | [Website](https://niessner.github.io/Matterport/) |

### Embodied Multi-Task & Household

Benchmarks combining navigation, manipulation, and reasoning in household or open-world settings.

| Name | Highlights | References |
|------|-----------|------------|
| [Habitat 3.0](https://aihabitat.org/) | [ICLR 2024] Social navigation, collaboration, and rearrangement tasks in embodied AI simulation | [arXiv](https://arxiv.org/abs/2310.13724) · [GitHub](https://github.com/facebookresearch/habitat-sim) · [Website](https://aihabitat.org/) |
| [EmbodiedBench](https://embodiedbench.github.io/) | [ICML 2025] Comprehensive benchmark evaluating MLLMs as embodied agents across 1128 tasks spanning high-level (household, habitat) and low-level (manipulation, navigation) with 6 capability dimensions | [arXiv](https://arxiv.org/abs/2502.09560) · [GitHub](https://github.com/EmbodiedBench/EmbodiedBench) · [Website](https://embodiedbench.github.io/) |
| [ARNOLD](https://arnold-benchmark.github.io/) | [ICCV 2023] Language-conditioned articulated object state change tasks in 3D scenes | [arXiv](https://arxiv.org/abs/2304.04321) · [GitHub](https://github.com/arnold-benchmark/arnold) · [Website](https://arnold-benchmark.github.io/) |
| [TEACh](https://github.com/alexa/teach) | [AAAI 2022] Task completion in AI2-THOR via multi-turn dialogue history | [arXiv](https://arxiv.org/abs/2202.03488) · [GitHub](https://github.com/alexa/teach) |
| [ProcTHOR](https://procthor.allenai.org/) | [NeurIPS 2022] Procedurally generated AI2-THOR houses for training and evaluating generalist embodied agents | [arXiv](https://arxiv.org/abs/2206.06994) · [GitHub](https://github.com/allenai/procthor) · [Website](https://procthor.allenai.org/) |
| [ALFWorld](https://alfworld.github.io/) | [ICLR 2021] Aligns TextWorld with AI2-THOR for language-conditioned household task completion | [arXiv](https://arxiv.org/abs/2010.03768) · [GitHub](https://github.com/alfworld/alfworld) · [Website](https://alfworld.github.io/) |
| [ThreeDWorld (TDW)](https://www.threedworld.org/) | [NeurIPS 2021] Multi-modal physical simulation for transport, manipulation, and multi-agent tasks | [arXiv](https://arxiv.org/abs/2007.04954) · [GitHub](https://github.com/threedworld-mit/tdw) · [Website](https://www.threedworld.org/) |
| [Watch-And-Help](https://github.com/xavierpuigf/watch_and_help) | [ICLR 2021] Social intelligence benchmark for agent cooperation in VirtualHome environments | [arXiv](https://arxiv.org/abs/2010.09890) · [GitHub](https://github.com/xavierpuigf/watch_and_help) |
| [AI2-THOR](https://ai2thor.allenai.org/) | [CVPR 2018] Interactive 3D household simulation with physics for pick-and-place, slicing, cooking, and more | [arXiv](https://arxiv.org/abs/1712.05474) · [GitHub](https://github.com/allenai/ai2thor) · [Website](https://ai2thor.allenai.org/) |
| [VirtualHome](http://virtual-home.org/) | [CVPR 2018] Multi-step household simulation supporting natural language program execution | [arXiv](https://arxiv.org/abs/1806.07011) · [GitHub](https://github.com/xavierpuigf/virtualhome) · [Website](http://virtual-home.org/) |
| [BEHAVIOR-1K](https://behavior.stanford.edu/) | 1000 household activities grounded in real human needs, simulated in OmniGibson | [GitHub](https://github.com/StanfordVL/BEHAVIOR-1K) · [Website](https://behavior.stanford.edu/) |
| [LANMP](https://github.com/h2r/LANMP) | Language-conditioned navigation and manipulation on a real mobile manipulator | [arXiv](https://arxiv.org/abs/2312.02937) · [GitHub](https://github.com/h2r/LANMP) |

### Social & Human-Robot Interaction

Benchmarks for collaborative, communicative, and socially-aware robot behavior.

| Name | Highlights | References |
|------|-----------|------------|
| [Habitat 3.0 Social Nav](https://aihabitat.org/) | [ICLR 2024] Social navigation requiring robots to move around humans and follow social norms | [arXiv](https://arxiv.org/abs/2310.13724) · [Website](https://aihabitat.org/) |
| [ConcepFusion / LangNav](https://github.com/concept-fusion/concept-fusion) | [RSS 2023] Open-vocabulary 3D feature fields enabling natural language queries for navigation | [arXiv](https://arxiv.org/abs/2302.07241) · [GitHub](https://github.com/concept-fusion/concept-fusion) |
| [TDW-Social](https://www.threedworld.org/) | [NeurIPS 2021] Multi-agent social simulation requiring cooperation and communication in TDW | [arXiv](https://arxiv.org/abs/2007.04954) · [GitHub](https://github.com/threedworld-mit/tdw) · [Website](https://www.threedworld.org/) |
| [SEAN](https://sean.interactive-machines.com/) | [RA-L 2020] Navigation benchmark requiring socially compliant behavior around pedestrians | [arXiv](https://arxiv.org/abs/2009.14684) · [Website](https://sean.interactive-machines.com/) |
| [RoboTHOR Challenge](https://ai2thor.allenai.org/robothor/) | ObjectNav challenge bridging simulation and real robot deployment in home-like environments | [arXiv](https://arxiv.org/abs/2004.06799) · [Website](https://ai2thor.allenai.org/robothor/) |
| [ProCo](https://github.com/ProCo-benchmark) | Proactive cooperation benchmark requiring initiative and dialogue from embodied agents | [GitHub](https://github.com/ProCo-benchmark) |

---

## Autonomous Driving

Benchmarks for vision-language grounded driving decisions and planning.

| Name | Highlights | References |
|------|-----------|------------|
| [DriveLM](https://github.com/OpenDriveLab/DriveLM) | [ECCV 2024] Graph-structured vision-language QA benchmark for end-to-end driving on nuScenes | [arXiv](https://arxiv.org/abs/2312.14150) · [GitHub](https://github.com/OpenDriveLab/DriveLM) · [HF](https://huggingface.co/datasets/OpenDriveLab/DriveLM) |
| [LingoQA](https://github.com/wayveai/LingoQA) | [CVPR 2024] Video QA benchmark for driving scene understanding grounded in real-world footage | [arXiv](https://arxiv.org/abs/2312.14751) · [GitHub](https://github.com/wayveai/LingoQA) |
| [Rank2Tell](https://github.com/LLVM-AD/rank2tell) | [WACV 2024] Dataset for ranking and describing important objects in driving scenes | [arXiv](https://arxiv.org/abs/2309.11726) · [GitHub](https://github.com/LLVM-AD/rank2tell) |
| [MAPLM](https://github.com/LLVM-AD/MAPLM) | [WACV 2024] Map-based language model benchmark for understanding HD maps in autonomous driving | [arXiv](https://arxiv.org/abs/2310.04821) · [GitHub](https://github.com/LLVM-AD/MAPLM) |
| [NuScenes-QA](https://github.com/qiantianwen/NuScenes-QA) | [AAAI 2024] 460k QA pairs for visual question answering built on nuScenes | [arXiv](https://arxiv.org/abs/2305.14836) · [GitHub](https://github.com/qiantianwen/NuScenes-QA) |
| [TOD3Cap](https://github.com/jxbbb/TOD3Cap) | [ECCV 2024] 3D dense captioning for autonomous driving with 2.3M natural language descriptions | [arXiv](https://arxiv.org/abs/2403.14680) · [GitHub](https://github.com/jxbbb/TOD3Cap) |
| [DriveVLM](https://tsinghua-mars-lab.github.io/DriveVLM/) | [CoRL 2024] Chain-of-thought VLM reasoning integrated with motion planning for autonomous driving | [arXiv](https://arxiv.org/abs/2406.03230) · [Website](https://tsinghua-mars-lab.github.io/DriveVLM/) |
| [MMAD](https://github.com/MMAD-Benchmark/MMAD) | [NeurIPS 2024] Massive multimodal AD benchmark with 18 perception and reasoning subtasks | [arXiv](https://arxiv.org/abs/2408.12622) · [GitHub](https://github.com/MMAD-Benchmark/MMAD) |
| [nuScenes](https://www.nuscenes.org/) | [CVPR 2020] Large-scale AD dataset with 3D bounding boxes, HD maps, and rich multi-sensor data | [GitHub](https://github.com/nutonomy/nuscenes-devkit) · [Website](https://www.nuscenes.org/) |
| [Waymo Open Dataset](https://waymo.com/open/) | [CVPR 2020] High-quality driving dataset with LiDAR and camera data for perception and prediction | [Website](https://waymo.com/open/) |
| [BDD-X](https://github.com/JinkyuKimUCB/explainable-deep-driving) | [ECCV 2018] Explainable driving dataset with textual descriptions and justifications for actions | [arXiv](https://arxiv.org/abs/1807.11546) · [GitHub](https://github.com/JinkyuKimUCB/explainable-deep-driving) |
| [CARLA Challenge](https://leaderboard.carla.org/) | [CoRL 2017] Open urban driving simulation benchmark for route completion and safety compliance | [GitHub](https://github.com/carla-simulator/leaderboard) · [Website](https://leaderboard.carla.org/) |
| [nuPlan](https://nuplan.org/) | Closed-loop motion planning benchmark with expert demonstrations and reactive simulation | [arXiv](https://arxiv.org/abs/2106.11810) · [GitHub](https://github.com/motional/nuplan-devkit) · [Website](https://nuplan.org/) |
| [DriveBench](https://drive-bench.github.io/) | Comprehensive benchmark evaluating VLMs across multiple driving perception and QA tasks | [Website](https://drive-bench.github.io/) |
| [VLAAD](https://github.com/keyanzhai/VLAAD) | Vision-Language-Action benchmark for autonomous driving with natural language instructions | [GitHub](https://github.com/keyanzhai/VLAAD) |
| [LaMPilot](https://github.com/PurdueDigitalTwin/LaMPilot) | [CVPR 2024] Open benchmark dataset for autonomous driving evaluated via language model programs | [arXiv](https://arxiv.org/abs/2312.04489) · [GitHub](https://github.com/PurdueDigitalTwin/LaMPilot) |
| [STSBench](https://github.com/LRP-IVC/STSBench) | Spatio-temporal scenario benchmark for evaluating MLLMs in interactive autonomous driving scenarios | [GitHub](https://github.com/LRP-IVC/STSBench) |
| [Drive4C](https://github.com/porscheofficial/Drive4C) | Closed-loop benchmark assessing what foundation models need to enable language-guided autonomous driving | [GitHub](https://github.com/porscheofficial/Drive4C) |
| [NAVSIM](https://github.com/autonomousvision/navsim) | [NeurIPS 2024] Non-reactive simulation benchmark for data-driven autonomous driving evaluation with 1000+ hours of real-world driving data | [arXiv](https://arxiv.org/abs/2406.15349) · [GitHub](https://github.com/autonomousvision/navsim) |
| [Bench2Drive](https://github.com/Thinklab-SJTU/Bench2Drive) | Closed-loop multi-ability benchmark for end-to-end autonomous driving across 220 scenarios in CARLA covering perception, prediction, and planning | [arXiv](https://arxiv.org/abs/2406.03877) · [GitHub](https://github.com/Thinklab-SJTU/Bench2Drive) |

---

## GUI & Computer-Use Agents

Benchmarks where a VLA agent perceives a screen (GUI) and takes keyboard/mouse actions.

| Name | Highlights | References |
|------|-----------|------------|
| [AndroidWorld](https://google-research.github.io/android_world/) | [ICLR 2025] 116 programmatic tasks across 20 real Android apps | [arXiv](https://arxiv.org/abs/2405.14573) · [GitHub](https://github.com/google-research/android_world) · [Website](https://google-research.github.io/android_world/) |
| [GUI-Odyssey](https://github.com/OpenGVLab/GUI-Odyssey) | [ICCV 2025] Cross-app Android navigation requiring multi-step actions across multiple apps | [arXiv](https://arxiv.org/abs/2406.08451) · [GitHub](https://github.com/OpenGVLab/GUI-Odyssey) |
| [WebArena](https://webarena.dev/) | [ICLR 2024] 812 realistic tasks across e-commerce, social, coding, and content websites | [arXiv](https://arxiv.org/abs/2307.13854) · [GitHub](https://github.com/web-arena-x/webarena) · [Website](https://webarena.dev/) |
| [VisualWebArena](https://jykoh.com/vwa) | [ACL 2024] Extends WebArena with visually grounded tasks requiring image-based reasoning | [arXiv](https://arxiv.org/abs/2401.13649) · [GitHub](https://github.com/web-arena-x/visualwebarena) · [Website](https://jykoh.com/vwa) |
| [OSWorld](https://os-world.github.io/) | [NeurIPS 2024] 369 open-ended computer tasks in real OS environments (Ubuntu, Windows, macOS) | [arXiv](https://arxiv.org/abs/2404.07972) · [GitHub](https://github.com/xlang-ai/OSWorld) · [HF](https://huggingface.co/datasets/xlangai/OSWorld) · [Website](https://os-world.github.io/) |
| [ScreenSpot](https://github.com/njucckevin/SeeClick) | [ACL 2024] GUI grounding benchmark for localizing UI elements from text instructions | [arXiv](https://arxiv.org/abs/2401.10935) · [GitHub](https://github.com/njucckevin/SeeClick) |
| [AssistGUI](https://showlab.github.io/assistgui/) | [CVPR 2024] Desktop productivity benchmark (Word, Excel, PowerPoint) with video-based evaluation | [arXiv](https://arxiv.org/abs/2312.13108) · [GitHub](https://github.com/showlab/assistgui) · [Website](https://showlab.github.io/assistgui/) |
| [AgentBench](https://llmbench.ai/agent) | [ICLR 2024] LLM-as-agent benchmark with 8 environments: OS, database, web, games, and more | [arXiv](https://arxiv.org/abs/2308.03688) · [GitHub](https://github.com/THUDM/AgentBench) · [Website](https://llmbench.ai/agent) |
| [WorkArena](https://servicenow.github.io/WorkArena/) | [ICML 2024] 33 enterprise software tasks on a real ServiceNow instance | [arXiv](https://arxiv.org/abs/2403.07718) · [GitHub](https://github.com/ServiceNow/WorkArena) · [Website](https://servicenow.github.io/WorkArena/) |
| [SWE-bench](https://swe-bench.github.io/) | [ICLR 2024] Requires agents to resolve real GitHub issues as a software engineering challenge | [arXiv](https://arxiv.org/abs/2310.06770) · [GitHub](https://github.com/swe-bench/SWE-bench) · [Website](https://swe-bench.github.io/) |
| [τ-bench (tau-bench)](https://github.com/sierra-research/tau-bench) | [NeurIPS 2024] Tool-agent-user interaction benchmark evaluating agentic task completion with tool use | [arXiv](https://arxiv.org/abs/2406.12045) · [GitHub](https://github.com/sierra-research/tau-bench) |
| [Mind2Web](https://osu-nlp-group.github.io/Mind2Web/) | [NeurIPS 2023] 2000+ tasks from 137 real-world websites for generalist web agent evaluation | [GitHub](https://github.com/OSU-NLP-Group/Mind2Web) · [Website](https://osu-nlp-group.github.io/Mind2Web/) |
| [AITW (Android in the Wild)](https://github.com/google-research/google-research/tree/master/android_in_the_wild) | [NeurIPS 2023] Large-scale human demonstration dataset on Android devices across diverse tasks | [arXiv](https://arxiv.org/abs/2307.10088) · [GitHub](https://github.com/google-research/google-research/tree/master/android_in_the_wild) |
| [WebSRC](https://x-lance.github.io/WebSRC/) | [EMNLP 2021] Structural reading comprehension for understanding web page layouts and content | [arXiv](https://arxiv.org/abs/2101.09465) · [GitHub](https://github.com/X-LANCE/WebSRC) · [Website](https://x-lance.github.io/WebSRC/) |
| [Screen2Words](https://github.com/google-research-datasets/screen2words) | [UIST 2021] 112k human-annotated mobile UI screen summaries for screen captioning | [arXiv](https://arxiv.org/abs/2108.03353) · [GitHub](https://github.com/google-research-datasets/screen2words) |
| [MiniWob++](https://miniwob.farama.org/) | [ICLR 2018] 100+ browser mini-tasks (clicking, typing, form filling) for web interaction | [GitHub](https://github.com/Farama-Foundation/miniwob-plusplus) · [Website](https://miniwob.farama.org/) |
| [WindowsAgentArena](https://microsoft.github.io/WindowsAgentArena/) | 154 Windows OS tasks spanning productivity, web, and system applications | [arXiv](https://arxiv.org/abs/2409.08264) · [GitHub](https://github.com/microsoft/WindowsAgentArena) · [Website](https://microsoft.github.io/WindowsAgentArena/) |
| [ScreenSpot-Pro](https://github.com/likaixin2000/ScreenSpot-Pro-GUI-Grounding) | GUI grounding benchmark for professional high-resolution computer use across complex desktop applications | [arXiv](https://arxiv.org/abs/2501.11747) · [GitHub](https://github.com/likaixin2000/ScreenSpot-Pro-GUI-Grounding) |
| [Spider2-V](https://spider2-v.github.io/) | [NeurIPS 2024] 494 tasks testing multimodal agents at automating real-world data science and engineering workflows | [arXiv](https://arxiv.org/abs/2407.10956) · [GitHub](https://github.com/xlang-ai/Spider2-V) · [Website](https://spider2-v.github.io/) |
| [GUI-World](https://gui-world.github.io/) | Comprehensive GUI benchmark for evaluating multimodal agents across mobile, web, and desktop interfaces with sequential tasks and QA scenarios | [arXiv](https://arxiv.org/abs/2406.10819) · [GitHub](https://github.com/Dongping-Chen/GUI-World) · [Website](https://gui-world.github.io/) |
| [AndroidLab](https://android-lab-leaderboard.github.io/) | [ICLR 2025] Systematic environment and benchmark for training and evaluating Android autonomous agents across 138 tasks in 9 apps | [arXiv](https://arxiv.org/abs/2410.24024) · [GitHub](https://github.com/THUDM/Android-Lab) · [Website](https://android-lab-leaderboard.github.io/) |
| [OmniACT](https://microsoft.github.io/OmniACT/) | Dataset and benchmark for multimodal autonomous agents performing computer tasks via UI element grounding across desktop and web interfaces | [arXiv](https://arxiv.org/abs/2402.17553) · [GitHub](https://github.com/microsoft/OmniACT) · [Website](https://microsoft.github.io/OmniACT/) |
| [AgentTrek](https://agent-trek.github.io/) | Automated GUI agent trajectory synthesis benchmark derived from web tutorials with 15K+ step-level annotations for agent training and evaluation | [arXiv](https://arxiv.org/abs/2412.09181) · [GitHub](https://github.com/xlang-ai/AgentTrek) · [Website](https://agent-trek.github.io/) |

---

## Game & Interactive Environments

Benchmarks in game or simulated worlds requiring sequential decision-making with language.

| Name | Highlights | References |
|------|-----------|------------|
| [Voyager / DEPS](https://voyager.minedojo.org/) | [NeurIPS 2023] LLM-powered lifelong learning Minecraft agent evaluation framework | [arXiv](https://arxiv.org/abs/2305.16291) · [GitHub](https://github.com/MineDojo/Voyager) · [Website](https://voyager.minedojo.org/) |
| [MineRL / MineDojo](https://minedojo.org/) | [NeurIPS 2022] 3000+ open-ended Minecraft tasks leveraging internet-scale video knowledge | [arXiv](https://arxiv.org/abs/2206.08853) · [GitHub](https://github.com/MineDojo/MineDojo) · [Website](https://minedojo.org/) |
| [ScienceWorld](https://sciworld.apps.allenai.org/) | [EMNLP 2022] 30 science experiment tasks requiring procedural multi-step reasoning and action | [arXiv](https://arxiv.org/abs/2203.07540) · [GitHub](https://github.com/allenai/ScienceWorld) · [Website](https://sciworld.apps.allenai.org/) |
| [CrafterBench](https://github.com/danijar/crafter) | [TMLR 2022] Open-world survival game measuring 22 achievements requiring long-horizon planning | [arXiv](https://arxiv.org/abs/2109.07990) · [GitHub](https://github.com/danijar/crafter) |
| [BEHAVIOR (iGibson)](https://behavior.stanford.edu/) | [NeurIPS 2021] 100 household activities in iGibson simulation requiring physical commonsense reasoning | [GitHub](https://github.com/StanfordVL/behavior) · [Website](https://behavior.stanford.edu/) |
| [NetHack Learning Environment (NLE)](https://github.com/facebookresearch/nle) | [NeurIPS 2020] Complex roguelike game for long-horizon decision making and language-conditioned play | [arXiv](https://arxiv.org/abs/2006.13760) · [GitHub](https://github.com/facebookresearch/nle) |
| [Atari-HEAD](https://github.com/Atari-HEAD/Atari-HEAD) | [AAAI 2019] Human eye-tracking data for Atari games enabling human-like visual attention evaluation | [arXiv](https://arxiv.org/abs/1903.06754) · [GitHub](https://github.com/Atari-HEAD/Atari-HEAD) |
| [BabyAI](https://github.com/mila-iqia/babyai) | [ICLR 2019] Gridworld benchmark with 19 procedurally generated instruction difficulty levels | [arXiv](https://arxiv.org/abs/1810.08272) · [GitHub](https://github.com/mila-iqia/babyai) |
| [GROOT](https://github.com/GreyCampus/GROOT) | Open-ended Minecraft agent benchmark with skill learning and generalization | [GitHub](https://github.com/GreyCampus/GROOT) |
| [MiniGrid / MiniWorld](https://github.com/Farama-Foundation/Minigrid) | Lightweight 2D/3D grid environments for language-conditioned navigation and reasoning | [GitHub](https://github.com/Farama-Foundation/Minigrid) |
| [TextWorld](https://github.com/microsoft/TextWorld) | Framework for generating and playing text-based adventure games to train language agents | [arXiv](https://arxiv.org/abs/1806.11532) · [GitHub](https://github.com/microsoft/TextWorld) |

---

## Multimodal Perception & Understanding

Benchmarks for evaluating visual, temporal, and language-grounded perception capabilities that underpin VLA models.

### General Multimodal

General-purpose benchmarks for evaluating multimodal reasoning, instruction following, and grounding.

| Name | Highlights | References |
|------|-----------|------------|
| [MMMU](https://mmmu-benchmark.github.io/) | [CVPR 2024] 11.5k expert-level questions across 57 subjects for massive multidisciplinary evaluation | [arXiv](https://arxiv.org/abs/2311.16502) · [GitHub](https://github.com/MMMU-Benchmark/MMMU) · [HF](https://huggingface.co/datasets/MMMU/MMMU) · [Website](https://mmmu-benchmark.github.io/) |
| [MMBench](https://mmbench.opencompass.org.cn/) | [ECCV 2024] Systematic 20-dimension VLM evaluation with 3000 questions | [arXiv](https://arxiv.org/abs/2307.06281) · [GitHub](https://github.com/open-compass/MMBench) · [Website](https://mmbench.opencompass.org.cn/) |
| [SEED-Bench](https://github.com/AILab-CVC/SEED-Bench) | [CVPR 2024] 19K questions across 12 dimensions for multi-granularity generative MLLM evaluation | [arXiv](https://arxiv.org/abs/2307.16125) · [GitHub](https://github.com/AILab-CVC/SEED-Bench) |
| [HallusionBench](https://github.com/tianyi-lab/HallusionBench) | [CVPR 2024] Hallucination detection benchmark for visual understanding in VLMs | [arXiv](https://arxiv.org/abs/2310.14566) · [GitHub](https://github.com/tianyi-lab/HallusionBench) |
| [MMStar](https://mmstar-benchmark.github.io/) | [NeurIPS 2024] 1500 carefully curated samples minimizing data leakage and requiring genuine VL reasoning | [arXiv](https://arxiv.org/abs/2403.20330) · [GitHub](https://github.com/MMStar-Benchmark/MMStar) · [Website](https://mmstar-benchmark.github.io/) |
| [CV-Bench](https://github.com/cambridgeltl/cv-bench) | [EMNLP 2024] Compositional reasoning and spatial understanding benchmark for VLMs | [GitHub](https://github.com/cambridgeltl/cv-bench) |
| [BLINK](https://zeyofu.github.io/blink/) | [ECCV 2024] Visual perception benchmark targeting human intuitive abilities that challenge VLMs | [arXiv](https://arxiv.org/abs/2404.12390) · [GitHub](https://github.com/zeyofu/BLINK_Benchmark) · [Website](https://zeyofu.github.io/blink/) |
| [WildVision](https://huggingface.co/spaces/WildVision/vision-arena) | [NeurIPS 2024] Real-world VLM evaluation via human preference collected from live user interactions | [HF](https://huggingface.co/spaces/WildVision/vision-arena) |
| [VLMEvalKit](https://github.com/open-compass/VLMEvalKit) | [ACM MM 2024] Open-source toolkit supporting 100+ VLMs across 50+ benchmarks | [arXiv](https://arxiv.org/abs/2407.11691) · [GitHub](https://github.com/open-compass/VLMEvalKit) |
| [POPE](https://github.com/AoiDragon/POPE) | [EMNLP 2023] Polling-based object probing for evaluating object hallucination in VLMs | [arXiv](https://arxiv.org/abs/2305.10355) · [GitHub](https://github.com/AoiDragon/POPE) |
| [MME](https://github.com/BradyFU/Awesome-Multimodal-Large-Language-Models/tree/Evaluation) | 14-subtask benchmark covering MLLM perception and cognition capabilities | [arXiv](https://arxiv.org/abs/2306.13394) · [GitHub](https://github.com/BradyFU/Awesome-Multimodal-Large-Language-Models) |
| [TouchStone](https://github.com/OFA-Sys/TouchStone) | GPT-4 scored VLM evaluation across 5 ability dimensions | [arXiv](https://arxiv.org/abs/2308.16890) · [GitHub](https://github.com/OFA-Sys/TouchStone) |
| [RealWorldQA](https://x.ai/blog/grok-1.5v) | Real-world spatial understanding benchmark from xAI testing physical world reasoning | [Website](https://x.ai/blog/grok-1.5v) |
| [MMTE](https://github.com/MMTE-benchmark/MMTE) | Multimodal task execution benchmark for following complex visual instructions | [GitHub](https://github.com/MMTE-benchmark/MMTE) |
| [MMIU](https://mmiu-bench.github.io/) | [ICLR 2025] Multimodal Multi-image Understanding benchmark with 7 image-relationship types, 52 tasks, and 11K questions for evaluating LVLMs | [arXiv](https://arxiv.org/abs/2408.02718) · [GitHub](https://github.com/OpenGVLab/MMIU) · [Website](https://mmiu-bench.github.io/) |
| [MathVista](https://mathvista.github.io/) | [ICLR 2024] Mathematical reasoning in visual contexts benchmark requiring compositional reasoning across 28 math tasks and 5 visual types | [arXiv](https://arxiv.org/abs/2310.02255) · [GitHub](https://github.com/lupantech/MathVista) · [Website](https://mathvista.github.io/) |
| [MMMU-Pro](https://mmmu-benchmark.github.io/mmmu-pro/) | [NeurIPS 2024] More robust MMMU extension with college-level expert questions requiring genuine multimodal understanding, resistant to language-only shortcuts | [arXiv](https://arxiv.org/abs/2409.02813) · [GitHub](https://github.com/MMMU-Benchmark/MMMU-Pro) · [Website](https://mmmu-benchmark.github.io/mmmu-pro/) |
| [CharXiv](https://charxiv.github.io/) | [NeurIPS 2024] Chart understanding benchmark exposing significant gaps in VLMs on 2323 scientific paper figures with descriptive and reasoning tasks | [arXiv](https://arxiv.org/abs/2406.18521) · [GitHub](https://github.com/princeton-nlp/CharXiv) · [Website](https://charxiv.github.io/) |
| [OlympiadBench](https://github.com/OpenBMB/OlympiadBench) | [ACL 2024] Olympiad-level bilingual multimodal science benchmark with 8952 problems in mathematics and physics for frontier VLM evaluation | [arXiv](https://arxiv.org/abs/2402.14008) · [GitHub](https://github.com/OpenBMB/OlympiadBench) |
| [MEGA-Bench](https://tiger-ai-lab.github.io/MEGA-Bench/) | [NeurIPS 2024] Scaling multimodal evaluation to 500+ diverse real-world tasks covering perception, reasoning, and generation across many domains | [arXiv](https://arxiv.org/abs/2410.10563) · [GitHub](https://github.com/TIGER-AI-Lab/MEGA-Bench) · [Website](https://tiger-ai-lab.github.io/MEGA-Bench/) |
| [MM-Vet v2](https://github.com/yuweihao/MM-Vet) | Harder and more comprehensive integrated capabilities benchmark for large multimodal models using GPT-4 scoring across 16 skills | [arXiv](https://arxiv.org/abs/2408.00765) · [GitHub](https://github.com/yuweihao/MM-Vet) |

### Video & Temporal Understanding

Benchmarks requiring understanding of temporal dynamics, actions, and causal reasoning in video.

| Name | Highlights | References |
|------|-----------|------------|
| [TemporalBench](https://github.com/mu-cai/TemporalBench) | [ICLR 2025] Fine-grained temporal video understanding benchmark for VLMs with 2M QA pairs | [arXiv](https://arxiv.org/abs/2410.20953) · [GitHub](https://github.com/mu-cai/TemporalBench) |
| [Video-MME](https://video-mme.github.io/) | [CVPR 2025] First comprehensive evaluation benchmark of MLLMs in video analysis covering short/medium/long videos across 30 domains | [arXiv](https://arxiv.org/abs/2405.21075) · [GitHub](https://github.com/MME-Benchmarks/Video-MME) · [Website](https://video-mme.github.io/) |
| [LongVideoBench](https://longvideobench.github.io/) | [NeurIPS 2024] Long-context interleaved video-language understanding benchmark with 6678 questions on videos ranging from minutes to 1 hour | [arXiv](https://arxiv.org/abs/2407.15754) · [GitHub](https://github.com/longvideobench/LongVideoBench) · [Website](https://longvideobench.github.io/) |
| [MLVU](https://github.com/JUNJIE99/MLVU) | [NeurIPS 2024] Multi-task long video understanding benchmark with 9 task types spanning holistic, single-detail, and multi-detail evaluation across 10–180 minute videos | [arXiv](https://arxiv.org/abs/2406.04264) · [GitHub](https://github.com/JUNJIE99/MLVU) |
| [MVBench](https://github.com/OpenGVLab/Ask-Anything) | [CVPR 2024] 20 challenging temporal reasoning tasks for multi-task video understanding | [arXiv](https://arxiv.org/abs/2311.17437) · [GitHub](https://github.com/OpenGVLab/Ask-Anything) |
| [EgoTaskQA](https://github.com/Buzz-Beater/EgoTaskQA) | [NeurIPS 2022] Egocentric video QA with task goal inference, procedural reasoning, and state tracking | [arXiv](https://arxiv.org/abs/2210.03929) · [GitHub](https://github.com/Buzz-Beater/EgoTaskQA) |
| [STAR (Situated Reasoning)](https://bobbywu.com/STAR/) | [NeurIPS 2021] Situated temporal action reasoning with 4 question types grounded in real videos | [arXiv](https://arxiv.org/abs/2105.09912) · [Website](https://bobbywu.com/STAR/) |
| [NExT-QA](https://doc-doc.github.io/docs/nextqa.html) | [CVPR 2021] Video QA benchmark emphasizing causal and temporal reasoning about actions | [arXiv](https://arxiv.org/abs/2105.08276) · [GitHub](https://github.com/doc-doc/NExT-QA) · [Website](https://doc-doc.github.io/docs/nextqa.html) |
| [COIN](https://coin-dataset.github.io/) | [CVPR 2019] 11,827 instructional videos across 180 tasks and 778 procedural steps | [arXiv](https://arxiv.org/abs/1903.02874) · [GitHub](https://github.com/coin-dataset/annotations) · [Website](https://coin-dataset.github.io/) |
| [CrossTask](https://github.com/DmZhukov/CrossTask) | [CVPR 2019] Procedural activity understanding across 83 instructional video tasks | [arXiv](https://arxiv.org/abs/1903.08675) · [GitHub](https://github.com/DmZhukov/CrossTask) |
| [HowTo100M](https://www.di.ens.fr/willow/research/howto100m/) | [ICCV 2019] Narrated instructional videos for learning action-language grounding at scale | [arXiv](https://arxiv.org/abs/1906.03327) · [Website](https://www.di.ens.fr/willow/research/howto100m/) |
| [Something-Something v2](https://developer.qualcomm.com/software/ai-datasets/something-something) | [ICCV 2017] Temporal reasoning requiring understanding of object interactions and motion direction | [arXiv](https://arxiv.org/abs/1706.04261) · [Website](https://developer.qualcomm.com/software/ai-datasets/something-something) |
| [Charades](https://prior.allenai.org/projects/charades) | [ECCV 2016] Indoor activity dataset requiring temporal localization and compositional reasoning | [arXiv](https://arxiv.org/abs/1705.02101) · [Website](https://prior.allenai.org/projects/charades) |
| [ActivityNet](http://activity-net.org/) | [CVPR 2015] Activity recognition, localization, and dense video captioning at large scale | [arXiv](https://arxiv.org/abs/1506.01707) · [Website](http://activity-net.org/) |
| [Kinetics-700](https://www.deepmind.com/open-source/kinetics) | Large-scale action recognition dataset with 700 human action classes | [arXiv](https://arxiv.org/abs/1907.06987) · [Website](https://www.deepmind.com/open-source/kinetics) |
| [Video-Bench](https://github.com/PKU-YuanGroup/Video-Bench) | Video-exclusive benchmark for evaluating video understanding capabilities in MLLMs | [arXiv](https://arxiv.org/abs/2311.16103) · [GitHub](https://github.com/PKU-YuanGroup/Video-Bench) |
| [VideoVista](https://github.com/HITsz-TMG/VideoVista) | Diverse video understanding benchmark spanning 14 task types and 35 categories | [arXiv](https://arxiv.org/abs/2406.11303) · [GitHub](https://github.com/HITsz-TMG/VideoVista) |
| [DREAM-1K](https://github.com/TNT-Robotics/DREAM-1K) | Procedural video understanding benchmark for evaluating robot task planning | [arXiv](https://arxiv.org/abs/2312.04519) · [GitHub](https://github.com/TNT-Robotics/DREAM-1K) |

### Egocentric & Activity

Benchmarks from a first-person perspective, closely aligned with robot/agent perception.

| Name | Highlights | References |
|------|-----------|------------|
| [Ego-Exo4D](https://ego-exo4d-data.org/) | [CVPR 2024] Paired egocentric and exocentric video dataset for skill assessment and correspondence | [arXiv](https://arxiv.org/abs/2311.18259) · [Website](https://ego-exo4d-data.org/) |
| [Ego4D](https://ego4d-data.org/) | [CVPR 2022] 3670h egocentric video with benchmarks for episodic memory, forecasting, and hand-object interaction | [arXiv](https://arxiv.org/abs/2110.07058) · [GitHub](https://github.com/facebookresearch/Ego4d) · [Website](https://ego4d-data.org/) |
| [EPIC-Kitchens-100](https://epic-kitchens.github.io/) | [IJCV 2022] 100 hours of unscripted egocentric cooking actions with fine-grained annotations | [arXiv](https://arxiv.org/abs/2006.13256) · [GitHub](https://github.com/epic-kitchens/epic-kitchens-100-annotations) · [Website](https://epic-kitchens.github.io/) |
| [Assembly101](https://assembly-101.github.io/) | [CVPR 2022] Egocentric procedural dataset for assembling and disassembling 101 toy vehicles | [arXiv](https://arxiv.org/abs/2203.14712) · [GitHub](https://github.com/assembly-101/assembly101-annotations) · [Website](https://assembly-101.github.io/) |
| [HOI4D](https://hoi4d.github.io/) | [CVPR 2022] Egocentric 4D dataset for category-level human-object interaction manipulation | [arXiv](https://arxiv.org/abs/2203.01577) · [GitHub](https://github.com/leolyliu/HOI4D-Instructions) · [Website](https://hoi4d.github.io/) |
| [EgoProceL](https://github.com/Sid2697/EgoProceL) | [ECCV 2022] Egocentric procedural learning benchmark for keystep recognition from instructional videos | [arXiv](https://arxiv.org/abs/2206.11173) · [GitHub](https://github.com/Sid2697/EgoProceL) |
| [LEMMA](https://sites.google.com/view/lemma-activity) | [ECCV 2020] Multi-person, multi-task dataset for compositional action understanding | [arXiv](https://arxiv.org/abs/2007.03152) · [Website](https://sites.google.com/view/lemma-activity) |
| [EGTEA Gaze+](https://cbs.ic.gatech.edu/fpv/) | [ECCV 2018] First-person cooking dataset with gaze and hand masks for fine-grained recognition | [arXiv](https://arxiv.org/abs/1801.09014) · [Website](https://cbs.ic.gatech.edu/fpv/) |
| [EPIC-Kitchens Challenges](https://epic-kitchens.github.io/2024) | Annual challenges on action recognition, detection, anticipation, and retrieval | [Website](https://epic-kitchens.github.io/2024) |
| [EgoPlan-Bench](https://github.com/ChenYi99/EgoPlan) | [IJCV 2024] Benchmarking MLLMs for human-level task planning from egocentric video with real-world household scenarios | [arXiv](https://arxiv.org/abs/2312.06722) · [GitHub](https://github.com/ChenYi99/EgoPlan) |

### 3D Scene Understanding

Benchmarks for grounding language in 3D space, enabling perception for embodied action.

| Name | Highlights | References |
|------|-----------|------------|
| [EmbodiedScan](https://tai-wang.github.io/embodiedscan/) | [CVPR 2024] Holistic 3D perception benchmark with RGB-D input from egocentric views | [arXiv](https://arxiv.org/abs/2312.16170) · [GitHub](https://github.com/OpenRobotLab/EmbodiedScan) · [Website](https://tai-wang.github.io/embodiedscan/) |
| [LEO](https://embodied-generalist.github.io/) | [ICML 2024] Embodied generalist benchmark requiring 3D scene understanding for grounded dialogue and planning | [arXiv](https://arxiv.org/abs/2311.12871) · [GitHub](https://github.com/embodied-generalist/embodied-generalist) · [Website](https://embodied-generalist.github.io/) |
| [SQA3D (Situated QA)](https://sqa3d.github.io/) | [ICLR 2023] Situated reasoning benchmark where agents answer questions from a 3D first-person perspective | [arXiv](https://arxiv.org/abs/2210.07474) · [GitHub](https://github.com/SilongYong/SQA3D) · [Website](https://sqa3d.github.io/) |
| [3D-VisTA](https://3d-vista.github.io/) | [ICCV 2023] Pre-trained transformer for 3D VL tasks: grounding, QA, and dense captioning | [arXiv](https://arxiv.org/abs/2308.04352) · [GitHub](https://github.com/3d-vista/3D-VisTA) · [Website](https://3d-vista.github.io/) |
| [MultiScan](https://3dlg-hcvc.github.io/multiscan/) | [NeurIPS 2022] Multi-scan indoor reconstruction with articulated object annotations for VLA research | [arXiv](https://arxiv.org/abs/2212.04477) · [GitHub](https://github.com/3dlg-hcvc/multiscan) · [Website](https://3dlg-hcvc.github.io/multiscan/) |
| [ScanEnts3D](https://github.com/daveredrum/ScanEnts3D) | [ECCV 2022] Links 3D scene entities to text mentions for fine-grained object grounding | [arXiv](https://arxiv.org/abs/2109.04675) · [GitHub](https://github.com/daveredrum/ScanEnts3D) |
| [ScanRefer](https://daveredrum.github.io/ScanRefer/) | [ECCV 2020] Localizes objects in 3D point clouds using free-form language descriptions | [arXiv](https://arxiv.org/abs/1912.08830) · [GitHub](https://github.com/daveredrum/ScanRefer) · [Website](https://daveredrum.github.io/ScanRefer/) |
| [CLEVR3D](https://github.com/yancie-yjr/3d-clevr) | 3D extension of CLEVR for spatial reasoning questions in synthetic environments | [GitHub](https://github.com/yancie-yjr/3d-clevr) |
| [Nu-Scenes QA](https://github.com/qiantianwen/NuScenes-QA) | QA benchmark grounded in outdoor 3D LiDAR scenes for driving reasoning | [arXiv](https://arxiv.org/abs/2305.14836) · [GitHub](https://github.com/qiantianwen/NuScenes-QA) |
| [MMScan](https://tai-wang.github.io/mmscan) | [NeurIPS 2024] Multi-modal 3D scene dataset with 1.4M hierarchical grounded language annotations on 109k objects and benchmarks for visual grounding and QA | [arXiv](https://arxiv.org/abs/2312.16170) · [GitHub](https://github.com/rbler1234/MMScan) · [Website](https://tai-wang.github.io/mmscan) |
| [SceneVerse](https://scene-verse.github.io/) | [ECCV 2024] Large-scale 3D vision-language dataset with 68K indoor scenes and 2.5M language-scene pairs for grounded scene understanding and spatial reasoning | [arXiv](https://arxiv.org/abs/2401.09340) · [GitHub](https://github.com/scene-verse/SceneVerse) · [Website](https://scene-verse.github.io/) |

### Language-Grounded Perception

Benchmarks for visual grounding, referring expression comprehension, and spatial reasoning.

| Name | Highlights | References |
|------|-----------|------------|
| [SeedBench-2-Plus](https://github.com/AILab-CVC/SEED-Bench) | [NeurIPS 2024] Extended SEED-Bench focusing on charts, maps, web pages, and document comprehension | [arXiv](https://arxiv.org/abs/2404.16790) · [GitHub](https://github.com/AILab-CVC/SEED-Bench) |
| [ARO (Attribution, Relation, Order)](https://github.com/mertyg/vision-language-models-are-bows) | [ICLR 2023] Reveals VLMs' limited sensitivity to word order and relational structure | [arXiv](https://arxiv.org/abs/2210.01936) · [GitHub](https://github.com/mertyg/vision-language-models-are-bows) |
| [VSR (Visual Spatial Reasoning)](https://github.com/cambridgeltl/visual-spatial-reasoning) | [NAACL 2022] True/false benchmark testing spatial relationships between objects in images | [arXiv](https://arxiv.org/abs/2205.00363) · [GitHub](https://github.com/cambridgeltl/visual-spatial-reasoning) |
| [Winoground](https://huggingface.co/datasets/facebook/winoground) | [CVPR 2022] Tests visio-linguistic compositional reasoning via image-caption matching with swapped words | [arXiv](https://arxiv.org/abs/2204.03162) · [HF](https://huggingface.co/datasets/facebook/winoground) |
| [FLUTE](https://github.com/google-research/google-research/tree/master/flute) | [EMNLP 2022] Figurative language understanding for VLMs involving metaphors and similes | [arXiv](https://arxiv.org/abs/2205.12404) · [GitHub](https://github.com/google-research/google-research/tree/master/flute) |
| [GQA](https://cs.stanford.edu/people/dorarad/gqa/) | [CVPR 2019] Compositional QA benchmark requiring multi-step spatial and relational reasoning | [arXiv](https://arxiv.org/abs/1902.09506) · [Website](https://cs.stanford.edu/people/dorarad/gqa/) |
| [Visual Genome](https://visualgenome.org/) | [IJCV 2017] Densely annotated images with region descriptions, QA, and scene graphs for grounded understanding | [arXiv](https://arxiv.org/abs/1602.07332) · [GitHub](https://github.com/ranjaykrishna/visual_genome_python_driver) · [Website](https://visualgenome.org/) |
| [CLEVR](https://cs.stanford.edu/people/jcjohns/clevr/) | [CVPR 2017] Compositional language and elementary visual reasoning diagnostic benchmark | [arXiv](https://arxiv.org/abs/1612.06890) · [GitHub](https://github.com/facebookresearch/clevr-dataset-gen) · [Website](https://cs.stanford.edu/people/jcjohns/clevr/) |
| [RefCOCO / RefCOCO+ / RefCOCOg](https://github.com/lichengunc/refer) | [ECCV 2016] Referring expression comprehension benchmarks for localizing objects from natural language | [arXiv](https://arxiv.org/abs/1608.00272) · [GitHub](https://github.com/lichengunc/refer) |
| [SpatialBot](https://github.com/BAAI-DCAI/SpatialBot) | Spatial understanding benchmark evaluating depth-aware reasoning in VLMs | [GitHub](https://github.com/BAAI-DCAI/SpatialBot) |

---

## Infrastructure & Resources

Simulation engines, datasets, and evaluation platforms used to build and run VLA benchmarks.

### Simulation Environments & Platforms

Simulation engines and platforms used to construct and run VLA benchmarks.

| Name | Highlights | References |
|------|-----------|------------|
| [IsaacGym](https://developer.nvidia.com/isaac-gym) | [NeurIPS 2021] Legacy GPU physics simulation for massively parallel RL training on dexterous tasks | [arXiv](https://arxiv.org/abs/2108.10470) · [Website](https://developer.nvidia.com/isaac-gym) |
| [Robosuite](https://robosuite.ai/) | [IROS 2021] Modular robot learning framework built on MuJoCo with standardized task suites | [arXiv](https://arxiv.org/abs/2009.12293) · [GitHub](https://github.com/ARISE-Initiative/robosuite) · [Website](https://robosuite.ai/) |
| [SAPIEN](https://sapien.ucsd.edu/) | [CVPR 2020] Simulation platform for articulated object manipulation with PhysX physics | [arXiv](https://arxiv.org/abs/2003.08515) · [GitHub](https://github.com/haosulab/SAPIEN) · [Website](https://sapien.ucsd.edu/) |
| [Habitat-Sim](https://aihabitat.org/) | [ICCV 2019] High-performance 3D simulator for embodied AI with photorealistic rendering and physics | [arXiv](https://arxiv.org/abs/1904.01201) · [GitHub](https://github.com/facebookresearch/habitat-sim) · [Website](https://aihabitat.org/) |
| [CARLA](https://carla.org/) | [CoRL 2017] Open urban driving simulator with rich sensor modalities for autonomous driving research | [arXiv](https://arxiv.org/abs/1711.03938) · [GitHub](https://github.com/carla-simulator/carla) · [Website](https://carla.org/) |
| [MuJoCo](https://mujoco.org/) | [IROS 2012] Fast and accurate physics simulation engine widely used for locomotion and manipulation | [arXiv](https://arxiv.org/abs/2103.14685) · [GitHub](https://github.com/google-deepmind/mujoco) · [Website](https://mujoco.org/) |
| [IsaacSim / IsaacLab](https://developer.nvidia.com/isaac-sim) | NVIDIA's GPU-accelerated simulation platform for robot learning and VLA development | [GitHub](https://github.com/isaac-sim/IsaacLab) · [Website](https://developer.nvidia.com/isaac-sim) |
| [Genesis](https://genesis-world.readthedocs.io/) | Generative simulation engine with ultra-fast physics and photorealistic rendering | [arXiv](https://arxiv.org/abs/2501.10963) · [GitHub](https://github.com/Genesis-Embodied-AI/Genesis) · [Website](https://genesis-world.readthedocs.io/) |
| [PyBullet / Panda-Gym](https://pybullet.org/) | Open-source physics simulation with Panda robot gym environments for tabletop manipulation | [GitHub](https://github.com/bulletphysics/bullet3) · [Website](https://pybullet.org/) |
| [OmniGibson](https://behavior.stanford.edu/omnigibson/) | NVIDIA Omniverse-based simulation for BEHAVIOR-1K with realistic physics and rendering | [arXiv](https://arxiv.org/abs/2403.09227) · [GitHub](https://github.com/StanfordVL/OmniGibson) · [Website](https://behavior.stanford.edu/omnigibson/) |
| [AI2-THOR (Simulator)](https://ai2thor.allenai.org/) | Photorealistic interactive indoor simulation for embodied household task research | [arXiv](https://arxiv.org/abs/1712.05474) · [GitHub](https://github.com/allenai/ai2thor) · [Website](https://ai2thor.allenai.org/) |
| [CoppeliaSim (V-REP)](https://www.coppeliarobotics.com/) | Versatile robot simulation platform underlying RLBench and other benchmarks | [Website](https://www.coppeliarobotics.com/) |
| [SUMO](https://eclipse.dev/sumo/) | Microscopic traffic simulation supporting multi-modal transportation research | [GitHub](https://github.com/eclipse-sumo/sumo) · [Website](https://eclipse.dev/sumo/) |
| [XR-EgoBench](https://github.com/XR-EgoBench) | Extended reality egocentric benchmark platform for AR/VR embodied agent evaluation | [GitHub](https://github.com/XR-EgoBench) |

### Large-Scale Datasets & Model Hubs

Key datasets and hubs that supply training and evaluation data for VLA models.

| Name | Highlights | References |
|------|-----------|------------|
| [HuggingFace LeRobot Datasets](https://huggingface.co/lerobot) | Standardized real-robot demonstration datasets for VLA training and benchmarking | [GitHub](https://github.com/huggingface/lerobot) · [HF](https://huggingface.co/lerobot) |
| [HuggingFace Open-VLA](https://huggingface.co/openvla) | HuggingFace hub for OpenVLA model weights, training data, and evaluation scripts | [GitHub](https://github.com/openvla/openvla) · [HF](https://huggingface.co/openvla) |
| [HuggingFace Robot Benchmarks](https://huggingface.co/collections/lerobot/benchmarks) | Curated collection of robot learning benchmarks and evaluation protocols | [HF](https://huggingface.co/collections/lerobot/benchmarks) |
| [Open X-Embodiment Dataset](https://huggingface.co/datasets/jxu124/OpenX-Embodiment) | HuggingFace mirror of the OXE cross-embodiment dataset aggregating 1M+ robot episodes | [arXiv](https://arxiv.org/abs/2310.08864) · [HF](https://huggingface.co/datasets/jxu124/OpenX-Embodiment) |
| [RoboSet](https://robopen.github.io/roboset/) | Large-scale robot manipulation dataset with 100k+ demonstrations across 12 task categories | [arXiv](https://arxiv.org/abs/2312.07941) · [Website](https://robopen.github.io/roboset/) |
| [DROID Dataset](https://huggingface.co/datasets/rail-berkeley/DROID) | 76k robot manipulation demonstrations on HuggingFace for diverse real-world VLA training | [arXiv](https://arxiv.org/abs/2403.12945) · [HF](https://huggingface.co/datasets/rail-berkeley/DROID) |
| [BridgeData V2 (HF)](https://huggingface.co/datasets/rail-berkeley/bridge_dataset) | HuggingFace version of BridgeData V2 for easy access and VLA pretraining | [arXiv](https://arxiv.org/abs/2308.12952) · [HF](https://huggingface.co/datasets/rail-berkeley/bridge_dataset) |
| [EgoMimic Dataset](https://egomimic.github.io/) | Paired egocentric human video and robot demonstration dataset for VLA transfer learning | [arXiv](https://arxiv.org/abs/2410.24221) · [Website](https://egomimic.github.io/) |
| [RH20T](https://rh20t.github.io/) | Large-scale robotic dataset with 110k demonstrations across 20 tasks | [arXiv](https://arxiv.org/abs/2307.00595) · [GitHub](https://github.com/rh20t/rh20t_api) · [Website](https://rh20t.github.io/) |
| [Ego4D HuggingFace](https://huggingface.co/datasets/lmms-lab/Ego4D) | Ego4D benchmark data accessible via HuggingFace for convenient evaluation | [arXiv](https://arxiv.org/abs/2110.07058) · [HF](https://huggingface.co/datasets/lmms-lab/Ego4D) |

### Leaderboards & Evaluation Platforms

Platforms hosting challenges, competitions, and live leaderboards for VLA models.

| Name | Highlights | References |
|------|-----------|------------|
| [EvalAI](https://eval.ai/) | Cloud-based challenge platform hosting embodied AI, VQA, navigation, and VLA competitions | [Website](https://eval.ai/) |
| [PaperWithCode Embodied AI](https://paperswithcode.com/methods/category/embodied-ai) | Live leaderboards tracking SOTA across navigation, manipulation, and QA benchmarks | [Website](https://paperswithcode.com/methods/category/embodied-ai) |
| [HuggingFace Open VLA Leaderboard](https://huggingface.co/spaces/lerobot/eval_real_world_vla) | Community leaderboard for real-world robot VLA performance | [HF](https://huggingface.co/spaces/lerobot/eval_real_world_vla) |
| [Open-Compass (OpenVLM Leaderboard)](https://rank.opencompass.org.cn/leaderboard-multimodal) | Comprehensive VLM leaderboard comparing models across 50+ benchmarks | [Website](https://rank.opencompass.org.cn/leaderboard-multimodal) |
| [LIBERO Leaderboard](https://libero-project.github.io/main.html) | Official leaderboard for the LIBERO manipulation benchmark suite | [Website](https://libero-project.github.io/main.html) |
| [CARLA Autonomous Driving Leaderboard](https://leaderboard.carla.org/) | Official competition leaderboard for autonomous driving agents in CARLA | [Website](https://leaderboard.carla.org/) |
| [WebArena Leaderboard](https://docs.google.com/spreadsheets/d/1M801lEpBbKSNwP-vDBkC_pF7LdyGU1f_ufZb_NWNBZQ) | Community tracking sheet for web agent performance on WebArena | [Website](https://docs.google.com/spreadsheets/d/1M801lEpBbKSNwP-vDBkC_pF7LdyGU1f_ufZb_NWNBZQ) |
| [OSWorld Leaderboard](https://os-world.github.io/) | Live leaderboard for OS computer-use agents on the OSWorld benchmark | [Website](https://os-world.github.io/) |
| [Ego4D Challenges (EvalAI)](https://eval.ai/web/challenges/list) | Annual Ego4D challenge tracks on episodic memory, forecasting, AV, hands, and narrations | [Website](https://eval.ai/web/challenges/list) |
| [BEHAVIOR-1K Leaderboard](https://behavior.stanford.edu/benchmark-guide.html) | Evaluation results for household activity agents in the BEHAVIOR benchmark | [Website](https://behavior.stanford.edu/benchmark-guide.html) |
| [AgentBench Leaderboard](https://llmbench.ai/agent/data) | Rankings for LLM-as-agent performance across OS, web, game, and database tasks | [Website](https://llmbench.ai/agent/data) |
| [EmbodiedBench Leaderboard](https://embodiedbench.github.io/) | CVPR 2026 challenge leaderboard for MLLM-based embodied agents across high-level and low-level tasks | [Website](https://embodiedbench.github.io/) |

---

## Contributing

Contributions are welcome! To add a benchmark:
1. Fork this repository.
2. Add the entry to the appropriate section in `README.md` following the table format.
3. Submit a pull request.

Please ensure that:
- The benchmark is relevant to VLA or embodied AI evaluation.
- You provide links to the official website, paper, or GitHub repository in the References column.
- The Highlights description is concise (one sentence).

---

## License

[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

This list is released under the [CC0 1.0 Universal](LICENSE) public domain dedication. You are free to copy, modify, and distribute this work, even for commercial purposes, without asking permission.
