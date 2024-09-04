# Crossword Puzzle Generator

This repository contains code that creates questions and answers for a topic
that you supply. It uses the question-answer pairs to create a crossword puzzle.

The generator uses an LLM that is hosted locally. Ollama provides an interface
to the LLM.

## Get started

There are two notebooks in the `juypter-notebooks` directory.

### Setup

The `crossword-setup.ipynb` notebook connects you to a locally hosted LLM.

### Generate a puzzle

The `crossword-create-puzzle.ipynb` notebook generates the puzzle.

The example code creates a puzzle based on the Sherlock Holmes stories. To
change the puzzle topic, edit the query prompt.

## Requirements

This project requires [Ollama](https://ollama.com/). If haven't already
installed Ollama, follow the instructions on the Ollama website to download it.

## Credits

The code that generates the list of clues and answers is new.

The code that uses the list to generate a puzzle is a lightly modified version
of the [`crossword_helmig`](https://github.com/jeremy886/crossword_helmig)
project.
