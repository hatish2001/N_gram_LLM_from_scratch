
# Neural Network for Character-Level Name Generation

This repository contains a neural network built using PyTorch that performs character-level name generation. The model is trained on a dataset of names and predicts the next character given a sequence of previous characters.

## Project Overview

This project demonstrates how to:
- Build a vocabulary from a dataset of names.
- Construct input-output pairs for training a neural network using a sliding window approach.
- Train a simple neural network to predict the next character in a sequence.
- Generate names using the trained model.

### Key Features:
- Character embedding: Each character is mapped to a fixed-size embedding vector.
- Sliding window approach: The model is trained using a fixed-size context to predict the next character.
- Random initialization of embedding weights for learning.

## Files

- **My_first_nn.ipynb**: The main notebook that contains all the code for data preparation, model building, and training.
- **names.txt**: The dataset of names used for training. Each line contains a single name.
- **README.md**: This file, providing details about the project and instructions for usage.

## Requirements

To run this project, you need the following dependencies:

- Python 3.7 or later
- PyTorch
- Matplotlib

You can install the necessary dependencies using:

```bash
pip install torch matplotlib
```

## Usage

1. Clone the repository to your local machine:

```bash
git clone https://github.com/your_username/your_repository_name.git
```

2. Open the Jupyter notebook `My_first_nn.ipynb` and run all the cells. This will:

   - Read the dataset (`names.txt`).
   - Create a vocabulary mapping for characters.
   - Build the dataset for training the neural network.
   - Initialize and train the neural network to predict the next character.
   - Display results and generate names based on the trained model.

3. You can modify the `block_size` parameter to change the size of the context used for name generation.

## Dataset

The `names.txt` file is a simple text file containing a list of names, one per line. You can replace this file with any list of names to train the model on a different dataset.

## Model

The neural network is a basic feed-forward model, where:

- Characters are embedded into vectors using an embedding matrix.
- The input is a sequence of characters (context), and the output is the next predicted character.
- The model is trained using negative log-likelihood loss.

## Results

Once trained, the model can generate names based on learned character sequences. The longer the training time, the better the model gets at generating realistic names.

## Contributing

Feel free to submit issues or pull requests if you find bugs or want to contribute to this project.

