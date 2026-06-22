# awesome-strategic-ai-reasoning

Strategic reasoning in AI — game theory, counterfactual regret minimization, poker AI, multi-agent systems, and where LLMs meet all of it.

Noam Brown built Libratus and Pluribus — the AIs that beat the world's best poker players using counterfactual regret minimization (CFR). That family of ideas is now showing up in LLM reasoning research. This list maps the field: the foundational papers, the landmark systems, and the libraries you'd actually use.

> Curated by the [first-tree](https://github.com/unispark-inc/first-tree?ref=awesome-strategic-ai-reasoning) team.

### 🌳 use artifacts in [first-tree](https://first-tree.ai/?utm_source=github&utm_medium=readme&utm_campaign=awesome-strategic-ai-reasoning-site) for **free** — the most efficient way for **human & agent collaboration** :D


---

## Contents

- [Foundational papers](#foundational-papers)
- [Landmark systems](#landmark-systems)
- [Frameworks & libraries](#frameworks--libraries)
- [Environments](#environments)
- [Game theory tools](#game-theory-tools)
- [Learning resources](#learning-resources)
- [Contributing](#contributing)

---

## Foundational papers

The math that made imperfect-information games solvable at scale.

- [Safe and Nested Subgame Solving for Imperfect-Information Games](https://arxiv.org/abs/1705.02955) — Brown & Sandholm, 2017. The Libratus technique. Solves each decision point as a local subgame.
- [Deep Counterfactual Regret Minimization](https://arxiv.org/abs/1811.00164) — Brown et al., ICML 2019. CFR scaled with deep learning, no domain-specific abstraction.
- [Combining Deep Reinforcement Learning and Search for Imperfect-Information Games (ReBeL)](https://arxiv.org/abs/2007.13544) — Brown et al., NeurIPS 2020. A general framework that bridges RL and CFR-style search.
- [Mastering Chess and Shogi by Self-Play (AlphaZero)](https://arxiv.org/abs/1712.01815) — Silver et al., 2017. Self-play search for perfect-information games.
- [Mastering Atari, Go, Chess and Shogi by Planning with a Learned Model (MuZero)](https://arxiv.org/abs/1911.08265) — Schrittwieser et al., 2020. Planning without knowing the rules.
- [Human-level play in Diplomacy by combining language models with strategic reasoning](https://arxiv.org/abs/2210.05492) — Bakhtin, Brown et al., 2022. The research behind Cicero.
- [SOTOPIA: Interactive Evaluation for Social Intelligence in Language Agents](https://arxiv.org/abs/2310.11667) — 2023. A benchmark for LLM social and strategic reasoning.

## Landmark systems

The AIs that actually beat humans.

- [Libratus](https://www.science.org/doi/10.1126/science.aam6914) — first AI to beat top pros at heads-up no-limit Texas Hold'em (2017).
- [Pluribus](https://www.science.org/doi/10.1126/science.aay2400) — first AI to beat pros at 6-player poker (2019).
- [Cicero](https://github.com/facebookresearch/diplomacy_cicero) — plays Diplomacy at a human level, combining strategic reasoning with natural-language negotiation.
- [KataGo](https://github.com/lightvector/KataGo) — the strongest open-source Go engine, widely used for analysis and research.
- [AlphaStar](https://github.com/google-deepmind/alphastar) — grandmaster-level StarCraft II, a hard real-time imperfect-information game.

## Frameworks & libraries

What you'd build on.

- [OpenSpiel](https://github.com/google-deepmind/open_spiel) — a collection of environments and algorithms for research in general reinforcement learning and search in games.
- [RLCard](https://github.com/datamllab/rlcard) — reinforcement learning toolkit for card games (poker, UNO, mahjong, and more).
- [mctx](https://github.com/google-deepmind/mctx) — Monte Carlo Tree Search in JAX, including MuZero-style planning.
- [pycfr](https://github.com/tansey/pycfr) — a reference CFR implementation. Old (2013) but still a clear teaching resource.

## Environments

Where agents play.

- [PettingZoo](https://github.com/Farama-Foundation/PettingZoo) — the multi-agent counterpart to Gymnasium. The standard API for multi-agent RL.
- [pgx](https://github.com/sotetsuk/pgx) — vectorized game environments in JAX, fast enough for large-scale self-play.

## Game theory tools

The classical foundations.

- [Gambit](https://gambit-project.org) — software for computing Nash equilibria and analyzing finite games.
- [Nashpy](https://github.com/drvinceknight/Nashpy) — a small Python library for the computation of equilibria of 2-player games.

## Learning resources

Start here if the papers are dense.

- [OpenSpiel Tutorials (Colab)](https://github.com/google-deepmind/open_spiel/tree/master/open_spiel/colabs) — runnable notebooks covering CFR, best response, and more.
- [An Introduction to Counterfactual Regret Minimization (PDF)](http://modelai.gettysburg.edu/2013/cfr/cfr.pdf) — the canonical CFR tutorial. Implements a Rock-Paper-Scissors and Kuhn poker solver from scratch.

---

## Contributing

Add an entry if it's a real, maintained resource on strategic reasoning in AI — a foundational paper, a landmark system, or a library people actually use.

- Verify every link is live before submitting.
- Keep the one-line description concrete: what it is, why it matters.
- One entry per PR. No marketing language.

```markdown
- [Name](URL) — one sentence on what it is and why it belongs here.
```

---

*Maintained as part of [first-tree](https://github.com/unispark-inc/first-tree?ref=awesome-strategic-ai-reasoning) — shared context infrastructure for agent teams.*
