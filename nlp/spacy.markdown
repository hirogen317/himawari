spacy: Python NLP library



Features:

Tokenization
POS Tagging
Dependency Parsing

Lemmatization

Sentence Boundary Detection

Named Entity Recognition

Entity Linking

Similarity: Comparing words text spans and documents and ow similar they are

Text Classification

Rule-based matching

Training

Serialization

Binary weights for the part of speech tagger

Lexical entries

Data files

Word vectors

Configuration


Liguistic annotations

```bash
python -m spacy download en_core_web_sm
```


```python
nlp = spacy.load("en_core_web_sm")
```


Language object containing all components and data needed to process text


when you call nlp on a text, spacy first tokenizes the text to produce a doc, the doc is then processed in several different steps, referred to as the processing pipeline.


displaCy visualizer


Vocab, hash

Lexeme : context-independent information about a word.


Knowledge Base


stores external knowledge in KnowledgeBase
entity linking task

knowledge base is created by first adding all entities to it.

for each potential mention or alias, a list of relevant KB IDs and their prior probabilities is added.



Candidate generation

candidate generation:
KB can provide a list of plausible candidates or entity identifiers. The EntityLinker

will take tis list of candidates as input, and disambiguate the mention to the most probable identifier


Serialization: save your progress


Training: 

Language

Stop words

Tokenizer exceptions

Norm exceptions

Punctuation rules

Character classes

Lexical attributes

Syntax iterators

Tag map

Morph rules

Lemmatizer


Lightning tour



https://github.com/nltk/nltk
https://stanfordnlp.github.io/CoreNLP/


https://spacy.io/usage/spacy-101#annotations-pos-deps