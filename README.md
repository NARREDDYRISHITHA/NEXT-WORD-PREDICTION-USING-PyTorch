# Pytorch Notebooks Repository
Welcome to my Torch Noteboks repository contains a collection of Jupyter notebook and code related to deep learning project using Pytorch

## Overview
In this repository, you will find notebooks and code examples covering a wide range of topics related to deep learning and PyTorch, including:

**1. Python:** Python is a popular choice for machine learning and natural language processing tasks
due to its simplicity and extensive ecosystem of libraries.

**2. PyTorch:** PyTorch is utilized to define the architecture of the neural network
(LexiconModel) and to perform training and inference operations. The model learns the
probability distribution of the next word given the current word, which is crucial for
generating predictions.

**3. Numpy:** NumPy provides support for numerical operations on multi-dimensional arrays and
matrices. It is used in the code to manipulate data efficiently, particularly in converting
data into tensors, which are the primary data structures used by PyTorch for computations.
NumPy helps in handling numerical data and performing computations required during
the preprocessing steps and training process.

**4. String Module:** In the next-word prediction model, the
‘string’ module is used to preprocess words by converting them to lowercase and
removing punctuation marks. This preprocessing ensures consistency in the representation
of words, which is essential for the accurate modeling of word transitions and predictions.

#### Steps Involved:

**1. Data Preprocessing:** It reads a dataset file and preprocesses each word by converting it to
lowercase and removing punctuation. It then creates a dictionary, where each word maps to a
dictionary of subsequent words along with their frequencies.

**2. Model Definition:** It defines a neural network model (Lexicon Model) using PyTorch. The
model architecture includes an embedding layer, a linear layer, and a softmax activation
function.

**3. Lexicon Conversion:** The lexicon dictionary is converted into tensors suitable for training.
Each word and its subsequent words are represented as tensors with corresponding transition
probabilities.

**4. Model Training:** The model is trained using cross-entropy loss and the Adam optimizer.
Training iterates over the lexicon, treating each word as input and its subsequent word as the
target output.

**5. Prediction:** After training, the code enters a prediction loop where that prompts the user for
input. It attempts to predict the next word based on the last word entered by the user, using the
trained model.

**6. Evaluation:** The effectiveness of the model should be evaluated after training. Metrics such
as loss during training, accuracy on a validation set, or even human evaluation of generated
sequences can be used to assess performance.

**7. Deployment:** Once the model is trained and evaluated, it can be saved for future use.
Integration into applications or systems where word prediction functionality is required can be
considered.

### Getting Started
# Prequisites
Before you begin, ensure you have met the following requirements:

      Python 3.9+
      
      PyTorch (Install it using pip install torch)
      
      Jupyter Notebook (Install it using pip install jupyter) or Colab(online platform)
      
