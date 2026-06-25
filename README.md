# Awesome Game Agent Papers [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[![Stars](https://img.shields.io/github/stars/JayCheng113/awesome-gameagent-papers?color=yellow)](https://github.com/JayCheng113/awesome-gameagent-papers/stargazers)
[![Forks](https://img.shields.io/github/forks/JayCheng113/awesome-gameagent-papers?color=blue&label=Fork)](https://github.com/JayCheng113/awesome-gameagent-papers/network/members)
[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-green.svg)](CONTRIBUTING.md)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](LICENSE)

## Introduction

Large language models, vision-language models, and other foundation models have become
the control core of a new generation of **game agents** — agents that perceive, reason,
remember, learn skills, use tools, and cooperate or compete inside games and interactive
environments. This repository collects **must-read papers on LLM / foundation-model based
game agents**, deliberately scoped to the foundation-model lineage rather than the broader
classic RL / search / game-AI tradition.

Papers are organized in a **hybrid taxonomy**: cross-domain landmark work sits under
*Core Capabilities* (perception, planning, memory, skill learning, tool use), while the
bulk of the literature is grouped **by environment / domain** (Minecraft & open-world,
social simulation, NPC dialogue & commercial agents, general computer control,
benchmarks & environments). Game environments, mechanisms, and **method paradigms**
(`#agentic`, `#vla`, `#post-training`, `#world-model`) are carried as inline `#tags`,
so a paper may be cross-listed across sections and read along an orthogonal
paradigm lens. This is an actively-maintained, community-driven list — contributions
are welcome via [pull request](CONTRIBUTING.md).
For mistakes or suggestions, please open an issue.

## Contents

<table>
<tr><td colspan="2"><a href="#1-surveys">1. Surveys</a></td></tr>
<tr><td colspan="2"><a href="#2-core-capabilities">2. Core Capabilities</a></td></tr>
<tr>
    <td>&ensp;<a href="#21-perception--world-modeling">2.1 Perception &amp; World Modeling</a></td>
    <td>&ensp;<a href="#22-planning--reasoning">2.2 Planning &amp; Reasoning</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#23-memory">2.3 Memory</a></td>
    <td>&ensp;<a href="#24-skill-learning--curriculum">2.4 Skill Learning &amp; Curriculum</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#25-tool-use--code-as-action">2.5 Tool Use &amp; Code-as-Action</a></td>
    <td></td>
</tr>
<tr><td colspan="2"><a href="#3-minecraft--open-world-embodied-agents">3. Minecraft &amp; Open-World Embodied Agents</a></td></tr>
<tr>
    <td>&ensp;<a href="#31-foundation-policies--vla">3.1 Foundation Policies &amp; VLA</a></td>
    <td>&ensp;<a href="#32-planning--reasoning">3.2 Planning &amp; Reasoning</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#33-memory--self-evolution">3.3 Memory &amp; Self-Evolution</a></td>
    <td>&ensp;<a href="#34-multi-agent--collaboration">3.4 Multi-Agent &amp; Collaboration</a></td>
</tr>
<tr>
    <td>&ensp;<a href="#35-tooling--benchmarks">3.5 Tooling &amp; Benchmarks</a></td>
    <td></td>
</tr>
<tr><td colspan="2"><a href="#4-multi-agent-social-simulation--communication-games">4. Multi-Agent, Social Simulation &amp; Communication Games</a></td></tr>
<tr>
    <td>&ensp;<a href="#41-agent-societies--social-simulation">4.1 Agent Societies &amp; Social Simulation</a></td>
    <td>&ensp;<a href="#42-communication--strategic-games">4.2 Communication &amp; Strategic Games</a></td>
</tr>
<tr><td colspan="2"><a href="#5-npc-dialogue--commercial-agents">5. NPC Dialogue &amp; Commercial Agents</a></td></tr>
<tr><td colspan="2"><a href="#6-general-computer--3d-world-control">6. General Computer &amp; 3D-World Control</a></td></tr>
<tr><td colspan="2"><a href="#7-benchmarks--environments">7. Benchmarks &amp; Environments</a></td></tr>
<tr>
    <td>&ensp;<a href="#71-interactive-environments--benchmarks">7.1 Interactive Environments &amp; Benchmarks</a></td>
    <td>&ensp;<a href="#72-classic-pre-llm-milestones">7.2 Classic Pre-LLM Milestones</a></td>
</tr>
<tr><td colspan="2"><a href="#contributing">Contributing</a> &ensp;|&ensp; <a href="#license">License</a></td></tr>
</table>

## Latest Update

- 2026/06/25: Major expansion — ~110 vetted papers across 7 sections, with method-paradigm tags (`#agentic` / `#vla` / `#post-training` / `#world-model`); added Minecraft, social-simulation, NPC/commercial, and environment sections 🔥
- 2026/06/25: Initial release — skeleton + ~18 vetted seed papers across 8 capability topics

## 1. Surveys

