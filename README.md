# Markov Chain Text Generator

## Introduction

A Markov chain is a mathematical system that undergoes transitions from one state to another within a finite or countable number of possible states. It is characterized by the property that the next state depends only on the current state and not on the sequence of events that preceded it. This memoryless property is known as the Markov property. Markov chains are used to model a variety of random processes in fields such as physics, finance, and biology.

## Project Overview

This project is an implementation of a random text generator using Markov chains, written in Go. The generator can produce random text based on the patterns learned from a given input text. By analyzing the frequency of word sequences in the input text, the generator creates a model that can be used to generate new, coherent text.

## How to Run the Project

1. **Clone the Repository:**
   ```sh
   git clone https://github.com/aaivanov23/markov-text-generator.git
   cd markov-text-generator
2. **Build the Project**
    ```sh
    go build
    ```
3. **Run the Generator**
    ```sh
    ./markov-text-generator -input=input.txt -output=output.txt -length=100
    ```
    - `-input`: Path to the input text file used for building the model.
    - `-output`: Path to the output text file where the generated text will be saved.
    - `-length`: The number of words to generate.

## Input text

The generator can use any text file to build the model. Examples of suitable input texts include:

- Literary works (e.g., novels, poems)
- Articles and essays
- Transcripts of speeches or dialogues

By providing different input texts, the generator can produce a wide range of stylistic outputs, mimicking the patterns and vocabulary of the original source.

## Example

To generate text using a sample input file `example.txt`, run the following command:

```sh
./markov-text-generator -input=example.txt -output=generated.txt -length=200
```

This command will produce a text file `generated.txt` with 200 words generated based on the patterns found in `example.txt`.

## Conclusion

This Markov chain text generator offers a simple yet powerful way to create random, coherent text based on any input source. By leveraging the principles of Markov chains, it can mimic the style and structure of various text genres, providing a versatile tool for text generation tasks.