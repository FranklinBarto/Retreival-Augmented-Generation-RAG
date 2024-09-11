# Retreival-Augmented-Generation-RAG
Python-based FAQ retrieval system designed to answer common questions about Golden Retrievers


# Golden Retriever FAQ Retrieval System

This repository contains a Python-based FAQ retrieval system designed to answer common questions about Golden Retrievers. It utilizes fuzzy matching and semantic search techniques to handle various ways a question may be phrased, offering relevant answers from a predefined FAQ database.

## Features
- **Comprehensive FAQ Dataset**: The system is equipped with a wide range of FAQs about Golden Retrievers, covering topics like lifespan, diet, grooming, training, health, and more.
- **Fuzzy Matching**: Handles user queries that are close but not identical to predefined FAQ questions using fuzzy matching with the `rapidfuzz` library.
- **Semantic Search**: Uses embedding-based similarity (via language models) to find semantically similar questions, ensuring flexibility in understanding different phrasings of the same question.

## Table of Contents
- [Retreival-Augmented-Generation-RAG](#retreival-augmented-generation-rag)
- [Golden Retriever FAQ Retrieval System](#golden-retriever-faq-retrieval-system)
  - [Features](#features)
  - [Table of Contents](#table-of-contents)
  - [Installation](#installation)
  - [Usage](#usage)
  - [FAQ Examples](#faq-examples)
  - [Contributing](#contributing)
  - [License](#license)

## Installation

1. **Clone this repository**:
    ```bash
    git clone https://github.com/yourusername/golden-retriever-faq-retrieval.git
    cd golden-retriever-faq-retrieval
    ```

2. **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

    The key dependencies include:
    - `rapidfuzz`: For fuzzy matching of queries
    - `torch`: For embedding-based semantic search
    - `transformers`: To load and use pre-trained language models for embeddings
    - `datasets`: To handle the FAQ dataset and perform search operations

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

## FAQ Examples

Here are some example questions the system can handle:

- **What is the average lifespan of a Golden Retriever?**
    - The average lifespan of a Golden Retriever is around 10 to 12 years.
  
- **How much exercise do Golden Retrievers need?**
    - Golden Retrievers need at least one hour of exercise per day. This can include walking, running, or playing fetch.

- **What are common health issues in Golden Retrievers?**
    - Common health issues in Golden Retrievers include hip dysplasia, elbow dysplasia, cataracts, and heart problems.

The system can handle different phrasings, such as:
- *How long do Golden Retrievers usually live?*
- *What is the life expectancy of a Golden Retriever?*

## Contributing

1. **Fork the repository**.
2. **Create a new branch** for your feature or bug fix:
    ```bash
    git checkout -b feature-name
    ```
3. **Commit your changes**:
    ```bash
    git commit -m "Add new feature"
    ```
4. **Push to the branch**:
    ```bash
    git push origin feature-name
    ```
5. **Open a pull request**.

We welcome contributions in the form of additional FAQs, optimizations to the retrieval system, or improved handling of queries.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.
