# Danish Relatedness Word Intrusion Datasets

The word intrusion datasets consists of a list of words where:
- Three words belong to the core group and are semantically related in one or more aspects
- One word is an outlier

The task is to identify the outlier in the list of words.

This dataset was developed as part of the Danish Reasoning Benchmark.
To cite, please use following citation:

[INDSÆT ARTIKEL...]

All data is based on the Danish Thesaurus. Read more here:
https://euralex.org/wp-content/themes/euralex/proceedings/Euralex%202014/euralex_2014_012_p_191.pdf

## Content

Two granularities:
- Fine 
- Medium

### Fine-grained relatedness

The data is a tab-separated text-file with the following columns:
candidates	label	core_group_placement	outlier_placement

- candidates: list containing core group + outlier (example: ['word_1', 'word_2', 'word_3', 'word_4'])
- label: outlier (example: 'word_3')
- core_group_placement: which section and keyword in the Danish Thesaurus the core group words are taken from (example: chapter 1, section 2, under måne 'moon' = 01.002.måne)
- Outlier_placement: which keyword, subkeyword and dotgroup index the outlier is taken from. Outlier is always from same section as the core group. (example: himmellegeme.stjerne.0) 


### Medium-grained relatedness
The data is a tab-separated text-file with the following columns:
candidates	label	core_group_placement	outlier_placement

- candidates: list containing core group + outlier (example: ['word_1', 'word_2', 'word_3', 'word_4'])
- label: outlier (example: 'word_3')
- core_group_placement: which section in the Danish Thesaurus the core group words are taken from (example: chapter 1, section 2 = 01.002)
- Outlier_placement: which other section the outlier is taken from + dotgroup and concept index (example: chapter 2, section 21, dotgroup number 7, first concept = 02.021.7.0)


## License
[CC BY-ND](https://creativecommons.org/licenses/by-nd/4.0/)

Credit: [Society for Danish Language and Literature](https://dsl.dk/)

Contact: Nathalie Hau Sørensen (nats @ dsl.dk)


