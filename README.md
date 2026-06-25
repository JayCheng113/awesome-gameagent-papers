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

Papers are organized **by capability / topic** (perception, planning, memory, skill
learning, tool use, multi-agent play), plus surveys and benchmarks. Game environments are
carried as inline `#tags`, so a paper may be cross-listed across sections. This is an
actively-maintained, community-driven list — contributions are welcome via
[pull request](CONTRIBUTING.md). For mistakes or suggestions, please open an issue.

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
<tr><td colspan="2"><a href="#3-multi-agent--social-games">3. Multi-Agent &amp; Social Games</a></td></tr>
<tr><td colspan="2"><a href="#4-benchmarks--environments">4. Benchmarks &amp; Environments</a></td></tr>
<tr><td colspan="2"><a href="#contributing">Contributing</a> &ensp;|&ensp; <a href="#license">License</a></td></tr>
</table>

## Latest Update

- 2026/06/25: Initial release — skeleton + ~18 vetted seed papers across 8 capability topics 🔥

## 1. Surveys

- [2024/04] **A Survey on Large Language Model-Based Game Agents** *ACM CSUR* [[paper](https://arxiv.org/abs/2404.02039)] `#survey`

## 2. Core Capabilities

### 2.1 Perception & World Modeling

- [2024/03] **Scaling Instructable Agents Across Many Simulated Worlds (SIMA)** *arXiv* [[paper](https://arxiv.org/abs/2404.10179)] `#3d-worlds` `#vlm`
- [2024/02] **Genie: Generative Interactive Environments** *ICML 2024* [[paper](https://arxiv.org/abs/2402.15391)] `#world-model` `#generation`
- [2022/06] **MineDojo: Building Open-Ended Embodied Agents with Internet-Scale Knowledge** *NeurIPS 2022* [[paper](https://arxiv.org/abs/2206.08853)][[code](https://github.com/MineDojo/MineDojo)][[project](https://minedojo.org/)] `#minecraft` `#benchmark`

### 2.2 Planning & Reasoning

- [2022/10] **ReAct: Synergizing Reasoning and Acting in Language Models** *ICLR 2023* [[paper](https://arxiv.org/abs/2210.03629)][[code](https://github.com/ysymyth/ReAct)] `#planning` `#text-game`
- [2023/02] **Describe, Explain, Plan and Select: Interactive Planning with Large Language Models Enables Open-World Multi-Task Agents (DEPS)** *NeurIPS 2023* [[paper](https://arxiv.org/abs/2302.01560)] `#minecraft` `#planning`
- [2023/05] **SwiftSage: A Generative Agent with Fast and Slow Thinking for Complex Interactive Tasks** *NeurIPS 2023* [[paper](https://arxiv.org/abs/2305.17390)] `#text-game` `#planning`
- [2023/05] **Ghost in the Minecraft: Generally Capable Agents for Open-World Environments via Large Language Models with Text-based Knowledge and Memory (GITM)** *arXiv* [[paper](https://arxiv.org/abs/2305.17144)] `#minecraft` `#planning` `#memory`

### 2.3 Memory

- [2023/04] **Generative Agents: Interactive Simulacra of Human Behavior** *UIST 2023* [[paper](https://arxiv.org/abs/2304.03442)] `#memory` `#social-sim`
- [2023/11] **JARVIS-1: Open-World Multi-task Agents with Memory-Augmented Multimodal Language Models** *IEEE TPAMI 2025* [[paper](https://arxiv.org/abs/2311.05997)][[code](https://github.com/CraftJarvis/JARVIS-1)] `#minecraft` `#memory`
- [2024/08] **Optimus-1: Hybrid Multimodal Memory Empowered Agents Excel in Long-Horizon Tasks** *NeurIPS 2024* [[paper](https://arxiv.org/abs/2408.03615)] `#minecraft` `#memory`

### 2.4 Skill Learning & Curriculum

- [2023/05] **Voyager: An Open-Ended Embodied Agent with Large Language Models** *TMLR 2024* [[paper](https://arxiv.org/abs/2305.16291)][[code](https://github.com/MineDojo/Voyager)][[project](https://voyager.minedojo.org/)] `#minecraft` `#skill-learning` `#tool-use`
- [2023/05] **Ghost in the Minecraft: Generally Capable Agents for Open-World Environments via Large Language Models with Text-based Knowledge and Memory (GITM)** *arXiv* [[paper](https://arxiv.org/abs/2305.17144)] `#minecraft` `#skill-learning`

### 2.5 Tool Use & Code-as-Action

- [2023/05] **Voyager: An Open-Ended Embodied Agent with Large Language Models** *TMLR 2024* [[paper](https://arxiv.org/abs/2305.16291)][[code](https://github.com/MineDojo/Voyager)][[project](https://voyager.minedojo.org/)] `#minecraft` `#code-as-action`
- [2024/02] **Executable Code Actions Elicit Better LLM Agents (CodeAct)** *ICML 2024* [[paper](https://arxiv.org/abs/2402.01030)][[code](https://github.com/xingyaoww/code-act)] `#code-as-action` `#tool-use`
- [2024/03] **Cradle: Empowering Foundation Agents Towards General Computer Control** *arXiv* [[paper](https://arxiv.org/abs/2403.03186)][[code](https://github.com/BAAI-Agents/Cradle)] `#gui-control` `#tool-use`

## 3. Multi-Agent & Social Games

- [2023/09] **Exploring Large Language Models for Communication Games: An Empirical Study on Werewolf** *arXiv* [[paper](https://arxiv.org/abs/2309.04658)] `#social-deduction` `#multi-agent`
- [2022/11] **Human-level play in the game of Diplomacy by combining language models with strategic reasoning (CICERO)** *Science* [[paper](https://www.science.org/doi/10.1126/science.ade9097)] `#diplomacy` `#multi-agent`
- [2023/04] **Generative Agents: Interactive Simulacra of Human Behavior** *UIST 2023* [[paper](https://arxiv.org/abs/2304.03442)] `#social-sim` `#multi-agent`

## 4. Benchmarks & Environments

- [2020/10] **ALFWorld: Aligning Text and Embodied Environments for Interactive Learning** *ICLR 2021* [[paper](https://arxiv.org/abs/2010.03768)][[code](https://github.com/alfworld/alfworld)][[project](https://alfworld.github.io/)] `#text-game` `#benchmark`
- [2022/06] **MineDojo: Building Open-Ended Embodied Agents with Internet-Scale Knowledge** *NeurIPS 2022* [[paper](https://arxiv.org/abs/2206.08853)][[code](https://github.com/MineDojo/MineDojo)][[project](https://minedojo.org/)] `#minecraft` `#benchmark`
- [2023/10] **SmartPlay: A Benchmark for LLMs as Intelligent Agents** *ICLR 2024* [[paper](https://arxiv.org/abs/2310.01557)][[code](https://github.com/microsoft/SmartPlay)] `#benchmark`

## Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for the
entry format and scope before opening a pull request.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](LICENSE)

To the extent possible under law, the contributors have waived all copyright and
related or neighboring rights to this work. See [LICENSE](LICENSE) (CC0 1.0).
