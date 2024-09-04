# Crossword Puzzle Generator

This repository contains code that creates questions and answers for a topic
that you supply. It uses the question-answer pairs to create a crossword puzzle.

You supply an initial prompt. The code searches a vectorized collection of
Wikipedia data and generates a list of people and places that are associated
with the topic. The list is a list of potential puzzle answers.

Once it has the list of answers, the code searches the Wikipedia collection
again to create a clue for each answer.

Finally, the code passes the list of clues and answers to a puzzle generator.
The puzzle generator creates a crossword puzzle that uses as many of the answers
as it can fit into a puzzle grid.

## Get started

There are two notebooks in the `juypter-notebooks` directory.

### Setup

Use `crossword-setup.ipynb` to create a collection of data based on Wikipedia.

The notebook uses the Simple English subset of the Wikipedia data set from
Cohere.

This is where the language is configured: `import_wiki_data("simple", num_rows, skip_rows)`.

To import a different language, uncomment one of the other import rows or edit
the code to add the language name.

### Generate a puzzle

Use `crossword-create-puzzle.ipynb` to generate the puzzle.

The example code creates a puzzle based on the Harry Potter series. This is the
query prompt: `query="Get the name of a Harry Potter character or the name of a
place associated with Harry Potter"` To change the puzzle topic, edit the query
prompt.

## Requirements

This project uses [Cohere](https://cohere.com/) for the data set and LLM. You
need a Cohere API key to run the code in `crossword-create-puzzle.ipynb`.

## Credits

The code that generates the list of clues and answers is new.

The code that uses the list to generate a puzzle is a lightly modified version
of the [`crossword_helmig`](https://github.com/jeremy886/crossword_helmig)
project.
