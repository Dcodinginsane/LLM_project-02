# Train a Language Model on your WhatsApp Chats
## Overview
This repository facilitates the training of a character-level or word-level language model solely based on WhatsApp chat messages. After model training, one can kick-off a synthetic conversation with the trained on Whatsapp chat group. <br>
- <b>Chat messages:</b> I have privately trained the model on Whatsapp chats from a group with >8 Mio characters. The <code>assets/input/chat.txt</code> is just a placeholder, to be replaced with the actual corpus of chat messages.
- <b>Language model:</b>
The model closely follows the architecture introduced in "Attention Is All You Need" (2017) by Vaswani et. al.. Also the pytorch implementation of the model is heavily inspired by a [video tutorial by Andrew Kaparty](https://www.youtube.com/watch?v=kCc8FmEb1nY).
- <b>Results:</b> While the overall performance of my privately trained model is clearly not comparable with sota language models, the generated text clearly exhibits recognizable lingusitic patterns and vocabulary.

## Folder Structure
```
|-- assets
|   |-- input
|   |   |-- chat.txt
|   |-- output
|   |   |-- contacts.txt
|   |   |-- vocab.txt
|   |   |-- train.pt
|   |   |-- valid.pt
|   |-- models
|   |   |--model.pt
|-- src
|   |-- chat.py
|   |-- model.py
|   |-- preprocess.py
|   |-- train.py
|   |-- utils.py
|-- config.py
|-- run.py
```

