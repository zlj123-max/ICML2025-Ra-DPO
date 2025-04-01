# ICML2025 Ra-DPO

# An overview of the additional experiment results for "Risk-aware Direct Preference Optimization under Nested Risk Measure"

## Overall:

We add several experimental results to demonstrate the advantages of our method, specifically including:

1) **Numerical example:** includes a numerical example;
2) **Q&A  evaluation example using LLMs:** presents comparative evaluation results of LLMs across different algorithms on Q&A datasets;
3) **The results of Ra_DPO_2(Nested-ERM):** presents the results using nested ERM (an alternative risk measure function).
4) **The results with different seeds:** presents the results of multiple algorithms with different seeds

## Details:

**The "Numerical example" folder.**

* Figure 1 presents a simple example that demonstrates the characters of nested risk measures.

**The "Q&A  evaluation example using LLMs" folder includes three files:  Raw Q&A datasets, Selected Q&A datasets and Evaluation results of LLMs.**

* **Raw Q&A datasets:** contains several Q&A datasets, each corresponding to a different algorithm and sampled using AlpacaEval from the experiment conducted on the Anthropic HH dataset, with Pythia-1.4B serving as the base model.
* **Selected Q&A Datasets:** contains the Q&A datasets that we have chosen to demonstrate the advantages of our algorithm.
* **Evaluation results of LLMs:** contains the evaluations of DeepSeek and GPT-4o for our algorithm and  baselines answers for a selected few questions.

**The "The results of Ra_DPO_2(Nested-ERM)" folder.**

* Figures 1-3 show the results of the experiment conducted on the Anthropic HH dataset with Pythia-1.4B serving as the base model, when Nested-ERM is used as the risk measure function.
* The README.md file provides an introduction of ERM(entropic risk measure).

**The "The results with different seeds" folder.**

* This folder includes the comparison of results under different seeds and experimental results with different seeds, which is conducted on the Anthropic HH dataset using Pythia-1.4B as base models. 

