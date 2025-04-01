# Danish Similarity Word Intrusion Datasets

The word intrusion datasets consists of a list of words where:
- Five words belong to the core group and are semantically similar to each other (e.g., synonyms, near synonyms or other semantic overlap)
  (Note: this used to be three words in the older version. We have since expanded the dataset)
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

Three granularities:
- Fine 
- Medium
- corse

### Fine-grained similarity
In the fine-grained similarity dataset, the core group is always from the same dotgroup. The outlier belongs under the same keyword as the core group, but from a different dotgroup.

The data is a tab-separated text-file with the following columns:
candidates	label   outlier_position    id  chapter section

- candidates: list containing core group + outlier (example: ['it-udstyr', 'edb-udstyr', **'motherboard'**, 'maskinel', 'hardware', 'dataudstyr'])
- label: outlier (example: **'motherboard'**)
- label position: outlier index in list (example: **2**)
- example id: id to identify specific core group
- chapter: chapter from the Danish Thesaurus
- section: section from the Danish Thesaurus

### Medium-grained similarity
In the medium-grained similarity dataset, the core group is always from the same dotgroup as in the case of the fine-grained dataset.
The outlier is however now from a different subkeygroup, but still under the same main keyword.

The data is a tab-separated text-file with the following columns:
candidates	label   outlier_position    id  chapter section

- candidates: list containing core group + outlier (example: ['it-udstyr', 'edb-udstyr', **'gigabyte'**, 'maskinel', 'hardware', 'dataudstyr'])
- label: outlier (example: **'gigabyte'**)
- outlier position: outlier index in list (example: **2**)
- example id: id to identify specific core group
- chapter: chapter from the Danish Thesaurus
- section: section from the Danish Thesaurus

### corse-grained similarity
In the corse-grained similarity dataset, the core group is always from the same dotgroup as in the case of the fine-grained dataset.
The outlier is however now from a different keygroup, but still under the same section.

The data is a tab-separated text-file with the following columns:
candidates	label   outlier_position    id  chapter section

- candidates: list containing core group + outlier (example: ['it-udstyr', 'edb-udstyr', **'programmør'**, 'maskinel', 'hardware', 'dataudstyr'])
- label: outlier (example: **'programmør'**)
- outlier position: outlier index in list (example: **2**)
- example id: id to identify specific core group
- chapter: chapter from the Danish Thesaurus
- section: section from the Danish Thesaurus


## License
[CC BY-ND](https://creativecommons.org/licenses/by-nd/4.0/)

Credit: [Society for Danish Language and Literature](https://dsl.dk/)

Contact: Nathalie Hau Sørensen (nats @ dsl.dk)

