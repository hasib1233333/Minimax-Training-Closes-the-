Title

Worst-of-Portfolio Optimization Reduces Reconnaissance Brittleness in Learned Network-Robustness Design

Abstract

Reinforcement learning (RL) agents can discover network topologies substantially more robust to targeted attack than classical heuristics produce, and a 2026 study reported such agents spontaneously discover "multi-backbone" structures. Most methods in this line of work, learned or heuristic, are trained and evaluated against a single fixed attack strategy, typically high-degree attack (HDA). We test a worst-of-portfolio training objective that instead optimizes a network-redesign agent against whichever of a small attack set (HDA, betweenness attack, random failure) is currently most damaging, recomputed at every training step. Across three topology families (Barabási–Albert, Erdős–Rényi, Watts–Strogatz), 8 seeds per family (168 runs), and two optimizers (a graph-neural-network policy trained via actor-critic RL, and simulated annealing), portfolio optimization increased worst-of-portfolio robustness by 0.015–0.018 over HDA-only optimization (Wilcoxon signed-rank, n = 24, Holm-corrected p < 0.001) while reducing HDA-specific robustness comparably; roughly 55–59% of this reduction in an HDA-referenced degradation gap reflects that drop, not a pure gain. No significant difference was detected between the two optimizers at the tested scales and budgets. An ablation restricted to simulated annealing, one topology, and five seeds suggests betweenness attack, not portfolio size, drives most of this benefit, though this is not yet established at the main comparison's scale. The effect direction replicates on real US power-grid subgraphs and persists at double the network scale, both in small supplementary samples. Portfolio-based optimization improved worst-of-portfolio robustness relative to HDA-only optimization on the tested instances and budgets, with the same direction of effect for reinforcement learning and simulated annealing.

Keywords

network robustness, reinforcement learning, simulated annealing, critical infrastructure, graph neural networks, power grid
