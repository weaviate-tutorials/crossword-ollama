# Crossword Puzzle Generator

This repository contains code that creates clues and answers for a topic
that you supply. It uses the clue-answer pairs to create a crossword puzzle.

The project uses an LLM from [Ollama](https://ollama.com/) that is hosted
locally. Ollama provides an interface to the LLM.

The first notebook shows you how to import data and create a collection that
you can use to generate the clue-answer pairs. The example uses Sherlock Holmes
as a subject. You can also change the subject and the input data.

The other notebook generates the puzzle.

## Get started

There are two notebooks in the `jupyter-notebooks` directory
[`crossword-setup.ipynb`](#setup) and
[`crossword-create-puzzle.ipynb`](#generate-a-puzzle).

### Setup

The `crossword-setup.ipynb` notebook does these things:

- Gathers prerequisites
- Sets up a collection
- Imports data
- Connects you to a locally hosted LLM

### Generate a puzzle

The `crossword-create-puzzle.ipynb` notebook does these things:

- Creates a list of puzzle answers
- Creates clues for each answer
- Uses the clue-answer pairs to generate a puzzle

## Requirements

This project requires Ollama. If haven't already installed Ollama, follow the
instructions on the Ollama website to download it.

There are sample data files from [Project Gutenberg](https://www.gutenberg.org/)
in the `inputs` folder. If you want to change the data in the collection, you
need to change the input files.

## Credits

The code that uses the list to generate a puzzle is a lightly modified version
of the [`crossword_helmig`](https://github.com/jeremy886/crossword_helmig)
project.

The sample data is from [Project Gutenberg](https://www.gutenberg.org/).