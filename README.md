# NEXT-WORD-PREDICTION

# Text Generation Using LSTM and Sherlock Holmes Stories

This project demonstrates how to build a **Text Generation** model using an **LSTM (Long Short-Term Memory)** neural network, implemented in **TensorFlow/Keras**. The model is trained on the **Sherlock Holmes** stories dataset and can generate text that mimics the style of Sir Arthur Conan Doyle's writing.
## **Overview**

This project utilizes **Natural Language Processing (NLP)** techniques, specifically tokenization and sequence padding, to prepare text data for training an LSTM model. The model learns to predict the next word in a sequence based on previous words. Once trained, the model is used to generate new text based on a seed input.

## **Requirements**

Before running this project, make sure you have the following Python libraries installed:

- **TensorFlow** (for building and training the LSTM model)
- **NumPy** (for array manipulation)
- **Keras** (for text preprocessing and model building)
You can install the required packages via pip:

```bash
pip install tensorflow numpy
```
## **Code Explanation**

### **Text Preprocessing:**
- **Tokenization**: Converts words into numerical indices.
- **Sequence Creation**: Forms small word sequences for the model to learn.
- **Padding**: Makes all sequences the same length.

### **Model Architecture:**
- **Embedding Layer**: Converts word indices into dense vectors.
- **LSTM Layer**: Learns word patterns over time.
- **Dense Layer**: Predicts the next word based on learned patterns.
- **Softmax Activation**: Converts predictions into probabilities.

### **Model Training:**
- The model is trained with **categorical crossentropy** and **Adam optimizer** for 5 epochs.
