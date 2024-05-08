# Multilingual Speech Recognition Model for RAG

## Introduction
This project aims to build a multilingual speech recognition model for Retrieval-Augmented Generation (RAG) without the need for training. The model leverages OpenAI's Whisper-medium for its robust multilingual speech recognition capabilities and integrates it with Langchain's RetrialQA and the Mistral-7B language model for enhanced performance on tasks like translation and summarization.

## Project Overview
The project consists of the following key steps:

1. **Preprocessing**:
   - Video to Audio Conversion: Utilize the moviepy library to convert video files into audio format.
   - Audio Chunking: Segment the audio into smaller chunks to accommodate Whisper's limitations on audio size.

2. **Multilingual Speech Recognition with Whisper**:
   - Model Selection: Employ OpenAI Whisper medium model for its multilingual speech recognition capabilities.
   - Combining Transcriptions: Combine all transcriptions after segmenting the audio into chunks.

3. **RAG Model Integration**:
   - FAISS Vector Store: Establish a vector store using FAISS for efficient information retrieval from the database.

4. **Leveraging the Final Model**:
   - Langchain's RetrialQA: Combine retrieval with the Mistral-7B(llm) model for enhanced performance.

5. **Using the Model for Tasks**:
   - Task Execution: Provide appropriate prompts for tasks like translation and summarization of text.

6. **Evaluating the Model**:
   - Summarization Evaluation: Utilize rouge metrics for evaluating the summarization tasks.
   - Translation Evaluation: Implement sacrebleu metrics for evaluating translation tasks.

## Dependencies
- Python 3.x
- moviepy
- OpenAI Whisper
- FAISS
- Langchain
- Mistral-7B


## Conclusion
This project demonstrates a comprehensive approach to building a multilingual speech recognition model for RAG without the need for training. By leveraging OpenAI's Whisper-medium, FAISS, Langchain, and the Mistral-7B language model, the model can effectively handle tasks like translation and summarization. The project can be further extended and optimized based on specific requirements and use cases.