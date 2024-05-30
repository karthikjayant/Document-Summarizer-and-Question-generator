# Document-Summarizer-and-Question-generator
Addressing the challenge of extracting insights efficiently from dense PDF documents, this website introduces a Document Summarizer & Question Generator tool. Leveraging state-of-the-art natural language processing (NLP) models such as FLAN T5 for document summarization and GPT-3.5-Turbo for question generation, the website aims to simplify the navigation and comprehension of complex textual content.

#Methodology:

##Development of Document Summarizer:
The document summarization phase utilizes FLAN T5, a variant of the T5 model fine-tuned for various NLP tasks. FLAN T5 excels in compressing large documents into concise summaries while retaining key information. Fine-tuning on datasets like WikiSum and DialogSum enhances its summarization capabilities across different domains. Additionally, Pegasus, a transformer-based model designed for abstractive text summarization, further improves summarization quality through fine-tuning on the SamSum dataset.

##Development of Question Generator:
The question generation phase employs GPT-3.5-Turbo, an advanced NLP model developed by OpenAI. With its transformer architecture and large parameter count, GPT-3.5-Turbo generates contextually relevant questions based on provided documents. While fine-tuning enhances performance, the website implements the model without fine-tuning to manage computational costs. Users can customize question parameters such as quantity and difficulty level to tailor generated questions.

##Application Interface Development with Streamlit:
Integrating the document summarization and question generation models into a user-friendly web application using Streamlit, the website allows users to easily upload documents and interact with the summarization and question generation pipeline. Upon document upload, the backend processes the document and generates summaries and questions, which are then displayed to users. Additional features such as customization options enhance user experience.

#Constraints:
Despite its efficacy, the website faces certain constraints. The use of powerful NLP models like FLAN T5 and GPT-3.5-Turbo imposes limitations on computing resources and model complexity. Fine-tuning these models requires substantial time, effort, and skill, while GPT-3.5-Turbo's computational requirements may restrict its practical application in resource-constrained scenarios. Extensive testing is necessary to ensure the reliability and performance of the website under various user interactions and document types.
