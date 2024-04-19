# Named Entity Recognition (NER) Project

This project is an implementation of Named Entity Recognition (NER) using Python and spaCy library.

## Overview

Named Entity Recognition (NER) is a subtask of information extraction that seeks to locate and classify named entities mentioned in unstructured text into pre-defined categories such as the names of persons, organizations, locations, expressions of times, quantities, monetary values, percentages, etc.

This project utilizes spaCy, a popular natural language processing library, for performing NER on text data.

## Requirements

- Python 3.x
- spaCy library

## Installation

1. Clone the repository:

```bash
git clone <repository_url>

## Install the required dependencies

pip install -r requirements.txt

## Download the spaCy language model:

python -m spacy download en_core_web_sm

## Navigate to the project directory:

cd named-entity-recognition

## Run the main script:

python named_entity_recognition.py

## Input the text you want to perform NER on.

## Here's an example of how to use this project:

import spacy

# Load the 'en_core_web_sm' model
nlp = spacy.load('en_core_web_sm')

# Process the text
text = nlp('Hi, My name is Lahari \n I am from India \n I want to work with Google \n Steve Jobs is My Inspiration')

# Print named entities
for ent in text.ents:
    print(ent.text, ent.label_)


