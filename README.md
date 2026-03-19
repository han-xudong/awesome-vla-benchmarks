# Awesome VLA Benchmarks [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A comprehensive, curated list of benchmarks for evaluating Vision-Language-Action (VLA) models — organized by application domain, covering embodied robotics, autonomous driving, GUI agents, game environments, multimodal perception, and more.

## Contents

- [Overview](#overview)
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

---

## Overview

**Vision-Language-Action (VLA)** models unify visual perception, natural language understanding, and action generation into a single framework. Unlike pure vision-language models (VLMs), VLA models must produce *grounded, executable actions* in response to multimodal inputs. This list covers benchmarks from **all domains** where this capability is evaluated — including robotics, GUI navigation, autonomous driving, egocentric video, interactive games, and general multimodal reasoning.

---

## Embodied Robotics

Benchmarks for physical or simulated robots that must perceive, reason, and act in the real or virtual world.

### Robot Manipulation

Benchmarks focused on language-conditioned robot arm or bimanual manipulation tasks.

- **[RLBench](https://github.com/stepjam/RLBench)** - A large-scale robot learning benchmark with 100+ unique language-conditioned tasks built on CoppeliaSim.
- **[MetaWorld](https://meta-world.github.io/)** - A multi-task and meta-RL benchmark with 50 distinct tabletop manipulation tasks.
- **[LIBERO](https://libero-project.github.io/)** - A benchmark studying knowledge transfer across 130 language-conditioned manipulation tasks organized into 4 suites.
- **[Calvin](http://calvin.cs.uni-freiburg.de/)** - Long-horizon language-conditioned manipulation benchmark requiring chaining up to 5 tasks in a row.
- **[VIMA-BENCH](https://vimalabs.github.io/)** - A multimodal manipulation benchmark with 17 task types specified via interleaved text and image prompts.
- **[FurnitureBench](https://clvrai.github.io/furniture-bench/)** - Real and simulated furniture assembly benchmark requiring long-horizon dexterous manipulation.
- **[BridgeData V2](https://rail-berkeley.github.io/bridgedata/)** - Large-scale tabletop manipulation dataset with language annotations across diverse kitchen scenes.
- **[Open X-Embodiment (OXE)](https://robotics-transformer-x.github.io/)** - Cross-embodiment dataset aggregating 1M+ robot episodes from 22 institutions and 22 robot types.
- **[DROID](https://droid-dataset.github.io/)** - Large-scale robot manipulation dataset with 76k demonstrations collected across diverse real-world environments.
- **[RoboMimic](https://robomimic.github.io/)** - A benchmark for robot learning from demonstrations with standardized datasets and multiple algorithm baselines.
- **[ManiSkill2](https://maniskill2.github.io/)** - A unified benchmark for generalizable manipulation skills with 20 task families and rigid/soft-body physics.
- **[ManiSkill3](https://maniskill.ai/)** - Next-generation of ManiSkill with GPU-parallelized simulation, richer tasks, and improved evaluation protocols.
- **[RoboCasa](https://robocasa.ai/)** - Large-scale kitchen manipulation benchmark with 100+ tasks and photorealistic environments, built on MuJoCo.
- **[SimplerEnv](https://simpler-env.github.io/)** - A simulation-based evaluation framework designed to match real-world robot performance for VLA comparison.
- **[Franka Kitchen](https://github.com/google-research/relay-policy-learning)** - A multi-task kitchen manipulation benchmark using a Franka Panda robot with 7 subtasks.
- **[ALOHA / ACT](https://tonyzhaozh.github.io/aloha/)** - Low-cost bimanual teleoperation benchmark with demonstrations for imitation learning.
- **[Mobile ALOHA](https://mobile-aloha.github.io/)** - Extension of ALOHA to a mobile whole-body manipulation platform with household tasks.
- **[RoboAgent](https://robopen.github.io/)** - Generalizable manipulation using semantic augmentations evaluated across 12 real-world tasks.
- **[SpatialBench](https://github.com/kahnchana/spatial_bench)** - Evaluation of spatial reasoning capabilities of VLMs applied to manipulation contexts.
- **[Octo](https://octo-models.github.io/)** - Generalist robot policy trained on OXE data, evaluated across BridgeV2, Franka, and other platforms.
- **[π0 (pi-zero)](https://www.physicalintelligence.company/blog/pi0)** - Physical Intelligence's large robot foundation model evaluated on a diverse dexterous task suite.
- **[GR-1](https://github.com/bytedance/GR-1)** - ByteDance's generalist robot manipulation policy evaluated on CALVIN and real-world tasks.
- **[RT-1](https://robotics-transformer1.github.io/)** - Google's Robotics Transformer evaluated on 700+ real-world manipulation tasks.
- **[RT-2](https://robotics-transformer2.github.io/)** - Robotic Transformer 2 combining internet-scale VLM pretraining with robot control evaluation.
- **[OpenVLA](https://openvla.github.io/)** - Open-source VLA model evaluated on BridgeV2 and OXE tasks, available on HuggingFace.

### Dexterous Manipulation & Locomotion

Benchmarks for fine motor skills, multi-fingered hands, and legged/mobile robots.

- **[D4RL](https://github.com/Farama-Foundation/D4RL)** - Offline RL benchmark covering locomotion, manipulation, and navigation tasks.
- **[Adroit](https://github.com/aravindr93/hand_dapg)** - Dexterous manipulation benchmark using a 24-DoF anthropomorphic hand for pen/door/hammer/relocate tasks.
- **[DexArt](https://www.chenbao.tech/dexart/)** - Benchmark for dexterous articulated object manipulation with 4 complex tasks using a multi-fingered hand.
- **[DexDeform](https://github.com/sizhe-li/DexDeform)** - Dexterous deformable object manipulation benchmark with 5 tasks.
- **[IsaacGym Benchmark](https://developer.nvidia.com/isaac-gym)** - GPU-accelerated dexterous manipulation benchmarks including in-hand cube reorientation and pen spinning.
- **[HumanoidBench](https://humanoid-bench.github.io/)** - A benchmark for whole-body humanoid robot control with 27 diverse tasks.
- **[DeepMind Control Suite](https://github.com/google-deepmind/dm_control)** - Continuous control tasks for locomotion and manipulation used as standard RL/VLA baselines.
- **[MyoSuite](https://sites.google.com/view/myosuite)** - Musculoskeletal simulation benchmark for physiologically accurate hand and arm control tasks.
- **[LEAP Hand](https://leaphand.com/)** - Low-cost dexterous hand platform with benchmark tasks for in-hand manipulation.

### Embodied Navigation

Benchmarks requiring agents to navigate in 3D environments guided by language or vision.

- **[R2R (Room-to-Room)](https://bringmeaspoon.org/)** - Instruction-following navigation in Matterport3D environments; foundational VLN benchmark.
- **[RxR (Room-Across-Rooms)](https://github.com/google-research-datasets/RxR)** - Multilingual navigation benchmark in 3 languages with denser language annotations than R2R.
- **[REVERIE](https://yuankaiqi.github.io/REVERIE_Challenge/)** - Remote Embodied Visual referring Expressions combining navigation and object grounding.
- **[SOON](https://scenario-oriented-object-navigation.github.io/)** - Scenario-oriented object navigation requiring reasoning about object-scene relations.
- **[EQA (Embodied Question Answering)](https://embodiedqa.org/)** - Agents navigate and answer visual questions about indoor environments.
- **[ObjectNav (Habitat)](https://aihabitat.org/)** - Navigate to an object of a specified category in novel environments.
- **[ImageNav](https://github.com/facebookresearch/image-goal-nav-dataset)** - Navigation to a goal specified by an image rather than a category label.
- **[VLN-BERT / HAMT](https://github.com/cshizhe/VLN-BERT)** - BERT-based and history-aware transformer approaches evaluated on R2R and REVERIE.
- **[VLN-CE](https://github.com/jacobkrantz/VLN-CE)** - Continuous-environment version of R2R using Habitat, without teleportation between viewpoints.
- **[CVDN](https://github.com/mmurray/cvdn)** - Cooperative Vision-and-Dialog Navigation requiring multi-turn dialogue to guide an agent.
- **[TOUCHDOWN](https://github.com/lil-lab/touchdown)** - Street-view navigation following natural language descriptions in real-world NYC environments.
- **[ScanQA](https://github.com/ATR-DBI/ScanQA)** - Spatial question answering benchmark grounded in 3D indoor point clouds.
- **[MP3D (Matterport3D)](https://niessner.github.io/Matterport/)** - Large-scale RGB-D dataset of real indoor environments widely used as a navigation substrate.
- **[MultiON](https://multinav.github.io/)** - Multi-object navigation benchmark requiring sequential finding of multiple target objects.

### Embodied Multi-Task & Household

Benchmarks combining navigation, manipulation, and reasoning in household or open-world settings.

- **[AI2-THOR](https://ai2thor.allenai.org/)** - Interactive 3D household simulation with physics for pick-and-place, slicing, cooking, and more.
- **[ALFWorld](https://alfworld.github.io/)** - Aligns text-based games (TextWorld) with AI2-THOR for generalizable language-conditioned task completion.
- **[VirtualHome](http://virtual-home.org/)** - Multi-step household activity simulation supporting natural language program execution.
- **[BEHAVIOR-1K](https://behavior.stanford.edu/)** - 1000 household activities grounded in real human needs, simulated in OmniGibson with rich annotations.
- **[Habitat 3.0](https://aihabitat.org/)** - Embodied AI simulation for social navigation, collaboration, and rearrangement tasks.
- **[ThreeDWorld (TDW)](https://www.threedworld.org/)** - Multi-modal physical simulation platform for transport, manipulation, and multi-agent tasks.
- **[TEACh](https://github.com/alexa/teach)** - Execution from Dialog History: task completion in AI2-THOR via multi-turn dialogues.
- **[LANMP](https://github.com/h2r/LANMP)** - Language-conditioned navigation and manipulation using a real mobile manipulator.
- **[ARNOLD](https://arnold-benchmark.github.io/)** - A benchmark for language-conditioned articulated object state change in 3D scenes.
- **[Watch-And-Help](https://github.com/xavierpuigf/watch_and_help)** - A social intelligence benchmark for cooperation between agents in VirtualHome.
- **[ProcTHOR](https://procthor.allenai.org/)** - Procedurally generated AI2-THOR houses for training and evaluating generalist embodied agents.

### Social & Human-Robot Interaction

Benchmarks for collaborative, communicative, and socially-aware robot behavior.

- **[Habitat 3.0 Social Nav](https://aihabitat.org/)** - Social navigation tasks requiring robots to navigate around humans and follow social norms.
- **[RoboTHOR Challenge](https://ai2thor.allenai.org/robothor/)** - ObjectNav challenge bridging simulation and real robot deployment in home-like environments.
- **[SEAN (Social Embodied Agent Navigation)](https://sean.interactive-machines.com/)** - Navigation benchmark requiring socially compliant behavior around pedestrians.
- **[TDW-Social](https://www.threedworld.org/)** - Multi-agent social simulation tasks requiring cooperation and communication in TDW.
- **[ProCo](https://github.com/ProCo-benchmark)** - Proactive cooperation benchmark for embodied agents requiring initiative and dialogue.
- **[ConcepFusion / LangNav](https://github.com/concept-fusion/concept-fusion)** - Open-vocabulary 3D feature fields enabling natural language queries for navigation.

---

## Autonomous Driving

Benchmarks for vision-language grounded driving decisions and planning.

- **[nuScenes](https://www.nuscenes.org/)** - Large-scale autonomous driving dataset with 3D bounding boxes, maps, and rich sensor data.
- **[Waymo Open Dataset](https://waymo.com/open/)** - High-quality driving dataset with LiDAR and camera data for perception and prediction.
- **[CARLA Challenge](https://leaderboard.carla.org/)** - Open urban driving simulation benchmark requiring route completion and safety compliance.
- **[DriveLM](https://github.com/OpenDriveLab/DriveLM)** - Vision-language driving benchmark with graph-structured QA over nuScenes scenes.
- **[nuPlan](https://nuplan.org/)** - Closed-loop motion planning benchmark with expert demonstrations and reactive simulation.
- **[LingoQA](https://github.com/wayveai/LingoQA)** - Video QA benchmark for driving scene understanding grounded in real-world footage.
- **[BDD-X](https://github.com/JinkyuKimUCB/explainable-deep-driving)** - Explainable driving dataset with textual descriptions and justifications for driving actions.
- **[Rank2Tell](https://github.com/LLVM-AD/rank2tell)** - Dataset for ranking and describing important objects in driving scenes.
- **[MAPLM](https://github.com/LLVM-AD/MAPLM)** - Map-based language model benchmark for understanding HD maps in autonomous driving.
- **[DriveBench](https://drive-bench.github.io/)** - Comprehensive benchmark evaluating VLMs across multiple driving perception and QA tasks.
- **[NuScenes-QA](https://github.com/qiantianwen/NuScenes-QA)** - Large-scale visual question answering benchmark built on nuScenes with 460k QA pairs.
- **[TOD3Cap](https://github.com/jxbbb/TOD3Cap)** - 3D dense captioning benchmark for autonomous driving with 2.3M descriptions.
- **[VLAAD](https://github.com/keyanzhai/VLAAD)** - Vision-Language-Action benchmark for autonomous driving with natural language instructions.
- **[DriveVLM](https://tsinghua-mars-lab.github.io/DriveVLM/)** - Evaluation framework integrating chain-of-thought VLM reasoning with motion planning.
- **[MMAD](https://github.com/MMAD-Benchmark/MMAD)** - Massive multimodal autonomous driving benchmark with 18 perception and reasoning subtasks.

---

## GUI & Computer-Use Agents

Benchmarks where a VLA agent perceives a screen (GUI) and takes keyboard/mouse actions.

- **[MiniWob++](https://miniwob.farama.org/)** - Web interaction benchmark with 100+ mini tasks (clicking, typing, form filling) in a browser.
- **[WebArena](https://webarena.dev/)** - Realistic web environment benchmark with 812 tasks across e-commerce, social, coding, and content sites.
- **[VisualWebArena](https://jykoh.com/vwa)** - Extension of WebArena with visually grounded tasks requiring image-based reasoning.
- **[Mind2Web](https://osu-nlp-group.github.io/Mind2Web/)** - Generalist web agent benchmark with 2000+ tasks from 137 real-world websites.
- **[OSWorld](https://os-world.github.io/)** - Open-ended computer task benchmark in a real OS environment (Ubuntu/Windows/macOS) with 369 tasks.
- **[WindowsAgentArena](https://microsoft.github.io/WindowsAgentArena/)** - Windows OS agent benchmark with 154 tasks spanning productivity, web, and system applications.
- **[AndroidWorld](https://google-research.github.io/android_world/)** - Android device agent benchmark with 116 programmatic tasks across 20 real Android apps.
- **[AITW (Android in the Wild)](https://github.com/google-research/google-research/tree/master/android_in_the_wild)** - Large-scale dataset of human demonstrations on Android devices across diverse tasks.
- **[ScreenSpot](https://github.com/njucckevin/SeeClick)** - GUI grounding benchmark for evaluating VLMs' ability to localize UI elements from text instructions.
- **[GUI-Odyssey](https://github.com/OpenGVLab/GUI-Odyssey)** - Cross-app navigation benchmark on Android requiring multi-step actions across multiple apps.
- **[AssistGUI](https://showlab.github.io/assistgui/)** - Desktop productivity benchmark (Word, Excel, PowerPoint) evaluated by video + screen interaction.
- **[AgentBench](https://llmbench.ai/agent)** - Comprehensive LLM-as-agent benchmark with 8 environments including OS, database, web, and games.
- **[WorkArena](https://servicenow.github.io/WorkArena/)** - Enterprise software agent benchmark with 33 tasks on a real ServiceNow instance.
- **[WebSRC](https://x-lance.github.io/WebSRC/)** - Structural reading comprehension benchmark for understanding web page layouts and content.
- **[Screen2Words](https://github.com/google-research-datasets/screen2words)** - Mobile UI screen captioning benchmark with 112k human-annotated screen summaries.
- **[SWE-bench](https://swe-bench.github.io/)** - Software engineering agent benchmark requiring VLA agents to resolve real GitHub issues.
- **[τ-bench (tau-bench)](https://github.com/sierra-research/tau-bench)** - Tool-agent-user interaction benchmark for evaluating agentic task completion with tool use.

---

## Game & Interactive Environments

Benchmarks in game or simulated worlds requiring sequential decision-making with language.

- **[NetHack Learning Environment (NLE)](https://github.com/facebookresearch/nle)** - Complex roguelike game benchmark for long-horizon decision making and language-conditioned play.
- **[MineRL / MineDojo](https://minedojo.org/)** - Minecraft-based benchmark with 3000+ diverse open-ended tasks using internet-scale knowledge.
- **[GROOT](https://github.com/GreyCampus/GROOT)** - Open-ended video game agent benchmark using Minecraft with skill learning and generalization.
- **[Atari-HEAD](https://github.com/Atari-HEAD/Atari-HEAD)** - Human eye-tracking dataset for Atari games enabling human-like visual attention evaluation.
- **[BabyAI](https://github.com/mila-iqia/babyai)** - Gridworld benchmark with procedurally generated language instructions at 19 difficulty levels.
- **[MiniGrid / MiniWorld](https://github.com/Farama-Foundation/Minigrid)** - Lightweight 2D/3D grid environments for language-conditioned navigation and reasoning.
- **[TextWorld](https://github.com/microsoft/TextWorld)** - Framework for generating and playing text-based adventure games to train language agents.
- **[ScienceWorld](https://sciworld.apps.allenai.org/)** - Interactive science experiment simulation with 30 tasks requiring procedural multi-step reasoning.
- **[CrafterBench](https://github.com/danijar/crafter)** - Open-world survival game benchmark measuring 22 achievements requiring long-horizon planning.
- **[Voyager / DEPS](https://voyager.minedojo.org/)** - LLM-powered lifelong learning Minecraft agent evaluation framework.
- **[BEHAVIOR (iGibson)](https://behavior.stanford.edu/)** - 100 household activities in iGibson simulation requiring physical commonsense reasoning.

---

## Multimodal Perception & Understanding

Benchmarks for evaluating visual, temporal, and language-grounded perception capabilities that underpin VLA models.

### General Multimodal

General-purpose benchmarks for evaluating multimodal reasoning, instruction following, and grounding.

- **[MMMU](https://mmmu-benchmark.github.io/)** - Massive Multidisciplinary Multimodal Understanding benchmark with 11.5k expert-level questions.
- **[MMBench](https://mmbench.opencompass.org.cn/)** - Systematic evaluation of VLMs across 20 capability dimensions with 3000 questions.
- **[MME](https://github.com/BradyFU/Awesome-Multimodal-Large-Language-Models/tree/Evaluation)** - Comprehensive evaluation benchmark for MLLMs with 14 subtasks covering perception and cognition.
- **[SEED-Bench](https://github.com/AILab-CVC/SEED-Bench)** - Multi-granularity evaluation for generative multimodal models with 19K questions across 12 dimensions.
- **[HallusionBench](https://github.com/tianyi-lab/HallusionBench)** - Hallucination detection benchmark for visual understanding in VLMs.
- **[POPE](https://github.com/AoiDragon/POPE)** - Polling-based object probing evaluation for object hallucination in VLMs.
- **[TouchStone](https://github.com/OFA-Sys/TouchStone)** - VLM evaluation benchmark via GPT-4 scoring across 5 ability dimensions.
- **[MMStar](https://mmstar-benchmark.github.io/)** - Elite multimodal benchmark of 1500 samples designed to minimize data leakage and require genuine VL reasoning.
- **[CV-Bench](https://github.com/cambridgeltl/cv-bench)** - Challenging vision-language benchmark focused on compositional reasoning and spatial understanding.
- **[RealWorldQA](https://x.ai/blog/grok-1.5v)** - Real-world spatial understanding benchmark from xAI testing physical world reasoning.
- **[BLINK](https://zeyofu.github.io/blink/)** - Visual perception benchmark requiring human intuitive visual abilities that challenge VLMs.
- **[WildVision](https://huggingface.co/spaces/WildVision/vision-arena)** - Real-world VLM evaluation via human preference collected from live user interactions.
- **[VLMEvalKit](https://github.com/open-compass/VLMEvalKit)** - Open-source evaluation toolkit supporting 100+ VLMs across 50+ benchmarks.
- **[MMTE](https://github.com/MMTE-benchmark/MMTE)** - Multimodal task execution benchmark evaluating models on following complex visual instructions.

### Video & Temporal Understanding

Benchmarks requiring understanding of temporal dynamics, actions, and causal reasoning in video.

- **[Something-Something v2](https://developer.qualcomm.com/software/ai-datasets/something-something)** - Temporal reasoning benchmark requiring understanding of object interactions and motion direction.
- **[Kinetics-700](https://www.deepmind.com/open-source/kinetics)** - Large-scale action recognition dataset with 700 human action classes.
- **[ActivityNet](http://activity-net.org/)** - Large-scale video benchmark for activity recognition, localization, and dense captioning.
- **[Charades](https://prior.allenai.org/projects/charades)** - Indoor activity dataset requiring temporal action localization and compositional reasoning.
- **[COIN](https://coin-dataset.github.io/)** - Comprehensive Instructional video dataset with 11,827 videos across 180 tasks and 778 steps.
- **[CrossTask](https://github.com/DmZhukov/CrossTask)** - Instructional video dataset for procedural activity understanding across 83 tasks.
- **[HowTo100M](https://www.di.ens.fr/willow/research/howto100m/)** - Large-scale narrated instructional video dataset for learning action-language grounding.
- **[STAR (Situated Reasoning)](https://bobbywu.com/STAR/)** - Situated temporal action reasoning benchmark with 4 question types grounded in real videos.
- **[NExT-QA](https://doc-doc.github.io/docs/nextqa.html)** - Video QA benchmark emphasizing causal and temporal reasoning about actions.
- **[TemporalBench](https://github.com/mu-cai/TemporalBench)** - Fine-grained temporal video understanding benchmark for VLMs with 2M QA pairs.
- **[EgoTaskQA](https://github.com/Buzz-Beater/EgoTaskQA)** - Egocentric video QA benchmark with task goal inference, procedural reasoning, and state tracking.
- **[Video-Bench](https://github.com/PKU-YuanGroup/Video-Bench)** - Comprehensive video-exclusive benchmark for evaluating video understanding in MLLMs.
- **[MVBench](https://github.com/OpenGVLab/Ask-Anything)** - Multi-task video understanding benchmark with 20 challenging temporal reasoning tasks.
- **[VideoVista](https://github.com/HITsz-TMG/VideoVista)** - Diverse video understanding benchmark spanning 14 types of tasks and 35 categories.
- **[DREAM-1K](https://github.com/TNT-Robotics/DREAM-1K)** - Benchmark for evaluating procedural video understanding needed for robot task planning.

### Egocentric & Activity

Benchmarks from a first-person perspective, closely aligned with robot/agent perception.

- **[Ego4D](https://ego4d-data.org/)** - Massive egocentric video dataset (3670h) with benchmarks for episodic memory, forecasting, and hand-object interaction.
- **[EPIC-Kitchens-100](https://epic-kitchens.github.io/)** - Egocentric kitchen activity dataset with 100 hours of unscripted cooking actions.
- **[EPIC-Kitchens Challenges](https://epic-kitchens.github.io/2024)** - Annual challenges on action recognition, detection, anticipation, and multi-instance retrieval.
- **[EGTEA Gaze+](https://cbs.ic.gatech.edu/fpv/)** - First-person cooking activity dataset with gaze and hand masks for fine-grained action recognition.
- **[Assembly101](https://assembly-101.github.io/)** - Egocentric procedural activity dataset for assembling/disassembling 101 toy vehicles.
- **[Ego-Exo4D](https://ego-exo4d-data.org/)** - Paired egocentric and exocentric (third-person) video dataset for skill assessment and correspondence.
- **[HOI4D](https://hoi4d.github.io/)** - Egocentric 4D human-object interaction dataset for category-level object manipulation.
- **[LEMMA](https://sites.google.com/view/lemma-activity)** - Multi-person, multi-task activity dataset for compositional action understanding.
- **[EgoProceL](https://github.com/Sid2697/EgoProceL)** - Egocentric procedural learning benchmark for keystep recognition from instructional videos.

### 3D Scene Understanding

Benchmarks for grounding language in 3D space, enabling perception for embodied action.

- **[ScanRefer](https://daveredrum.github.io/ScanRefer/)** - Language grounding benchmark for localizing objects in 3D point clouds using free-form descriptions.
- **[SQA3D (Situated Question Answering)](https://sqa3d.github.io/)** - Situational reasoning benchmark where agents answer questions from a situated perspective in 3D scenes.
- **[3D-VisTA](https://3d-vista.github.io/)** - Pre-trained transformer for 3D vision-language tasks covering grounding, QA, and dense captioning.
- **[EmbodiedScan](https://tai-wang.github.io/embodiedscan/)** - Holistic 3D perception benchmark for embodied agents with RGB-D input from egocentric views.
- **[MultiScan](https://3dlg-hcvc.github.io/multiscan/)** - Multi-scan indoor reconstruction dataset with articulated object annotations for VLA research.
- **[LEO](https://embodied-generalist.github.io/)** - An embodied generalist agent benchmark requiring 3D scene understanding for grounded dialogue and planning.
- **[ScanEnts3D](https://github.com/daveredrum/ScanEnts3D)** - Benchmark linking 3D scene entities to text mentions in descriptions for object grounding.
- **[CLEVR3D](https://github.com/yancie-yjr/3d-clevr)** - 3D extension of CLEVR for spatial reasoning questions grounded in 3D synthetic environments.
- **[Nu-Scenes QA](https://github.com/qiantianwen/NuScenes-QA)** - Question-answering benchmark grounded in outdoor 3D LiDAR scenes for autonomous driving reasoning.

### Language-Grounded Perception

Benchmarks for visual grounding, referring expression comprehension, and spatial reasoning.

- **[RefCOCO / RefCOCO+ / RefCOCOg](https://github.com/lichengunc/refer)** - Referring expression comprehension benchmarks requiring localizing objects from natural language.
- **[Visual Genome](https://visualgenome.org/)** - Densely annotated image dataset with region descriptions, QA, and scene graphs for grounded understanding.
- **[GQA](https://cs.stanford.edu/people/dorarad/gqa/)** - Compositional question answering benchmark requiring multi-step spatial and relational reasoning.
- **[VSR (Visual Spatial Reasoning)](https://github.com/cambridgeltl/visual-spatial-reasoning)** - True/false benchmark testing spatial relationships between objects in images.
- **[SpatialBot](https://github.com/BAAI-DCAI/SpatialBot)** - Spatial understanding benchmark evaluating depth-aware reasoning in VLMs.
- **[CLEVR](https://cs.stanford.edu/people/jcjohns/clevr/)** - Compositional language and elementary visual reasoning diagnostic benchmark.
- **[Winoground](https://huggingface.co/datasets/facebook/winoground)** - Benchmark testing visio-linguistic compositional reasoning via image-caption matching with swapped words.
- **[ARO (Attribution, Relation, Order)](https://github.com/mertyg/vision-language-models-are-bows)** - Benchmark revealing VLMs' limited sensitivity to word order and relational structure.
- **[FLUTE](https://github.com/google-research/google-research/tree/master/flute)** - Figurative language understanding for VLMs involving metaphors and similes.
- **[SeedBench-2-Plus](https://github.com/AILab-CVC/SEED-Bench)** - Extended SEED-Bench focusing on chart understanding, maps, web pages, and document comprehension.

---

## Infrastructure & Resources

Simulation engines, datasets, and evaluation platforms used to build and run VLA benchmarks.

### Simulation Environments & Platforms

Simulation engines and platforms used to construct and run VLA benchmarks.

- **[IsaacSim / IsaacLab](https://developer.nvidia.com/isaac-sim)** - NVIDIA's next-gen GPU-accelerated simulation platform for robot learning and VLA development.
- **[IsaacGym](https://developer.nvidia.com/isaac-gym)** - Legacy GPU physics simulation for massively parallel RL training on dexterous tasks.
- **[MuJoCo](https://mujoco.org/)** - Fast and accurate physics simulation engine widely used for locomotion and manipulation.
- **[Genesis](https://genesis-world.readthedocs.io/)** - Generative simulation engine with ultra-fast physics and photorealistic rendering for robot learning.
- **[SAPIEN](https://sapien.ucsd.edu/)** - Simulation platform for articulated object manipulation with PhysX physics.
- **[Robosuite](https://robosuite.ai/)** - Modular robot learning framework built on MuJoCo with standardized task suites.
- **[PyBullet / Panda-Gym](https://pybullet.org/)** - Open-source physics simulation with Panda robot gym environments for tabletop manipulation.
- **[OmniGibson](https://behavior.stanford.edu/omnigibson/)** - NVIDIA Omniverse-based simulation for BEHAVIOR-1K with realistic physics and rendering.
- **[Habitat-Sim](https://aihabitat.org/)** - High-performance 3D simulator for embodied AI with photorealistic rendering and physics.
- **[AI2-THOR (Simulator)](https://ai2thor.allenai.org/)** - Photorealistic interactive indoor simulation for embodied household task research.
- **[CoppeliaSim (V-REP)](https://www.coppeliarobotics.com/)** - Versatile robot simulation platform underlying RLBench and other benchmarks.
- **[CARLA](https://carla.org/)** - Open urban driving simulator with rich sensor modalities for autonomous driving research.
- **[SUMO](https://eclipse.dev/sumo/)** - Microscopic traffic simulation supporting multi-modal transportation research.
- **[XR-EgoBench](https://github.com/XR-EgoBench)** - Extended reality egocentric benchmark platform for AR/VR embodied agent evaluation.

### Large-Scale Datasets & Model Hubs

Key datasets and hubs that supply training and evaluation data for VLA models.

- **[HuggingFace LeRobot Datasets](https://huggingface.co/lerobot)** - Collection of standardized real-robot demonstration datasets for VLA training and benchmarking.
- **[HuggingFace Open-VLA](https://huggingface.co/openvla)** - HuggingFace hub for OpenVLA model weights, training data, and evaluation scripts.
- **[HuggingFace Robot Benchmarks](https://huggingface.co/collections/lerobot/benchmarks)** - Curated collection of robot learning benchmarks and evaluation protocols.
- **[Open X-Embodiment Dataset](https://huggingface.co/datasets/jxu124/OpenX-Embodiment)** - HuggingFace mirror of the cross-embodiment OXE dataset aggregating 1M+ robot episodes.
- **[RoboSet](https://robopen.github.io/roboset/)** - Large-scale robot manipulation dataset with 100k+ demonstrations across 12 task categories.
- **[DROID Dataset](https://huggingface.co/datasets/rail-berkeley/DROID)** - 76k robot manipulation demonstrations on HuggingFace for diverse real-world VLA training.
- **[BridgeData V2 (HF)](https://huggingface.co/datasets/rail-berkeley/bridge_dataset)** - HuggingFace version of BridgeData V2 for easy access and VLA pretraining.
- **[EgoMimic Dataset](https://egomimic.github.io/)** - Paired egocentric human video and robot demonstration dataset for VLA transfer learning.
- **[RH20T](https://rh20t.github.io/)** - Large-scale robotic dataset with 110k demonstrations across 20 tasks and temperature conditions.
- **[Ego4D HuggingFace](https://huggingface.co/datasets/lmms-lab/Ego4D)** - Ego4D benchmark data accessible via HuggingFace for convenient evaluation.

### Leaderboards & Evaluation Platforms

Platforms hosting challenges, competitions, and live leaderboards for VLA models.

- **[EvalAI](https://eval.ai/)** - Cloud-based challenge platform hosting embodied AI, VQA, navigation, and VLA competitions.
- **[PaperWithCode Embodied AI](https://paperswithcode.com/methods/category/embodied-ai)** - Live leaderboards tracking SOTA across navigation, manipulation, and QA benchmarks.
- **[HuggingFace Open VLA Leaderboard](https://huggingface.co/spaces/lerobot/eval_real_world_vla)** - Community leaderboard for real-world robot VLA performance.
- **[Open-Compass (OpenVLM Leaderboard)](https://rank.opencompass.org.cn/leaderboard-multimodal)** - Comprehensive VLM leaderboard comparing models across 50+ benchmarks.
- **[LIBERO Leaderboard](https://libero-project.github.io/main.html)** - Official leaderboard for the LIBERO manipulation benchmark suite.
- **[CARLA Autonomous Driving Leaderboard](https://leaderboard.carla.org/)** - Official competition leaderboard for autonomous driving agents in CARLA.
- **[WebArena Leaderboard](https://docs.google.com/spreadsheets/d/1M801lEpBbKSNwP-vDBkC_pF7LdyGU1f_ufZb_NWNBZQ)** - Community tracking sheet for web agent performance on WebArena.
- **[OSWorld Leaderboard](https://os-world.github.io/)** - Live leaderboard for OS computer-use agents on the OSWorld benchmark.
- **[Ego4D Challenges (EvalAI)](https://eval.ai/web/challenges/list)** - Annual Ego4D challenge tracks on episodic memory, forecasting, AV, hands, and narrations.
- **[BEHAVIOR-1K Leaderboard](https://behavior.stanford.edu/benchmark-guide.html)** - Evaluation results for household activity agents in the BEHAVIOR benchmark.
- **[AgentBench Leaderboard](https://llmbench.ai/agent/data)** - Rankings for LLM-as-agent performance across OS, web, game, and database tasks.

---

## Contributing

Contributions are welcome! To add a benchmark:
1. Fork this repository.
2. Add the entry to the appropriate section in `README.md` following the format: `**[Name](url)** - One-sentence description.`
3. Submit a pull request.

Please ensure that:
- The benchmark is relevant to VLA or embodied AI evaluation.
- You provide a link to the official website, paper, or GitHub repository.
- The description is concise (one sentence).
