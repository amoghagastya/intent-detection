# Intent Detection Assignment: Approach and Analysis

## Framing the Problem:
I framed intent detection as a multi-class classification problem.

Initially, I considered traditional ML/NLP methods like SVM, TF-IDF, n-grams, and RASA but quickly realized these methods are too resource-intensive and domain-specific—definitely not ideal for scalable, real-world Conversational AI solutions.

Given these constraints, I shifted my focus toward zero-shot classification using Large Language Models (LLMs). This approach appealed to me because it eliminated the tedious pre-training process, making it robust and highly scalable across different business domains.

## Model Building and Comparative Analysis:
In my notebook - intent_detection.ipynb, I explore a diverse range of intent detection methods:

1. Zero-shot classification models:
- Facebook’s BART-large-mnli model (general-purpose NLI-based zero-shot).
- FLAN-T5 fine-tuned zero-shot classifier from the open-intent-classifier package.
- Additional top-ranked Hugging Face models like DeBERTa variants.

2. Embedding-based methods:
Leveraged embeddings to map user utterances and intent descriptions into a shared semantic space, achieving promising accuracy but still dependent on embedding quality.

3. LLM-based methods:
Tested different prompting strategies with powerful language models. Specifically, I evaluated two distinct prompt structures and discovered that a simpler, more direct prompt significantly outperformed complex, verbose prompts.

The comparative evaluation highlighted the clear advantages of specialized fine-tuning—even a smaller model (flan-t5) with minimal fine-tuning significantly improved performance.
Impressively, using the optimized simple-prompt LLM-based approach, I achieved around 90% accuracy on the test set, with zero domain-specific training required. These results strongly validate the shift towards general-purpose NLU through LLMs.

## Running the Notebook
You'll need to create a .env file in the root dir and add Huggingface and OpenAI API keys to run the notebook. Full .env file link attached in email.

## Justifying Results:
The results are not just impressive in isolation—they represent a meaningful leap forward for Conversational AI. Traditionally, intent detection requires exhaustive pre-training for each business domain, an approach that's simply unsustainable at scale.

Achieving a ~90% accuracy rate with zero-shot classification signals a powerful paradigm shift, opening doors to scalable and universally applicable intent detection solutions powered by advanced LLMs.

## Suggested Improvements:
However, there's always room to optimize further. Currently, the approach embeds all possible intents within the LLM prompt, which can be costly and increase latency for large-scale intents.

My primary suggestion for enhancing the model’s efficiency involves integrating a Retrieval-Augmented Generation (RAG) system. By embedding all intent labels and descriptions beforehand, the system could dynamically retrieve and present only the top relevant intents in response to user queries. This would dramatically reduce cost and latency, improving the overall efficiency and scalability of the solution.

Overall, the methods I've implemented provide a strong foundation for scalable, robust, and efficient intent detection, aligned closely with the future trajectory of Conversational AI.

