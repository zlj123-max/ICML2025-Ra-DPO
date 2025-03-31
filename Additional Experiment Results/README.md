# Additional experiment results of  "Risk-aware Direct Preference Optimization under Nested Risk Measure"

## Overall:

We have added three experimental results to demonstrate the advantages of our method, specifically including:

1) **Numerical example:** includes a numerical example;
2) **Q&A  evaluation example using LLMs:** Presents comparative evaluation results of LLMs across different algorithms on Q&A datasets;
3) **The results of Ra_DPO_2(Nested-ERM):** Presents the results using nested ERM (an alternative risk measure function).

## Details:

**The "Numerical example" folder includes two images.**

* Figure 1 presents a simple example that  demonstrates the characters of nested risk measures.
* Figure 2 compares the computational differences among different algorithms to highlight the advantages of our method.

**The "Q&A  evaluation example using LLMs" folder includes three files:  Raw Q&A datasets, Selected Q&A datasets and Evaluation results of LLMs.**

* **Raw Q&A datasets:** contains several Q&A datasets, each corresponding to a different algorithm and sampled using AlpacaEval from the experiment conducted on the Anthropic HH dataset, with Pythia-1.4B serving as the base model.
* **Selected Q&A Datasets:** contains the Q&A datasets that we have chosen to demonstrate the advantages of our algorithm.
* **Evaluation results of LLMs:** contains the evaluations of DeepSeek and GPT-4o for our algorithm and  baselines answers for a selected few questions.

**The "The results of Ra_DPO_2(Nested-ERM)" folder includes one image.**

* Figure 1 shows the results of the experiment conducted on the Anthropic HH dataset with Pythia-1.4B serving as the base model, when Nested-ERM is used as the risk measure function.
