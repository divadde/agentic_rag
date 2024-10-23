# agentic_rag
## About the application:

The work aims to introduce the properties of Trustworthiness, Safeness and Fairness into an agentic retrieval-augmented generation application. Moreover, a concept of multi-aspect rag is introduced using specialized agents called "aspect-agents". LangChain and LangGraph framework are used to build the application. It is showed the overall structure of the computational graph:

![alt text](https://github.com/divadde/agentic_rag/blob/main/imgs/master%20workflow.png)

![alt text](https://github.com/divadde/agentic_rag/blob/main/imgs/aspect%20agent%20workflow.png)

Safeness is guaranteed through an "hate speech detection" module, encoder (supervised finetuning) and decoder (in-context learning) based solutions were performed.
Fairness is guaranteed through a "bias detection" module and a "debiasing" module, decoder based solutions were performed: introducing of Debiasing Score metric to measure quality and quantity of bias deleted.
Trustworthiness is guaranteed through a "textual-entailment task" with KBTs (Knowledge base trusted), this is the most crucial task of the entire pipeline.

Pinecone is used to store informations on Vector Data Stores. It is needed to enter the website of Pinecone to configure KBTs and VDS.

For more informations on the application structure and how properties are assured, see on thesis chapter 3. Experimental results are on Excel tables and explained in chapter 4.

## About the repository structure:

- agentic-rag-trust contains the core of application in form of notebook.
- build-vector-datastore contains the code to build the knowledge base trusted and the vectordatastore content
- in "modules" folder there are the files focused on bias detection, hate speech detection and entailment. each file contains, eventually, finetuning of encoders, prompts and few-shot examples for language models and a phase of testing
- in "previous" folder there are some old versions of the application.

