# Danish Word in Context Dataset

The Word in Context Dataset consist of a target word, two contexts with the target word and a label (same_sense, different_sense).
The position of the target word in each context is also given.

The task is tell whether the use of the target word in the two contexts are examples of the same sense or two different senses.
The task indirectly tests the ability to disambiguate word senses.

This dataset was developed as part of the Danish Reasoning Benchmark.
To cite, please use following citation:

Bolette Pedersen, Nathalie Sørensen, Sussi Olsen, & Sanni Nimb. 2024. 
Evaluering af sprogforståelsen i danske sprogmodeller – med udgangspunkt i semantiske ordbøger. 
*NyS - Nydanske Sprogstudier*, *65*, 8-40. Artikel 1. https://doi.org/10.7146/nys.v1i65.143072


The data is based on the semantic module of the COR resource. Read more here:\
Bolette Pedersen, Nathalie Sørensen, Sanni Nimb, Ida Flörke, Sussi Olsen & Thomas Troelsgård. 2022.
[Compiling a suitable level of sense granularity in a lexicon for AI purposes: The open source COR lexicon.](https://aclanthology.org/2022.lrec-1.6.pdf) 
In *Proceedings of the Thirteenth Language Resources and Evaluation Conference* (pp. 51-60).


## Content
The data is a tab-separated tsv-files with the following columns:
target	first_context	second_context	label	first_word	first_position	second_word	second_position	idx

- target = target word (example: *word_1*)
- first_context = context sentence 1 (example: *A sentence with word_1*)
- second_context = context sentence 2 (example: *Another sentence with word_1*)
- label = whether the contexts are examples of the *same_sense* or *different_sense* according to the sense descriptions in COR.SEM
- first_word = exact word form of the target in context 1
- first_position = character index in the context of the first and last character of the target word in context 1
- second_word = exact word form of the target in context 2
- second_position = character index in the context of the first and last character of the target word in context 2
- idx = id number

We provide two files:
- danwic_mono_selection = dataset with only monosemous words and therefore the label is always *same_sense*
- danwic_poly_selection = dataset with polysemous words


# License
[CC BY-ND](https://creativecommons.org/licenses/by-nd/4.0/)

Credit: [Society for Danish Language and Literature](https://dsl.dk/)

Contact: Nathalie Hau Sørensen (nats @ dsl.dk)

