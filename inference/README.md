# Danish Lexical Inference Datasets

The entailment datasets consist of a list of statements, where for each line is given
- Two true statements  encompassing features of hyponymy and inheritance are given
- These are followed by an additional similar statement 
- The last statement is supplemented with a label denoting whether it is *true* or *false*.
- Finally, information is given regarding the ontological types and/or relations being tested in the given set of statements

The task intended for the language model is to answer whether the third statement is true or false.

This dataset was developed as part of the Danish Reasoning Benchmark. To cite, please use following citation:

Bolette Pedersen, Nathalie Sørensen, Sussi Olsen, Sanni Nimb, and Simon Gray. 2024. 
[Towards a Danish Semantic Reasoning Benchmark - Compiled from Lexical-Semantic Resources for Assessing Selected Language Understanding Capabilities of Large Language Models](https://aclanthology.org/2024.lrec-main.1421/).
In *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)*, pages 16353–16363, Torino, Italia. ELRA and ICCL.



All data are derived from [the Danish WordNet, DanNet](https://wordnet.dk/dannet/page/frontpage). 

To cite, please use the following citation:
Pedersen et al. 2009. DanNet: the challenge of compiling a wordnet for Danish by reusing a monolingual dictionary. *Language Resources and Evaluation*, 43, 269–299. [DOI: 10.1007/s10579-009-9092-1](https://doi.org/10.1007/s10579-009-9092-1).

# Content
The datasets are composed based on the four Qualia Roles defined by J. Pustejovsky (in *The Generative Lexicon*. 1998, Cambridge, MA:  MIT Press):
- Agentive role (how a concept came about)
- Constitutive role (part-whole relation of a concept)
- Formal role (the taxonomical classification of a concept)
- Telic (the function of a concept)

Test instances are generated from a generic template constructed for each ontological type under each qualia role. 
For instance, for the telic role (function) with the ontological type Instrument, we use the template 

*Man bruger en X til at Y med*\
(you use a X for Y-ing). 

We negate a selected number of utterances and try to contrast with examples from different parts of the ontology, keeping, however, always track of the truth-value. 

# License
[CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

Credit: [Centre for Language Technology (CST), University of Copenhagen](https://cst.ku.dk/english/)

Contact: Bolette Sandford Pedersen (bspedersen @ hum.ku.dk)
