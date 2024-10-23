# agentic_rag
## About the application:

The work aims to introduce the properties of Trustworthiness, Safeness and Fairness into an agentic retrieval-augmented generation application. Moreover, a concept of multi-aspect rag is introduced using specialized agents called "aspect-agents". LangChain and LangGraph framework are used to build the application. It is showed the overall structure of the computational graph:

![alt text](https://github.com/divadde/agentic_rag/blob/main/imgs/master%20workflow.png)

![alt text](https://github.com/divadde/agentic_rag/blob/main/imgs/aspect%20agent%20workflow.png)

Safeness is guaranteed through an "hate speech detection" module, encoder (supervised finetuning) and decoder (in-context learning) based solutions were performed.
Fairness is guaranteed through a "bias detection" module and a "debiasing" module, decoder based solutions were performed: introducing of Debiasing Score metric to measure quality and quantity of bias deleted.
Trustworthiness is guaranteed through a "textual-entailment task" with KBTs (Knowledge base trusted), this is the most crucial task of the entire pipeline.

For more informations on the application structure and how properties are assured, see on thesis chapter 3. Experimental results are on Excel tables and explained in chapter 4.

## About the repository structure:

(TODO)

