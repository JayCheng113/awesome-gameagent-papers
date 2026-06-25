# Contributing

Thanks for helping grow **Awesome Game Agent Papers**! This list collects must-read
papers on **LLM / foundation-model based game agents**. Please keep contributions
within that scope and follow the format below.

## Scope

In scope:

- Agents that play, reason about, or act within games and interactive environments,
  driven by **large language models, vision-language models, or foundation models**.
- Surveys, methods, and benchmarks/environments directly relevant to such agents.

Out of scope (for this list):

- Classic game AI driven purely by RL / search / planning without a foundation-model
  component (e.g., AlphaStar, MuZero), unless the paper is a direct, frequently-cited
  reference for an LLM-agent topic.

## Entry Format

Add a single-line bullet to the most relevant capability section. Fields go in this
fixed order:

```
- [YYYY/MM] **Title** *Venue* [[paper](URL)][[code](URL)][[project](URL)] `#tag` `#tag`
```

Rules:

- **Date** `[YYYY/MM]` first (use the first public/arXiv date).
- **Title** in bold; **Venue** in italics (`*NeurIPS 2023*`, `*ICLR 2024*`, or `*arXiv*`).
- **Link group**: include only links that exist. Omit `[[code]]` / `[[project]]` when
  there is none. Always include a `[[paper]]` link.
- **Tags** are inline backtick code. Reuse existing tags where possible
  (e.g. `#minecraft`, `#text-game`, `#planning`, `#memory`, `#tool-use`,
  `#code-as-action`, `#multi-agent`, `#benchmark`). A paper may carry several tags.
- A paper may be **cross-listed** under more than one section if it is a landmark for
  multiple capabilities (e.g. Voyager under both Skill Learning and Tool Use).

## Checklist Before Opening a PR

- [ ] The paper fits the scope above.
- [ ] The entry is placed in the right capability section.
- [ ] The entry follows the format exactly (one line, correct field order).
- [ ] The `[[paper]]` link resolves to the real paper.
- [ ] Tags reuse existing ones where they apply.

## Example

```
- [2024/02] **Executable Code Actions Elicit Better LLM Agents (CodeAct)** *ICML 2024* [[paper](https://arxiv.org/abs/2402.01030)][[code](https://github.com/xingyaoww/code-act)] `#code-as-action` `#tool-use`
```
