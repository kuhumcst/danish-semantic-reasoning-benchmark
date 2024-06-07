# Danish Similarity Word Intrusion Datasets

The word intrusion datasets consists of a list of words where:
- Three words belong to the core group and are semantically similar to each other (e.g., synonyms, near synonyms or other semantic overlap)
- One word is an outlier

The task is to identify the outlier in the list of words.

This dataset was developed as part of the Danish Reasoning Benchmark.
To cite, please use following citation:

Bolette Pedersen, Nathalie Sørensen, Sussi Olsen, Sanni Nimb, and Simon Gray. 2024. 
[Towards a Danish Semantic Reasoning Benchmark - Compiled from Lexical-Semantic Resources for Assessing Selected Language Understanding Capabilities of Large Language Models](https://aclanthology.org/2024.lrec-main.1421/).
In *Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)*, pages 16353–16363, Torino, Italia. ELRA and ICCL.

All data is based on the Danish Thesaurus. Read more here:
https://euralex.org/wp-content/themes/euralex/proceedings/Euralex%202014/euralex_2014_012_p_191.pdf

## Content

Two granularities:
- Fine 
- Medium

### Fine-grained similarity
In the fine-grained similarity dataset, the core group is always from the same dotgroup. The outlier belongs under the same keyword as the core group, but from a different dotgroup.

The data is a tab-separated text-file with the following columns:
candidates	label	core_group_placement	outlier_placement

- candidates: list containing core group + outlier (example: ['word_1', 'word_2', 'word_3', 'word_4'])
- label: outlier (example: 'word_3')
- core_group_placement: which section, keyword, and dotgroup from the Danish Thesaurus the core group words are taken from (example: chapter 1, section 2, under måne 'moon', second dotgroup = 01.002.måne.01)
- Outlier_placement: NOT RELIABLE! which keyword, subkeyword and dotgroup index the outlier is taken from. Outlier is always from same section and keyword as the core group. (example: Månen.månefase.0) 


### Medium-grained similarity
In the medium-grained similarity dataset, the core group is always from the same dotgroup as in the case of the fine-grained dataset.
The outlier is however now from a different subkeygroup, but still under the same main keyword.

The data is a tab-separated text-file with the following columns:
candidates	label	core_group_placement	outlier_placement

- candidates: list containing core group + outlier (example: ['word_1', 'word_2', 'word_3', 'word_4'])
- label: outlier (example: 'word_3')
- core_group_placement: which section, keyword, and dotgroup from the Danish Thesaurus the core group words are taken from (example: chapter 1, section 2, under måne 'moon', second dotgroup = 01.002.måne.01)
- Outlier_placement: which other subkeygroup and dotgroup index the outlier is taken from (example: main_keyword.subkeyword.dotgroup: Månen.selenologi.0)


## License
[CC BY-ND](https://creativecommons.org/licenses/by-nd/4.0/)

Credit: [Society for Danish Language and Literature](https://dsl.dk/)

Contact: Nathalie Hau Sørensen (nats @ dsl.dk)

