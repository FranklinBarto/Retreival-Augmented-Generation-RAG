# Retreival-Augmented-Generation-RAG
Python-based FAQ retrieval system designed to answer common questions about Golden Retrievers


# Golden Retriever FAQ Retrieval System

This repository contains a Python-based FAQ retrieval system designed to answer common questions about Golden Retrievers. It utilizes fuzzy matching and semantic search techniques to handle various ways a question may be phrased, offering relevant answers from a predefined FAQ database.

## Features
- **Comprehensive FAQ Dataset**: The system is equipped with a wide range of AI generated FAQs about Golden Retrievers.
- **Fuzzy Matching**: Handles user queries that are close but not identical to predefined FAQ questions using fuzzy matching with the `rapidfuzz` library.
- **Semantic Search**: Uses embedding-based similarity (via language models) to find semantically similar questions, ensuring flexibility in understanding different phrasings of the same question.

## Usage

1. **Run the Jupyter Notebook**:
    ```bash
    jupyter notebook
    ```

2. **Load the FAQ Retrieval System**:
    The FAQ retrieval system can be run directly in the notebook. You can query it by providing a natural language question related to Golden Retrievers.

    Example of a query:
    ```python
    query = "How long do Golden Retrievers live?"
    answer = retrieve_with_fuzzy_faq(query)
    print(answer)
    ```

3. **Customize the FAQ Database**:
    The FAQ database can be easily modified by adding or removing questions in the `faq` dictionary. You can extend the system with new questions and answers about Golden Retrievers as needed.

4. **Open a pull request**.

You are welcome contributions in the form of additional FAQs, optimizations to the retrieval system, or improved handling of queries.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
