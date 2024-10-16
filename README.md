
# Virtual TA for Berkeley Large Language Model Agents Course

## Overview

This project provides a **virtual Teaching Assistant (TA)** for the **[CS294/194-196 Large Language Model Agents](https://rdi.berkeley.edu/llm-agents/f24)** course at UC Berkeley. It utilizes a Retrieval-Augmented Generation (RAG) system, built using LangChain and PGVector, to create a knowledge base that helps students by providing factual, contextually relevant answers to course-related questions.

The system allows users to load and query course materials, such as scientific papers, lecture notes, and other documents. It is powered by HuggingFace embeddings and uses PostgreSQL with PGVector for efficient semantic search. The local LLaMA model (Ollama) generates responses based on the most relevant documents retrieved from the knowledge base. This RAG system acts as a virtual TA to assist students in engaging with course content.

## Features

- Acts as a virtual TA for the Berkeley CS294/194-196 course.
- Load documents from PDF, text, or JSON files, including lecture materials and scientific papers.
- Split documents into manageable chunks for efficient processing and search.
- Vectorize and store documents using HuggingFace embeddings in a PostgreSQL database with PGVector.
- Query the knowledge base using natural language questions, with responses generated by the local LLaMA model.
- Scrape web pages and integrate their content into the knowledge base, expanding the system's resources.

## Course Description

The **[Berkeley CS294/194-196 Large Language Model Agents](https://rdi.berkeley.edu/llm-agents/f24)** course explores the development and application of large language models (LLMs) across various domains, including code generation, robotics, web automation, and scientific discovery. The course also covers foundational aspects of LLMs, their abilities, agent infrastructure, as well as ethical considerations, privacy issues, and the future directions of LLMs.

### Topics Covered:

- **LLM Fundamentals**: Task automation and agent infrastructure.
- **LLM Applications**: Code generation, web automation, multimodal agents, and robotics.
- **Limitations and Future Directions**: Privacy, safety, ethics, and multi-agent collaboration.

### Syllabus

| Lecture # | Date     | Topic                                     | Guest Lecture                             |
|-----------|----------|-------------------------------------------|-------------------------------------------|
| 1         | Sept 9   | LLM Reasoning                             | Denny Zhou, Google DeepMind               |
| 2         | Sept 16  | LLM Agents: Brief History and Overview    | Shunyu Yao, OpenAI                        |
| 3         | Sept 23  | Agentic AI Frameworks & AutoGen           | Chi Wang, AutoGen-AI                      |
| 4         | Sept 30  | Enterprise Trends for Generative AI       | Burak Gokturk, Google                     |
| 5         | Oct 7    | Compound AI Systems & the DSPy Framework  | Omar Khattab, Databricks                  |
| 6         | Oct 14   | Agents for Software Development           | Graham Neubig, Carnegie Mellon University |
| 7         | Oct 21   | AI Agents for Enterprise Workflows        | Nicolas Chapados, ServiceNow              |
| 8         | Oct 28   | Neural Networks with Symbolic Decision-Making | Yuandong Tian, Meta AI (FAIR)         |
| 9         | Nov 4    | Foundation Agent                          | Jim Fan, NVIDIA                           |
| 10        | Nov 18   | Cybersecurity, Agents, and Open-Source    | Percy Liang, Stanford University          |
| 11        | Dec 2    | LLM Agent Safety                          | Dawn Song, UC Berkeley                    |


## Virtual TA for LLM Agents Course

The **KnowledgeBase RAG with PGVector** serves as the virtual TA for the **[CS294/194-196 Large Language Model Agents](https://rdi.berkeley.edu/llm-agents/f24)** course. The system assists students by providing factual, detailed answers based on course materials, which include lectures, readings, and assignments. Using the RAG pipeline, students can query the virtual TA for insights into course topics and receive contextually accurate information.

This AI-powered TA enhances students' learning experience, ensuring they stay engaged with the rapidly evolving field of large language model agents.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/virtual-ta-llm-agents.git
   cd virtual-ta-llm-agents
   ```

2. Install dependencies:
   ```bash
   conda env create -f environment.yml
   conda activate llm
   ```

3. Setup PostgreSQL with PGVector:
   - Ensure PostgreSQL is installed and running.
   - Follow the [PGVector installation guide](https://github.com/pgvector/pgvector) to enable vector support in PostgreSQL.

4. Set up the virtual environment:
   ```bash
   source setup.sh
   ```

## Running the Application

1. After setting up the environment, run the Streamlit app:
   ```bash
   streamlit run main.py
   ```

## License

This project is licensed under the Apache License 2.0. See the [LICENSE](./LICENSE) file for more details.

For any inquiries, feel free to use the virtual TA and explore the topics discussed in the course!

Contact: mmemari@uvu.edu
