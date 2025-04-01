# ICML2025 Ra-DPO (Submission Number: 14821)

# An overview of the additional experiment results for "Risk-aware Direct Preference Optimization under Nested Risk Measure"

**Note: We apologize that some images or files are too large to preview and must be downloaded. Please click the 'Download Repository' button in the upper-right corner. Thank you !**

## Overall:

We add several experimental results to demonstrate the advantages of our method, specifically including:

1) **Numerical example:** includes a numerical example;
2) **Q&A  evaluation examples using LLMs:** presents comparative evaluation results of LLMs across different algorithms on Q&A datasets;
3) **The results of Ra_DPO_2(ERM):** presents the results using nested ERM (an alternative risk measure function);
4) **The results with different seeds:** presents the results of multiple algorithms with different seeds.

## Details:

### The "Numerical example" folder

* Figure 1 presents a simple example that demonstrates the characters of nested risk measures.

### The "Q&A  evaluation examples using LLMs" folder 

* **Raw Q&A datasets:** contains several Q&A datasets, each corresponding to a different algorithm and sampled using AlpacaEval from the experiment conducted on the Anthropic HH dataset, with Pythia-1.4B serving as the base model.
* **Selected Q&A Datasets:** contains the Q&A datasets selected for evaluation.
* **Evaluation results of LLMs:** presents the comparative performance of DeepSeek and GPT-4o on our algorithm versus baseline methods, using a selected set of questions.

_**Conclusions(LLMs):**_ Some (Our) algorithms (such as HH_py1.4b_sft_ra-tdpo1_cl0.97 and HH_py1.4b_sft_ra-tdpo2_alp0.5_cl0.97) can provide high-quality practical information, while the effectiveness of other algorithms (such as HH_py1.4b_sft_ra-tdpo1_cl0.99 and HH_py1.4b_sft_ra-tdpo2_alp0.5_cl0.99) is relatively low and their redundancy is relatively high. Future research should focus on optimizing algorithms to improve their performance in terms of effectiveness and redundancy, thereby enhancing their overall performance.

### The "The results of Ra_DPO_2(ERM)" folder

* Figures 1-3 show the results of the experiment conducted on the Anthropic HH dataset with Pythia-1.4B serving as the base model, when Nested-ERM is used as the risk measure function.
* The README.md file provides an introduction of ERM(entropic risk measure).

_**Conclusions:**_ Experimental results show that our $𝑅𝑎−𝐷𝑃𝑂_2$ algorithm (with Nested-ERM) also achieves consistently lower KL divergence and higher reward accuracy compared to baseline methods.

### The "The results with different seeds" folder

* This folder includes the comparison of results under different seeds and experimental results with different seeds, which is conducted on the Anthropic HH dataset using Pythia-1.4B as base models. 

_**Conclusions:**_ The experimental results demonstrate that our $Ra-DPO_2$ algorithm consistently maintains lower KL divergence and higher reward accuracy. The only exception occurs with seed=10, where $TDPO_2$ attains comparable accuracy levels.







