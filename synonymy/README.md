# Danish Synonymy selection dataset

The Danish Synonymy Selection Dataset consist of a target word and a list of
synonym candidates. The task is to identify the correct synonym among the candidates.

The list is constructed so the candidates can be placed on a 
scale of relevance for the target word:
- Closest = synonym
- Next closest = from same section in the Danish Thesaurus
- same broad topic/category = from the same chapter in the Danish Thesaurus
- Furthest: random concept from an unrelated chapter / section

This dataset was developed as part of the Danish Reasoning Benchmark.
To cite, please use following citation:

[INDSÆT ARTIKEL...]

All data is based on the Danish Thesaurus. Read more here:
https://euralex.org/wp-content/themes/euralex/proceedings/Euralex%202014/euralex_2014_012_p_191.pdf

## Content
The data is a tab-separated text-file with the following columns:
target	candidates	label	comment	section

- target = target word (example: word_1)
- candidates = list of candidates (example: ['word_2', 'word_3', 'word_4', 'word_5'])
- label = correct synonym from the candidates (example: 'word_3')
- comment = 'true_synonym' means is it also a registred synonym in the Danish Dictionary. We include this comment as we intend to expand the dataset in the future with near synonyms.
- section = which section from the Danish Thesaurus the target is from (example: 01.002 = chapter 1, section 2)

There is currently 288 instances in the first version.

# License

[CC BY-ND](https://creativecommons.org/licenses/by-nd/4.0/)

