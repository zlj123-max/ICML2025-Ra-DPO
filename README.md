# ICML2025-Ra-DPO
# Additional experiment results of  "Risk-aware Direct Preference Optimization under Nested Risk Measure"

## Overall:

We have added three experimental results to demonstrate the advantages of our method, specifically including:

1) **Numerical example:** includes a numerical example;
2) **Q&A  evaluation:** Presents comparative evaluation results of LLMs across different algorithms on Q&A datasets.
3) **Ra_DPO_2(Nested-ERM):** Presents the results using nested ERM (an alternative risk measure function).

## Details:

**The "Numerical example" folder includes two images.**

* Figure 1 shows a flowchart of token-level human preference optimization with nested risk measures
* Figure 2 compares the computational differences among different algorithms to highlight the advantages of our method.

**The "Q&A  evaluation" folder includes three files:  Q&A datasets, Selected Q&A datasets and Evaluation results of LLMs.**

* The "Q&A datasets" folder contains several Q&A datasets, each corresponding to a different algorithm and sampled using AlpacaEval from the experiment conducted on the Anthropic HH dataset, with Pythia-1.4B serving as the base model.
* The "Selected Q&A Datasets" folder contains the Q&A datasets that we have chosen to demonstrate the advantages of our algorithm.
* The "Evaluation results of LLMs" folder contains the evaluations of DeepSeek and Qwen for our algorithm and  baselines answers for a selected few questions.

**The "Ra_DPO_2(Nested-ERM)" folder includes one image.**

* Figure 1 shows the results of the experiment conducted on the Anthropic HH dataset with Pythia-1.4B serving as the base model, when Nested-ERM is used as the risk measure function.