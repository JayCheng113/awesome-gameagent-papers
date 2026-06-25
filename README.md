# Awesome Game Agent Papers [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> 🎮 **A curated list of must-read papers on LLM / foundation-model based game agents.**

[![PRs Welcome](https://img.shields.io/badge/PRs-Welcome-green.svg)](CONTRIBUTING.md)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](LICENSE)

This list focuses on agents that play, reason about, or act within games and
interactive environments **driven by large language models, vision-language models,
and foundation models** — not the broader classic RL / search / game-AI lineage.
Papers are organized **by capability / topic**; game environments are carried as
inline `#tags`, so a paper may be cross-listed across sections.

## Contents

- [Surveys](#surveys)
- [Perception & World Modeling](#perception--world-modeling)
- [Planning & Reasoning](#planning--reasoning)
- [Memory](#memory)
- [Skill Learning & Curriculum](#skill-learning--curriculum)
- [Tool Use & Code-as-Action](#tool-use--code-as-action)
- [Multi-Agent & Social Games](#multi-agent--social-games)
- [Benchmarks & Environments](#benchmarks--environments)
- [Contributing](#contributing)
- [License](#license)

## Surveys

- [2024/04] **A Survey on Large Language Model-Based Game Agents** *ACM CSUR* [[paper](https://arxiv.org/abs/2404.02039)] `#survey`

## Perception & World Modeling

- [2024/04] **Scaling Instructable Agents Across Many Simulated Worlds (SIMA)** *arXiv* [[paper](https://arxiv.org/abs/2404.10179)] `#3d-worlds` `#vlm`
- [2024/02] **Genie: Generative Interactive Environments** *ICML 2024* [[paper](https://arxiv.org/abs/2402.15391)] `#world-model` `#generation`
- [2022/06] **MineDojo: Building Open-Ended Embodied Agents with Internet-Scale Knowledge** *NeurIPS 2022* [[paper](https://arxiv.org/abs/2206.08853)][[code](https://github.com/MineDojo/MineDojo)][[project](https://minedojo.org/)] `#minecraft` `#benchmark`

## Planning & Reasoning

- [2022/10] **ReAct: Synergizing Reasoning and Acting in Language Models** *ICLR 2023* [[paper](https://arxiv.org/abs/2210.03629)][[code](https://github.com/ysymyth/ReAct)] `#planning` `#text-game`
- [2023/02] **Describe, Explain, Plan and Select (DEPS): Interactive Planning with LLMs for Open-World Multi-Task Agents** *NeurIPS 2023* [[paper](https://arxiv.org/abs/2302.01560)] `#minecraft` `#planning`
- [2023/05] **SwiftSage: A Generative Agent with Fast and Slow Thinking for Complex Interactive Tasks** *NeurIPS 2023* [[paper](https://arxiv.org/abs/2305.17390)] `#text-game` `#planning`
- [2023/05] **Ghost in the Minecraft (GITM): Generally Capable Agents for Open-World Environments** *arXiv* [[paper](https://arxiv.org/abs/2305.17144)] `#minecraft` `#planning` `#memory`

## Memory

- [2023/04] **Generative Agents: Interactive Simulacra of Human Behavior** *UIST 2023* [[paper](https://arxiv.org/abs/2304.03442)] `#memory` `#social-sim`
- [2023/11] **JARVIS-1: Open-World Multi-task Agents with Memory-Augmented Multimodal Language Models** *arXiv* [[paper](https://arxiv.org/abs/2311.05997)][[code](https://github.com/CraftJarvis/JARVIS-1)] `#minecraft` `#memory`
- [2024/08] **Optimus-1: Hybrid Multimodal Memory Empowered Agents Excel in Long-Horizon Tasks** *NeurIPS 2024* [[paper](https://arxiv.org/abs/2408.03615)] `#minecraft` `#memory`

## Skill Learning & Curriculum

- [2023/05] **Voyager: An Open-Ended Embodied Agent with Large Language Models** *NeurIPS 2023 Workshop* [[paper](https://arxiv.org/abs/2305.16291)][[code](https://github.com/MineDojo/Voyager)][[project](https://voyager.minedojo.org/)] `#minecraft` `#skill-learning` `#tool-use`
- [2023/05] **Ghost in the Minecraft (GITM)** *arXiv* [[paper](https://arxiv.org/abs/2305.17144)] `#minecraft` `#skill-learning`

## Tool Use & Code-as-Action

- [2023/05] **Voyager** *NeurIPS 2023 Workshop* [[paper](https://arxiv.org/abs/2305.16291)][[code](https://github.com/MineDojo/Voyager)] `#minecraft` `#code-as-action`
- [2024/02] **Executable Code Actions Elicit Better LLM Agents (CodeAct)** *ICML 2024* [[paper](https://arxiv.org/abs/2402.01030)][[code](https://github.com/xingyaoww/code-act)] `#code-as-action` `#tool-use`
- [2024/03] **Cradle: Empowering Foundation Agents Towards General Computer Control** *arXiv* [[paper](https://arxiv.org/abs/2403.03186)][[code](https://github.com/BAAI-Agents/Cradle)] `#gui-control` `#tool-use`

## Multi-Agent & Social Games

- [2023/09] **Exploring Large Language Models for Communication Games: An Empirical Study on Werewolf** *arXiv* [[paper](https://arxiv.org/abs/2309.04658)] `#social-deduction` `#multi-agent`
- [2022/11] **CICERO: Human-level Play in the Game of Diplomacy by Combining Language Models with Strategic Reasoning** *Science* [[paper](https://www.science.org/doi/10.1126/science.ade9097)] `#diplomacy` `#multi-agent`
- [2023/04] **Generative Agents: Interactive Simulacra of Human Behavior** *UIST 2023* [[paper](https://arxiv.org/abs/2304.03442)] `#social-sim` `#multi-agent`

## Benchmarks & Environments

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
