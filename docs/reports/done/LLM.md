## papers
- **FactorMiner: A Self-Evolving Agent with Skills and Experience Memory for Financial Alpha Discovery**
    - Source: arXiv
    - Link: [arXiv:2602.14670](https://arxiv.org/abs/2602.14670)
    - Tags: LLM, alpha mining
    - Notes:   
        - FactorMiner consists of three main components:
            - Experience Memory: Stores successful patterns and forbidden regions
            - Factor Mining Skill: Encapsulates operators, IC checks, correlation checks, and admission rules
            - Factor Library: Maintains a growing library of low-correlation interpretable factors
        The paper formulates factor discovery as an orthogonal library synthesis problem:

        - Mathematical objective  
            The goal is not merely to find the highest-IC individual factor, but to build a factor library L such that:

            each factor has predictive power;
            pairwise factor correlation is controlled;
            new factors complement the existing library instead of duplicating it.

            Redundancy is measured by the time-averaged cross-sectional Spearman correlation between factor signals.

        - The training period is 2024-Q1 to 2024-Q4, and the held-out test period is 2025. The target is the next 10-minute open-to-close price change ratio. Baselines include Alpha101, Random Formula, GPLearn, AlphaForge, and AlphaAgent.