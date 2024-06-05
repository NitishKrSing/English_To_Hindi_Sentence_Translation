# English to Hindi Sentence Translation using LSTM

This repository contains code to build a model for English to Hindi sentence translation using Long Short-Term Memory (LSTM) neural networks. LSTM is a type of recurrent neural network (RNN) architecture capable of learning sequences of data, making it suitable for translation tasks.

## Overview

- **Data Preparation:** The corpus consists of English sentences paired with their Hindi translations, each sentence containing '<start>' and '<end>' tokens.
- **Tokenization:** Tokenize the English and Hindi sentences using the Keras `Tokenizer` class.
- **Model Architecture:** Implement a sequence-to-sequence model with an encoder-decoder architecture using Keras. The encoder embeds the input English sentences and passes the output to an LSTM layer. The decoder then takes the embedded Hindi sentences and outputs the translated text.
- **Training:** Train the model on the English and Hindi sentence pairs. The model is optimized using the Adam optimizer and categorical cross-entropy loss function.
- **Inference:** Use the trained model to translate new English sentences to Hindi.

## Instructions

### Prerequisites

- Install Python (3.x recommended) and necessary libraries: NumPy, TensorFlow, and Keras.

### Usage

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/your-username/english-to-hindi-translation.git
    ```

2. Navigate to the project directory:

    ```bash
    cd english-to-hindi-translation
    ```

3. Run the Python script `translation_model.py`:

    ```bash
    python translation_model.py
    ```

4. Input an English sentence when prompted. The script will translate it to Hindi using the trained model and display the result.

## Example

```python
input_sentence = "Thank you"
translated_sentence = translate_sentence(input_sentence)
print(f'Input: {input_sentence}')
print(f'Translated: {translated_sentence}')
