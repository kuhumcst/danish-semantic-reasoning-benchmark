# danish-semantic-reasoning-benchmark
A Danish semantic reasoning benchmark compiled from lexical semantic resources
This benchmark is the first version of a semantic reasoning benchmark for Danish compiled semi-automatically from a number of human-curated lexical-semantic resources, which function as our gold standard. The datasets constitute a benchmark for assessing selected language understanding capacities of large language models (LLMs) for Danish. 

## Beta version
Current version is a beta version and is not yet fully curated.
Compared to the first version, errors in the “lexical inference” dataset have been corrected.

This version comprises 26 datasets across 7 different tasks and include 4,200 test instances. Although still limited in size, we go beyond comparative evaluation datasets for Danish by including both negative and contrastive examples as well as low-frequent vocabulary; aspects which tend to challenge current LLMs when based substantially on language transfer. 
The datasets focus on 

 - semantic inference
 - entailment
 - similarity
 - relatedness, 
 - disambiguation of words in context. 
 - sentiment

We have used ChatGPT to assess to which degree our datasets challenge the ceiling performance of state-of-the-art LLMs, average performance being relatively high with an average accuracy of 0.6 on ChatGPT 3.5 turbo and 0.8 on ChatGPT 4.0.



## Credit and reference
Bolette Pedersen, Nathalie Sørensen, Sussi Olsen, Sanni Nimb, and Simon Gray. 2024. 
[Towards a Danish Semantic Reasoning Benchmark - Compiled from Lexical-Semantic Resources for Assessing Selected Language Understanding Capabilities of Large Language Models](https://aclanthology.org/2024.lrec-main.1421/).
In *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)*, pages 16353–16363, Torino, Italia. ELRA and ICCL.



[Centre for Language Technology, Department of Nordic Studies and Linguistics, University of Copenhagen](https://cst.ku.dk/english/)

and

[Society for Danish Language and Literature](https://dsl.dk/)

## How to access zip files

The files are archived with a password so that the texts cannot be automatically scraped for training purposes. If you are a human, use the word 'benchmark'. 

Shield: [![CC BY-ND 4.0][cc-by-nd-shield]][cc-by-nd]

This work is licensed under a
[Creative Commons Attribution-NoDerivs 4.0 International License][cc-by-nd].

[![CC BY-ND 4.0][cc-by-nd-image]][cc-by-nd]

[cc-by-nd]: https://creativecommons.org/licenses/by-nd/4.0/
[cc-by-nd-image]: https://licensebuttons.net/l/by-nd/4.0/88x31.png
[cc-by-nd-shield]: https://img.shields.io/badge/License-CC%20BY--ND%204.0-lightgrey.svg
