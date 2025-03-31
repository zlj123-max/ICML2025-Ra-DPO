## Nested risk measure

In this paper, we introduce the nested risk measure function $\operatorname{\Phi}(\cdot)$ with risk control parameter $\mu$.

For any random variable $Z$, we have $\operatorname{\Phi}^{\mu}(Z)=\int_0^1 F_Z^{-1}(\xi) \mathrm{d} G(\xi),$ where $G$ is a weighting function over the quantiles.

Specifically, in the experiments, we employed the popular CVaR as the risk measure function.

To demonstrate its generality, we employ Nested-ERM as the risk measure function and add the results of the experiment conducted on the Anthropic HH dataset with Pythia-1.4B serving as the base model.

## The introduction of ERM (entropic risk measure)

The entropic risk measure (ERM) [1-3] is a special type of exponential utility functions, and its expression is as follows:

$ \rho_{\text{ERM}}(G; \mu) := \frac{1}{\mu} \log \mathbb{E} \left[ e^{-\mu G} \right], $

where,  $\mu > 0.$

Specifically, denote that the quantile function of  a random variable $Z$ is $F_Z^{-1}(\xi) = \inf \{ z \in \mathbb{R} \mid F_Z(z) \geq \xi \}$ and $G(\xi) = e^{-\mu \xi}$.

Then, $\Phi^\mu(Z) $ becomes

$\Phi^\mu(Z) = \frac{1}{\beta} \log \left( \int_{0}^{1} F_Z^{-1}(\xi) dG(\xi)  \right),$

where $\lim_{\xi \to 0^+} G(\xi) = 1, \ \lim_{\xi \to 1} G(\xi) = 0.$

 Note: Optimizing ERM is equivalent to optimizing an exponential utility function (EU),

$\rho_{\text{EU}}(G; \mu) := \mathbb{E} \left[ e^{-\mu G} \right].$

**References:**

[1] Föllmer, Hans, and Alexander Schied. Convex measures of risk and trading constraints. *Finance and stochastics* 6 (2002): 429-447.

[2] Hau, Jia Lin, Marek Petrik, and Mohammad Ghavamzadeh. Entropic risk optimization in discounted MDPs. In AISTATS, 2023.

[3] Fei, Yingjie, Zhuoran Yang, Yudong Chen, Zhaoran Wang, and Qiaomin Xie. Risk-sensitive reinforcement learning: Near-optimal risk-sample tradeoff in regret. In NeuriPS, 2020.
