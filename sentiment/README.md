# Danish Sentiment in Context Dataset

The Danish Sentiment in Context Dataset consist of a target word, a context with the target word and a sentiment label.
Additionally, we also provide the specific word form in the context and position.

The task is to give a sentiment label on a scale from negative (-3) to neutral (0) to positive (3) to the target word given the context.

This dataset was developed as part of the Danish Reasoning Benchmark.
To cite, please use following citation:



All data is based on the semantic module of the COR resource. Read more here:\
Bolette Pedersen, Nathalie Sørensen, Sanni Nimb, Ida Flörke, Sussi Olsen & Thomas Troelsgård. 2022.
[Compiling a suitable level of sense granularity in a lexicon for AI purposes: The open source COR lexicon.](https://aclanthology.org/2022.lrec-1.6.pdf) 
In *Proceedings of the Thirteenth Language Resources and Evaluation Conference* (pp. 51-60).


## Content
The data is a tab-separated text-file with the following columns:
target  context form    position    label

- target = target word (example: *word_1*)
- context = context sentence (example: *word_1 is a negative word*)
- form = word form in the context (e.g. conjugated form) 
- position = character index in the context of the first and last character of the target word
- label = sentiment value on a scale from *-3* to *+3*

There is currently 489 instances in the first version.

# License
[CC BY-ND](https://creativecommons.org/licenses/by-nd/4.0/)

Credit: [Society for Danish Language and Literature](https://dsl.dk/)

Contact: Nathalie Hau Sørensen (nats @ dsl.dk)

