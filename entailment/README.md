# The Danish Entailment Datasets

The entailment datasets consist of a list of statements, where for each line is given
- One statement that describes a verbal act or event
- A second statement that describes something that could be the result of act or event mentioned in the first statement. 
- The last statement is supplemented with a label denoting whether it is true or false.
- Finally, information is given regarding which frame (from Berkely FrameNet) was used for the act/event. 

The task intended for the language model is to answer whether the second statement is true or false. For that, it is necessary to have knowledge about what is entailed by the act or event of the first statement. 
This dataset was developed as part of the Danish Reasoning Benchmark. 

To cite, please use following citation:
Bolette Pedersen, Nathalie Sørensen, Sussi Olsen, Sanni Nimb, and Simon Gray. 2024. 
[Towards a Danish Semantic Reasoning Benchmark - Compiled from Lexical-Semantic Resources for Assessing Selected Language Understanding Capabilities of Large Language Models](https://aclanthology.org/2024.lrec-main.1421/).
In *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)*, pages 16353–16363, Torino, Italia. ELRA and ICCL.


Data is derived from the Danish FrameNet Lexicon. To cite, please use the following citation:  
Sanni Nimb. 2018. [The Danish FrameNet Lexicon: method and lexical coverage](http://lrec-conf.org/workshops/lrec2018/W5/pdf/3_W5.pdf). In *Proceedings of the Eleventh International Conference on Language Resources and Evaluation (LREC 2018)*
, Paris, France. European Language Resources Association (ELRA).

## Content

The datasets are based on the Danish FrameNet Lexicon that contains 671 different frames assigned to 5,300 Danish verbs and 6,490 deverbal nouns. The lexicon refers to the semantic event ontology of Berkeley FrameNet (Baker et al., 1998), where it is explained in detail what kind of event a frame refers to, what kind of result is achieved (if any), and which frame elements are typically evoked.

The purpose of this dataset is to assess to which degree LLMs grasp the result of a particular event, in particular of causative events. E.g. if it is stated that somebody kills somebody, it entails somebody being dead.

For a selection of frames, generic templates have been designed involving some of the verbs referring to the frames. For instance
COMMERCE_BUY: Peter X’s Y from Z. Z now has Y. True.

We also negate part of the statements though it is not always straightforward to establish the truth value of these, e.g.
TELLING: Peter did not tell Mary about the engagement. Mary does not know about the engagement. Neutral – cannot be verified. 

In the first versions of the dataset, we focused on frames that refer to causative events on more or less concrete items, where the result of the event is relatively unambiguous. Version 3 includes frames that refer to activities and accomplishments.

In a later version, we will include frames that denote events that are less straight-forward, e.g. mental or abstract frames, where the results will be more ambiguous.
There are currently 328 instances in the third version.

 

# License
[CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

Credit: [Centre for Language Technology (CST), University of Copenhagen](https://cst.ku.dk/english/)

Contact: Bolette Sandford Pedersen (bspedersen @ hum.ku.dk)


