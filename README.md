# Sentiment Analysis in Movie Reviews

This project focuses on utilizing various neural network architectures to perform sentiment analysis on the IMDB movie review dataset. Our goal is to classify reviews into positive or negative sentiments based on their content. The project explores the following models: Simple RNN, LSTM, Deep LSTM, and Bidirectional LSTM, providing insights into their performance and effectiveness.

## Dataset

We use the IMDB movie review dataset, which comprises 50,000 reviews divided evenly into training and testing sets. Each set contains an equal number of positive and negative reviews, allowing for a balanced sentiment analysis task.

## Models Overview

### Simple RNN

A basic RNN model serving as our baseline. It includes an embedding layer, a simple RNN layer, and a dense layer for output.

### LSTM (Long Short-Term Memory)

Improves upon the Simple RNN by addressing the vanishing gradient problem, making it better suited for long text sequences.

### Deep LSTM

A more complex model that features two LSTM layers. This model aims to capture deeper linguistic structures and relationships within the text data.

### Bidirectional LSTM

Expands on the LSTM model by processing the text data in both forward and reverse directions, offering a comprehensive understanding of the context.

## Implementation

The TensorFlow and Keras libraries were employed to construct and train our models. The Sequential API facilitated the stacking of layers in each model architecture.

## Results and Discussion

- The **Simple RNN** model showed initial promise but was ultimately limited by its simplistic nature, achieving around 79.10% accuracy.
- The **LSTM model** marked a significant improvement, with accuracy reaching approximately 84.34%, demonstrating the LSTM's capability in handling long-term dependencies.
- The **Deep LSTM model** further enhanced performance, slightly outperforming the standard LSTM with an accuracy of 84.90%, indicating the potential benefits of deeper architectures.
- The **Bidirectional LSTM** achieved the highest accuracy at 85.21%, underscoring the advantage of understanding text context from both directions.

## Conclusion

Our exploration underscores the effectiveness of LSTM-based models, particularly the Bidirectional LSTM, in sentiment analysis tasks. These models' ability to grasp the nuances of language and context significantly contributes to their superior performance over the simpler RNN model.