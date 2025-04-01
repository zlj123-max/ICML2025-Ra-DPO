
## Brief description of experimental results across different random seeds

* The "The results with different seeds" folder includes the comparison of results under different seeds and experimental results with different seeds, which is conducted on the Anthropic HH dataset using Pythia-1.4B as base models. Specifically, here includes three algorithms：
  - **baseline:** $TDPO_2$ with $\alpha= 0.5$;
  - **Ours:** $Ra-DPO_2$ (CVarR) with $\alpha= 0.5$, and risk  coefficient $\mu = 0.97$;
  - **Ours:** $Ra-DPO_2$ (ERM) with $\alpha= 0.5$, and risk  coefficient $\mu = 5$.


* The experimental results demonstrate that our $Ra-DPO_2$ algorithm consistently maintains lower KL divergence and higher reward accuracy. The only exception occurs with seed=10, where $TDPO_2$ attains comparable accuracy levels.