- [2024/03] **A Survey on Game Playing Agents and Large Models: Methods, Applications, and Challenges** *arXiv* [[paper](https://arxiv.org/abs/2403.10249)] `#survey`
- [2024/04] **A Survey on Large Language Model-Based Game Agents** *ACM CSUR* [[paper](https://arxiv.org/abs/2404.02039)] `#survey`
- [2026/05] **Towards Generalist Game Players: An Investigation of Foundation Models in the Game Multiverse** *arXiv* [[paper](https://arxiv.org/abs/2605.09965)] `#survey`

## 2. Core Capabilities

### 2.1 Perception & World Modeling

- [2024/02] **Genie: Generative Interactive Environments** *ICML 2024* [[paper](https://arxiv.org/abs/2402.15391)] `#world-model` `#generation`
- [2024/03] **Scaling Instructable Agents Across Many Simulated Worlds (SIMA)** *arXiv* [[paper](https://arxiv.org/abs/2404.10179)] `#3d-worlds` `#vlm` `#vla`
- [2025/09] **Training Agents Inside of Scalable World Models (Dreamer 4)** *arXiv* [[paper](https://arxiv.org/abs/2509.24527)] `#world-model` `#foundation-policy` `#3d-worlds`

### 2.2 Planning & Reasoning

- [2022/10] **ReAct: Synergizing Reasoning and Acting in Language Models** *ICLR 2023* [[paper](https://arxiv.org/abs/2210.03629)][[code](https://github.com/ysymyth/ReAct)] `#planning` `#text-game` `#agentic`
- [2023/05] **SwiftSage: A Generative Agent with Fast and Slow Thinking for Complex Interactive Tasks** *NeurIPS 2023* [[paper](https://arxiv.org/abs/2305.17390)] `#text-game` `#planning` `#agentic` `#post-training`

### 2.3 Memory

- [2023/04] **Generative Agents: Interactive Simulacra of Human Behavior** *UIST 2023* [[paper](https://arxiv.org/abs/2304.03442)] `#memory` `#social-sim` `#agentic`

### 2.4 Skill Learning & Curriculum

- [2023/05] **Voyager: An Open-Ended Embodied Agent with Large Language Models** *TMLR 2024* [[paper](https://arxiv.org/abs/2305.16291)][[code](https://github.com/MineDojo/Voyager)][[project](https://voyager.minedojo.org/)] `#minecraft` `#skill-learning` `#tool-use` `#agentic`
- [2026/05] **Ratchet: A Minimal Hygiene Recipe for Self-Evolving LLM Agents** *arXiv* [[paper](https://arxiv.org/abs/2605.22148)] `#self-evolving` `#skill-learning` `#agentic`

### 2.5 Tool Use & Code-as-Action

- [2023/05] **Voyager: An Open-Ended Embodied Agent with Large Language Models** *TMLR 2024* [[paper](https://arxiv.org/abs/2305.16291)][[code](https://github.com/MineDojo/Voyager)][[project](https://voyager.minedojo.org/)] `#minecraft` `#code-as-action` `#agentic`
- [2024/02] **Executable Code Actions Elicit Better LLM Agents (CodeAct)** *ICML 2024* [[paper](https://arxiv.org/abs/2402.01030)][[code](https://github.com/xingyaoww/code-act)] `#code-as-action` `#tool-use` `#agentic` `#post-training`

## 3. Minecraft & Open-World Embodied Agents

### 3.1 Foundation Policies & VLA

- [2022/06] **Video PreTraining (VPT): Learning to Act by Watching Unlabeled Online Videos** *NeurIPS 2022* [[paper](https://arxiv.org/abs/2206.11795)] `#minecraft` `#foundation-policy` `#vla`
- [2023/06] **STEVE-1: A Generative Model for Text-to-Behavior in Minecraft** *NeurIPS 2023* [[paper](https://arxiv.org/abs/2306.00937)][[code](https://github.com/Shalev-Lifshitz/STEVE-1)][[project](https://sites.google.com/view/steve-1)] `#minecraft` `#foundation-policy` `#vla`
- [2023/10] **GROOT: Learning to Follow Instructions by Watching Gameplay Videos** *arXiv* [[paper](https://arxiv.org/abs/2310.08235)][[code](https://github.com/CraftJarvis/GROOT)][[project](https://craftjarvis.github.io/GROOT/)] `#minecraft` `#foundation-policy` `#vla`
- [2024/03] **MineDreamer: Learning to Follow Instructions via Chain-of-Imagination for Simulated-World Control** *arXiv* [[paper](https://arxiv.org/abs/2403.12037)][[code](https://github.com/Zhoues/MineDreamer)] `#minecraft` `#world-model`
- [2024/06] **OmniJARVIS: Unified Vision-Language-Action Tokenization Enables Open-World Instruction Following Agents** *NeurIPS 2024* [[paper](https://arxiv.org/abs/2407.00114)] `#minecraft` `#vla` `#post-training`
- [2024/10] **ROCKET-1: Mastering Open-World Interaction with Visual-Temporal Context Prompting** *arXiv* [[paper](https://arxiv.org/abs/2410.17856)][[project](https://craftjarvis.github.io/ROCKET-1)] `#minecraft` `#vla`
- [2024/12] **GROOT-2: Weakly Supervised Multi-Modal Instruction Following Agents** *arXiv* [[paper](https://arxiv.org/abs/2412.10410)] `#minecraft` `#vla`
- [2025/02] **Optimus-2: Multimodal Minecraft Agent with Goal-Observation-Action Conditioned Policy** *CVPR 2025* [[paper](https://arxiv.org/abs/2502.19902)][[project](https://cybertronagent.github.io/Optimus-2.github.io/)] `#minecraft` `#vla`
- [2025/03] **JARVIS-VLA: Post-Training Large-Scale Vision Language Models to Play Visual Games with Keyboards and Mouse** *ACL 2025* [[paper](https://arxiv.org/abs/2503.16365)][[code](https://github.com/CraftJarvis/JarvisVLA)][[project](https://craftjarvis.github.io/JarvisVLA/)] `#minecraft` `#vla` `#post-training`
- [2025/03] **ROCKET-2: Steering Visuomotor Policy via Cross-View Goal Alignment** *arXiv* [[paper](https://arxiv.org/abs/2503.02505)] `#minecraft` `#foundation-policy` `#vla`
- [2025/03] **Open-World Skill Discovery from Unsegmented Demonstrations** *arXiv* [[paper](https://arxiv.org/abs/2503.10684)] `#minecraft` `#skill-learning` `#vla`
- [2025/06] **Optimus-3: Dual-Router Aligned Mixture-of-Experts Agent with Dual-Granularity Reasoning-Aware Policy Optimization** *arXiv* [[paper](https://arxiv.org/abs/2506.10357)] `#minecraft` `#vla` `#post-training`
- [2025/09] **OpenHA: A Series of Open-Source Hierarchical Agentic Models in Minecraft** *arXiv* [[paper](https://arxiv.org/abs/2509.13347)] `#minecraft` `#foundation-policy` `#vla`
- [2026/02] **MAIN-VLA: Modeling Abstraction of Intention and eNvironment for Vision-Language-Action Models** *arXiv* [[paper](https://arxiv.org/abs/2602.02212)] `#minecraft` `#vla`

### 3.2 Planning & Reasoning

- [2023/02] **Describe, Explain, Plan and Select: Interactive Planning with Large Language Models Enables Open-World Multi-Task Agents (DEPS)** *NeurIPS 2023* [[paper](https://arxiv.org/abs/2302.01560)] `#minecraft` `#planning` `#agentic`
- [2023/03] **Skill Reinforcement Learning and Planning for Open-World Long-Horizon Tasks (Plan4MC)** *arXiv* [[paper](https://arxiv.org/abs/2303.16563)][[project](https://sites.google.com/view/plan4mc)] `#minecraft` `#planning` `#skill-learning`
- [2023/05] **Ghost in the Minecraft: Generally Capable Agents for Open-World Environments via Large Language Models with Text-based Knowledge and Memory (GITM)** *arXiv* [[paper](https://arxiv.org/abs/2305.17144)] `#minecraft` `#planning` `#memory` `#agentic`
- [2023/05] **Voyager: An Open-Ended Embodied Agent with Large Language Models** *TMLR 2024* [[paper](https://arxiv.org/abs/2305.16291)][[code](https://github.com/MineDojo/Voyager)][[project](https://voyager.minedojo.org/)] `#minecraft` `#planning` `#skill-learning` `#agentic`
- [2023/11] **JARVIS-1: Open-World Multi-task Agents with Memory-Augmented Multimodal Language Models** *IEEE TPAMI 2025* [[paper](https://arxiv.org/abs/2311.05997)][[code](https://github.com/CraftJarvis/JARVIS-1)] `#minecraft` `#planning` `#memory` `#agentic`
- [2023/12] **MP5: A Multi-modal Open-ended Embodied System in Minecraft via Active Perception** *CVPR 2024* [[paper](https://arxiv.org/abs/2312.07472)] `#minecraft` `#planning` `#vlm` `#agentic`
- [2024/05] **Luban: Building Open-Ended Creative Agents via Autonomous Embodied Verification** *arXiv* [[paper](https://arxiv.org/abs/2405.15414)] `#minecraft` `#skill-learning` `#agentic`
- [2024/11] **APT: Architectural Planning and Text-to-Blueprint Construction Using Large Language Models for Open-World Agents** *arXiv* [[paper](https://arxiv.org/abs/2411.17255)] `#minecraft` `#planning` `#agentic`
- [2025/05] **Experience-based Knowledge Correction for Robust Planning in Minecraft (XENON)** *ICLR 2026* [[paper](https://arxiv.org/abs/2505.24157)][[project](https://sjlee-me.github.io/XENON)] `#minecraft` `#planning` `#agentic`
- [2025/05] **BAR: A Backward Reasoning based Agent for Complex Minecraft Tasks** *arXiv* [[paper](https://arxiv.org/abs/2505.14079)] `#minecraft` `#planning` `#agentic`
- [2025/08] **VistaWise: Building Cost-Effective Agent with Cross-Modal Knowledge Graph for Minecraft** *arXiv* [[paper](https://arxiv.org/abs/2508.18722)] `#minecraft` `#planning` `#vlm` `#agentic`
- [2025/12] **Training One Model to Master Cross-Level Agentic Actions via Reinforcement Learning** *arXiv* [[paper](https://arxiv.org/abs/2512.09706)] `#minecraft` `#post-training` `#planning`
- [2026/05] **GROW: Aligning GRPO with State-Action Modeling for Open-World VLM Agents** *arXiv* [[paper](https://arxiv.org/abs/2605.20246)] `#minecraft` `#planning` `#vlm` `#post-training`
- [2026/06] **WISE: A Long-Horizon Agent in Minecraft with Why-Which Reasoning** *arXiv* [[paper](https://arxiv.org/abs/2606.12852)] `#minecraft` `#planning` `#agentic`

### 3.3 Memory & Self-Evolution

- [2024/07] **Odyssey: Empowering Minecraft Agents with Open-World Skills** *arXiv* [[paper](https://arxiv.org/abs/2407.15325)] `#minecraft` `#skill-learning` `#agentic` `#post-training`
- [2024/08] **Optimus-1: Hybrid Multimodal Memory Empowered Agents Excel in Long-Horizon Tasks** *NeurIPS 2024* [[paper](https://arxiv.org/abs/2408.03615)] `#minecraft` `#memory` `#agentic`
- [2024/11] **MrSteve: Instruction-Following Agents in Minecraft with What-Where-When Memory** *ICLR 2025* [[paper](https://arxiv.org/abs/2411.06736)][[code](https://github.com/frechele/MrSteve)][[project](https://sites.google.com/view/mr-steve)] `#minecraft` `#memory` `#agentic`
- [2025/02] **EvolvingAgent: Curriculum Self-evolving Agent with Continual World Model for Long-Horizon Tasks** *arXiv* [[paper](https://arxiv.org/abs/2502.05907)] `#minecraft` `#self-evolving` `#world-model` `#agentic`
- [2025/05] **From Entity-Centric to Goal-Oriented Graphs: Enhancing LLM Knowledge Retrieval in Minecraft** *arXiv* [[paper](https://arxiv.org/abs/2505.18607)] `#minecraft` `#memory` `#planning` `#agentic`
- [2026/03] **MineEvolve: Self-Evolution with Accumulated Knowledge for Long-Horizon Embodied Minecraft Agents** *arXiv* [[paper](https://arxiv.org/abs/2603.13131)] `#minecraft` `#self-evolving` `#skill-learning` `#agentic`
- [2026/04] **Experience Transfer for Multimodal LLM Agents in Minecraft Game (Echo)** *arXiv* [[paper](https://arxiv.org/abs/2604.05533)] `#minecraft` `#memory` `#agentic`
- [2026/05] **PEAM: Parametric Embodied Agent Memory through Contrastive Internalization of Experience in Minecraft** *arXiv* [[paper](https://arxiv.org/abs/2605.27762)] `#minecraft` `#memory` `#agentic` `#post-training`

### 3.4 Multi-Agent & Collaboration

- [2024/06] **VillagerAgent: A Graph-Based Multi-Agent Framework for Coordinating Complex Task Dependencies in Minecraft** *arXiv* [[paper](https://arxiv.org/abs/2406.05720)] `#minecraft` `#multi-agent` `#agentic`
- [2024/11] **MindForge: Empowering Embodied Agents with Theory of Mind for Lifelong Cultural Learning** *NeurIPS 2025* [[paper](https://arxiv.org/abs/2411.12977)] `#minecraft` `#multi-agent` `#agentic`
- [2024/12] **TeamCraft: A Benchmark for Multi-Modal Multi-Agent Systems in Minecraft** *arXiv* [[paper](https://arxiv.org/abs/2412.05255)][[code](https://github.com/teamcraft-bench/teamcraft)] `#minecraft` `#multi-agent` `#benchmark`
- [2025/03] **Parallelized Planning-Acting for Efficient LLM-based Multi-Agent Systems in Minecraft** *arXiv* [[paper](https://arxiv.org/abs/2503.03505)] `#minecraft` `#multi-agent` `#agentic`
- [2025/08] **CausalMACE: Causality Empowered Multi-Agents in Minecraft Cooperative Tasks** *arXiv* [[paper](https://arxiv.org/abs/2508.18797)] `#minecraft` `#multi-agent` `#planning` `#agentic`
- [2025/09] **PillagerBench: Benchmarking LLM-Based Agents in Competitive Minecraft Team Environments** *arXiv* [[paper](https://arxiv.org/abs/2509.06235)] `#minecraft` `#multi-agent` `#benchmark`
- [2026/02] **Requesting Expert Reasoning: Augmenting LLM Agents with Learned Collaborative Intervention (AHCE)** *arXiv* [[paper](https://arxiv.org/abs/2602.22546)] `#minecraft` `#multi-agent` `#agentic`
- [2026/04] **Gated Coordination for Efficient Multi-Agent Collaboration in Minecraft Game** *arXiv* [[paper](https://arxiv.org/abs/2604.18975)] `#minecraft` `#multi-agent` `#agentic`
- [2026/06] **Multi-agent Framework for Time-Sensitive Complementary Collaboration in Minecraft** *arXiv* [[paper](https://arxiv.org/abs/2606.15684)] `#minecraft` `#multi-agent` `#benchmark`

### 3.5 Tooling & Benchmarks

- [2016/07] **The Malmo Platform for Artificial Intelligence Experimentation** *IJCAI 2016* [[paper](https://www.ijcai.org/Proceedings/16/Papers/643.pdf)][[code](https://github.com/microsoft/malmo)] `#minecraft` `#benchmark`
- [2019/07] **MineRL: A Large-Scale Dataset of Minecraft Demonstrations** *IJCAI 2019* [[paper](https://arxiv.org/abs/1907.13440)] `#minecraft` `#benchmark`
- [2022/06] **MineDojo: Building Open-Ended Embodied Agents with Internet-Scale Knowledge** *NeurIPS 2022* [[paper](https://arxiv.org/abs/2206.08853)][[code](https://github.com/MineDojo/MineDojo)][[project](https://minedojo.org/)] `#minecraft` `#benchmark`
- [2023/10] **MCU: An Evaluation Framework for Open-Ended Game Agents** *arXiv* [[paper](https://arxiv.org/abs/2310.08367)] `#minecraft` `#benchmark`
- [2024/12] **MineStudio: A Streamlined Package for Minecraft AI Agent Development** *arXiv* [[paper](https://arxiv.org/abs/2412.18293)][[code](https://github.com/CraftJarvis/MineStudio)] `#minecraft` `#benchmark`
- [2024/12] **Plancraft: an evaluation dataset for planning with LLM agents** *arXiv* [[paper](https://arxiv.org/abs/2412.21033)] `#minecraft` `#benchmark` `#planning`
- [2025/05] **MineAnyBuild: Benchmarking Spatial Planning for Open-world AI Agents** *arXiv* [[paper](https://arxiv.org/abs/2505.20148)] `#minecraft` `#benchmark` `#planning`
- [2026/01] **MineNPC-Task: Task Suite for Memory-Aware Minecraft Agents** *arXiv* [[paper](https://arxiv.org/abs/2601.05215)] `#minecraft` `#benchmark` `#memory`
- [2026/04] **Can Current Agents Close the Discovery-to-Application Gap? A Case Study in Minecraft (SciCrafter)** *arXiv* [[paper](https://arxiv.org/abs/2604.24697)] `#minecraft` `#benchmark`
- [2026/05] **MineExplorer: Evaluating Open-World Exploration of MLLM Agents in Minecraft** *arXiv* [[paper](https://arxiv.org/abs/2605.30931)] `#minecraft` `#benchmark`

## 4. Multi-Agent, Social Simulation & Communication Games

### 4.1 Agent Societies & Social Simulation

- [2023/04] **Generative Agents: Interactive Simulacra of Human Behavior** *UIST 2023* [[paper](https://arxiv.org/abs/2304.03442)] `#social-sim` `#multi-agent` `#memory` `#agentic`
- [2023/08] **AI Town: A Deployable Starter Kit for Building AI Agent Societies** *GitHub* [[code](https://github.com/a16z-infra/ai-town)] `#social-sim` `#multi-agent` `#agentic`
- [2023/12] **Generative agent-based modeling with actions grounded in physical, social, or digital space using Concordia** *arXiv* [[paper](https://arxiv.org/abs/2312.03664)] `#social-sim` `#multi-agent` `#agentic`
- [2024/10] **Project Sid: Many-agent simulations toward AI civilization** *arXiv* [[paper](https://arxiv.org/abs/2411.00114)] `#minecraft` `#social-sim` `#multi-agent` `#agentic`
- [2026/02] **AIvilization v0: Toward Large-Scale Artificial Social Simulation with a Unified Agent Architecture and Adaptive Agent Profiles** *arXiv* [[paper](https://arxiv.org/abs/2602.10429)] `#social-sim` `#multi-agent` `#agentic`
- [2026/06] **Agentopia: Long-Term Life Simulation and Learning in Agent Societies** *arXiv* [[paper](https://arxiv.org/abs/2606.07513)] `#social-sim` `#multi-agent` `#agentic` `#post-training`
- [2026/06] **Emergence World: A Platform for Evaluating Long-Horizon Multi-Agent Autonomy** *arXiv* [[paper](https://arxiv.org/abs/2606.08367)] `#social-sim` `#multi-agent` `#benchmark`

### 4.2 Communication & Strategic Games

- [2022/11] **Human-level play in the game of Diplomacy by combining language models with strategic reasoning (CICERO)** *Science* [[paper](https://www.science.org/doi/10.1126/science.ade9097)] `#diplomacy` `#multi-agent` `#post-training`
- [2023/09] **Exploring Large Language Models for Communication Games: An Empirical Study on Werewolf** *arXiv* [[paper](https://arxiv.org/abs/2309.04658)] `#social-deduction` `#multi-agent` `#agentic`
- [2024/07] **Werewolf Arena: A Case Study in LLM Evaluation via Social Deduction** *arXiv* [[paper](https://arxiv.org/abs/2407.13943)] `#werewolf` `#social-deduction` `#benchmark`
- [2025/04] **Among Us: A Sandbox for Measuring and Detecting Agentic Deception** *arXiv* [[paper](https://arxiv.org/abs/2504.04072)] `#social-deduction` `#multi-agent` `#benchmark`
- [2025/04] **MultiMind: Enhancing Werewolf Agents with Multimodal Reasoning and Theory of Mind** *arXiv* [[paper](https://arxiv.org/abs/2504.18039)] `#werewolf` `#social-deduction` `#vlm` `#agentic`
- [2025/09] **Can Large Language Models Master Complex Card Games?** *arXiv* [[paper](https://arxiv.org/abs/2509.01328)] `#card-game` `#strategy` `#post-training`
- [2025/10] **Beyond Survival: Evaluating LLMs in Social Deduction Games with Human-Aligned Strategies** *arXiv* [[paper](https://arxiv.org/abs/2510.11389)] `#social-deduction` `#werewolf` `#benchmark`
- [2026/02] **One Model, All Roles: Multi-Turn, Multi-Agent Self-Play Reinforcement Learning for Conversational Social Intelligence** *arXiv* [[paper](https://arxiv.org/abs/2602.03109)] `#social-deduction` `#werewolf` `#multi-agent` `#post-training`
- [2026/03] **Deception and Communication in Autonomous Multi-Agent Systems: An Experimental Study with Among Us** *arXiv* [[paper](https://arxiv.org/abs/2603.26635)] `#social-deduction` `#multi-agent` `#benchmark`
- [2026/05] **Cattle Trade: A Multi-Agent Benchmark for LLM Bluffing, Bidding, and Bargaining** *arXiv* [[paper](https://arxiv.org/abs/2605.14537)] `#card-game` `#multi-agent` `#benchmark`
- [2026/05] **QUACK: Questioning, Understanding, and Auditing Communicated Knowledge in Multimodal Social Deduction Agents** *arXiv* [[paper](https://arxiv.org/abs/2605.27068)] `#social-deduction` `#multi-agent` `#vlm` `#benchmark`
- [2026/06] **Poker Arena: Multi-Axis Profiling of Strategic Reasoning and Memory in LLMs** *arXiv* [[paper](https://arxiv.org/abs/2606.13815)] `#card-game` `#strategy` `#benchmark`

## 5. NPC Dialogue & Commercial Agents

- [2024/02] **Driving Generative Agents With Their Personality** *arXiv* [[paper](https://arxiv.org/abs/2402.14879)] `#npc` `#persona` `#agentic`
- [2024/03] **Ubisoft NEO NPC: Generative-AI-Powered Non-Player Characters** *Ubisoft (GDC 2024)* [[blog](https://news.ubisoft.com/en-us/article/5qXdxhshJBXoanFZApdG3L/how-ubisofts-new-generative-ai-prototype-changes-the-narrative-for-npcs)] `#npc` `#commercial` `#agentic`
- [2025/01] **NVIDIA ACE: Autonomous AI Companions (PUBG Ally)** *NVIDIA (CES 2025)* [[blog](https://www.nvidia.com/en-us/geforce/news/nvidia-ace-autonomous-ai-companions-pubg-naraka-bladepoint/)] `#npc` `#commercial` `#agentic`
- [2025/07] **An Empirical Evaluation of AI-Powered Non-Player Characters' Perceived Realism and Performance in Virtual Reality Environments** *arXiv* [[paper](https://arxiv.org/abs/2507.10469)] `#npc` `#evaluation`
- [2025/08] **FAIRGAMER: Evaluating Social Biases in LLM-Based Video Game NPCs** *arXiv* [[paper](https://arxiv.org/abs/2508.17825)] `#npc` `#benchmark`
- [2025/10] **Symbolically Scaffolded Play: Designing Role-Sensitive Prompts for Generative NPC Dialogue** *arXiv* [[paper](https://arxiv.org/abs/2510.25820)] `#npc` `#persona` `#agentic`
- [2025/12] **Vox Deorum: A Hybrid LLM Architecture for 4X / Grand Strategy Game AI — Lessons from Civilization V** *arXiv* [[paper](https://arxiv.org/abs/2512.18564)][[code](https://github.com/vox-deorum/vox-deorum)][[project](https://civitas-john.github.io/publication/2025-vox-deorum)] `#strategy` `#npc` `#agentic`
- **Convai: Conversational AI Platform for Game Characters** *Product* [[site](https://convai.com/)] `#npc` `#commercial` `#agentic`
- **Inworld AI: Real-Time AI Engine for Game Characters** *Product* [[site](https://inworld.ai/)] `#npc` `#commercial` `#agentic`

## 6. General Computer & 3D-World Control

- [2024/03] **Scaling Instructable Agents Across Many Simulated Worlds (SIMA)** *arXiv* [[paper](https://arxiv.org/abs/2404.10179)] `#3d-worlds` `#vlm` `#vla`
- [2024/03] **Cradle: Empowering Foundation Agents Towards General Computer Control** *arXiv* [[paper](https://arxiv.org/abs/2403.03186)][[code](https://github.com/BAAI-Agents/Cradle)] `#gui-control` `#tool-use` `#agentic`
- [2025/03] **CombatVLA: An Efficient Vision-Language-Action Model for Combat Tasks in 3D Action Role-Playing Games** *arXiv* [[paper](https://arxiv.org/abs/2503.09527)] `#vla` `#3d-worlds` `#post-training`
- [2025/03] **Cultivating Game Sense for Yourself: Making VLMs Gaming Experts** *arXiv* [[paper](https://arxiv.org/abs/2503.21263)] `#vlm` `#3d-worlds`
- [2025/08] **Pixels to Play: A Foundation Model for 3D Gameplay** *arXiv* [[paper](https://arxiv.org/abs/2508.14295)][[code](https://github.com/elefant-ai/open-p2p)][[project](https://elefant-ai.github.io/open-p2p/)] `#3d-worlds` `#foundation-policy` `#vla`
- [2025/10] **Game-TARS: Pretrained Foundation Models for Scalable Generalist Multimodal Game Agents** *arXiv* [[paper](https://arxiv.org/abs/2510.23691)] `#3d-worlds` `#foundation-policy` `#vla`
- [2025/10] **Learning to play: A Multimodal Agent for 3D Game-Play** *arXiv* [[paper](https://arxiv.org/abs/2510.16774)] `#3d-worlds` `#foundation-policy` `#vla`
- [2025/11] **Lumine: An Open Recipe for Building Generalist Agents in 3D Open Worlds** *arXiv* [[paper](https://arxiv.org/abs/2511.08892)] `#3d-worlds` `#foundation-policy` `#vla`
- [2025/11] **SIMA 2: A Generalist Embodied Agent for Virtual Worlds** *Google DeepMind* [[paper](https://arxiv.org/abs/2512.04797)][[blog](https://deepmind.google/blog/sima-2-an-agent-that-plays-reasons-and-learns-with-you-in-virtual-3d-worlds/)] `#3d-worlds` `#vlm` `#vla` `#post-training`
- [2025/11] **IPR-1: Interactive Physical Reasoner** *arXiv* [[paper](https://arxiv.org/abs/2511.15407)] `#3d-worlds` `#foundation-policy` `#world-model` `#vla`
- [2026/01] **NitroGen: An Open Foundation Model for Generalist Gaming Agents** *arXiv* [[paper](https://arxiv.org/abs/2601.02427)] `#3d-worlds` `#foundation-policy` `#vla`
- [2026/01] **Scaling Behavior Cloning Improves Causal Reasoning: An Open Model for Real-Time Video Game Playing** *arXiv* [[paper](https://arxiv.org/abs/2601.04575)] `#foundation-policy` `#vla`
- [2026/05] **Odysseus: Scaling VLMs to 100+ Turn Decision-Making in Games via Reinforcement Learning** *arXiv* [[paper](https://arxiv.org/abs/2605.00347)] `#vlm` `#post-training`

## 7. Benchmarks & Environments

### 7.1 Interactive Environments & Benchmarks

- [2018/06] **TextWorld: A Learning Environment for Text-based Games** *IJCAI 2018 Workshop* [[paper](https://arxiv.org/abs/1806.11532)] `#text-game` `#benchmark`
- [2020/06] **The NetHack Learning Environment** *NeurIPS 2020* [[paper](https://arxiv.org/abs/2006.13760)] `#roguelike` `#benchmark`
- [2020/10] **ALFWorld: Aligning Text and Embodied Environments for Interactive Learning** *ICLR 2021* [[paper](https://arxiv.org/abs/2010.03768)][[code](https://github.com/alfworld/alfworld)][[project](https://alfworld.github.io/)] `#text-game` `#benchmark`
- [2021/09] **Crafter: Benchmarking the Spectrum of Agent Capabilities** *ICLR 2022* [[paper](https://arxiv.org/abs/2109.06780)][[project](https://danijar.com/crafter)] `#benchmark`
- [2022/07] **WebShop: Towards Scalable Real-World Web Interaction with Grounded Language Agents** *NeurIPS 2022* [[paper](https://arxiv.org/abs/2207.01206)] `#web` `#benchmark`
- [2023/10] **SmartPlay: A Benchmark for LLMs as Intelligent Agents** *ICLR 2024* [[paper](https://arxiv.org/abs/2310.01557)][[code](https://github.com/microsoft/SmartPlay)] `#benchmark`
- [2024/02] **Craftax: A Lightning-Fast Benchmark for Open-Ended Reinforcement Learning** *ICML 2024* [[paper](https://arxiv.org/abs/2402.16801)] `#benchmark`
- [2024/02] **GTBench: Uncovering the Strategic Reasoning Limitations of LLMs via Game-Theoretic Evaluations** *arXiv* [[paper](https://arxiv.org/abs/2402.12348)] `#benchmark` `#strategy`
- [2024/11] **BALROG: Benchmarking Agentic LLM and VLM Reasoning On Games** *arXiv* [[paper](https://arxiv.org/abs/2411.13543)] `#benchmark` `#vlm` `#roguelike`
- [2025/03] **DSGBench: A Diverse Strategic Game Benchmark for Evaluating LLM-based Agents in Complex Decision-Making Environments** *arXiv* [[paper](https://arxiv.org/abs/2503.06047)] `#benchmark`
- [2025/03] **AVA: Attentive VLM Agent for Mastering StarCraft II** *arXiv* [[paper](https://arxiv.org/abs/2503.05383)] `#benchmark` `#vlm` `#starcraft` `#multi-agent`
- [2025/03] **SPIN-Bench: How Well Do LLMs Plan Strategically and Reason Socially?** *arXiv* [[paper](https://arxiv.org/abs/2503.12349)] `#benchmark` `#strategy` `#multi-agent`
- [2025/04] **TALES: Text Adventure Learning Environment Suite** *arXiv* [[paper](https://arxiv.org/abs/2504.14128)] `#text-game` `#benchmark`
- [2025/04] **V-MAGE: A Game Evaluation Framework for Assessing Vision-Centric Capabilities in Multimodal Large Language Models** *arXiv* [[paper](https://arxiv.org/abs/2504.06148)] `#benchmark` `#vlm`
- [2025/05] **lmgame-Bench: How Good are LLMs at Playing Games?** *arXiv* [[paper](https://arxiv.org/abs/2505.15146)] `#benchmark` `#vlm`
- [2025/05] **VideoGameBench: Can Vision-Language Models complete popular video games?** *arXiv* [[paper](https://arxiv.org/abs/2505.18134)] `#benchmark` `#vlm`
- [2025/06] **The Decrypto Benchmark for Multi-Agent Reasoning and Theory of Mind** *arXiv* [[paper](https://arxiv.org/abs/2506.20664)] `#benchmark` `#multi-agent`
- [2025/07] **StarDojo: Benchmarking Open-Ended Behaviors of Agentic Multimodal LLMs in Production-Living Simulations with Stardew Valley** *arXiv* [[paper](https://arxiv.org/abs/2507.07445)] `#benchmark` `#vlm`
- [2025/10] **StarBench: A Turn-Based RPG Benchmark for Agentic Multimodal Decision-Making and Information Seeking** *arXiv* [[paper](https://arxiv.org/abs/2510.18483)] `#benchmark` `#vlm`
- [2026/02] **AI Gamestore: Scalable, Open-Ended Evaluation of Machine General Intelligence with Human Games** *arXiv* [[paper](https://arxiv.org/abs/2602.17594)] `#benchmark` `#vlm`
- [2026/04] **PokeGym: A Visually-Driven Long-Horizon Benchmark for Vision-Language Models** *arXiv* [[paper](https://arxiv.org/abs/2604.08340)] `#benchmark` `#vlm`
- [2026/06] **OmniGameArena: A Unified UE5 Benchmark for VLM Game Agents with Improvement Dynamics** *arXiv* [[paper](https://arxiv.org/abs/2606.09826)] `#benchmark` `#vlm` `#3d-worlds`

### 7.2 Classic Pre-LLM Milestones

> Included for historical context. These predate the LLM-agent lineage but are frequently-cited references for game-AI agents.

- [2019/10] **Grandmaster level in StarCraft II using multi-agent reinforcement learning (AlphaStar)** *Nature* [[paper](https://doi.org/10.1038/s41586-019-1724-z)] `#starcraft` `#rl`
- [2019/12] **Dota 2 with Large Scale Deep Reinforcement Learning (OpenAI Five)** *arXiv* [[paper](https://arxiv.org/abs/1912.06680)] `#dota` `#rl`

## Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for the
entry format and scope before opening a pull request.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](LICENSE)

To the extent possible under law, the contributors have waived all copyright and
related or neighboring rights to this work. See [LICENSE](LICENSE) (CC0 1.0).
