# danish-semantic-reasoning-benchmark
A Danish semantic reasoning benchmark compiled from lexical semantic resources
This benchmark is the first version of a semantic reasoning benchmark for Danish compiled semi-automatically from a number of human-curated lexical-semantic resources, which function as our gold standard. The datasets constitute a benchmark for assessing selected language understanding capacities of large language models (LLMs) for Danish. 

## Beta version
Current version is a beta version and is not yet fully curated. 

This first version comprises 25 datasets across 6 different tasks and include 3,800 test instances. Although still limited in size, we go beyond comparative evaluation datasets for Danish by including both negative and contrastive examples as well as low-frequent vocabulary; aspects which tend to challenge current LLMs when based substantially on language transfer. 
The datasets focus on 

 - semantic inference
 - entailment
 - similarity
 - relatedness, 
 - disambiguation of words in context.  

We have used ChatGPT to assess to which degree our datasets challenge the ceiling performance of state-of-the-art LLMs, average performance being relatively high with an average accuracy of 0.6 on ChatGPT 3.5 turbo and 0.8 on ChatGPT 4.0.

We hope to extend the datasets in the near future depending on funding. 


## Credit and reference
Pedersen, B. S., Sørensen, N. C. H., Olsen, S., Nimb, S. & Gray, S. (in print). Towards a Danish Semantic Reasoning Benchmark - Compiled from Lexical-Semantic Resources for Assessing Selected Language Understanding Capabilities of Large Language Models. In *Proceedings of the Fourteenth Language Resources and Evaluation Conference.*

[Center for Language Technology, Department of Nordic Studies and Linguistics, University of Copenhagen](https://cst.ku.dk/english/)

and

[Society for Danish Language and Literature](https://dsl.dk/)

