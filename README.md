# Seq2Seq English-French Translator

Utilizing TensorFlow, I've developed a translator between English and French using the `Seq2Seq` model. This implementation strongly emphasizes the use of **Batch Training**.

## 📝 Project Overview

- Due to TensorFlow's "define and run" structure, I've set **checkpoints** at intervals to ensure the stability of the learning process.
- Instead of the default `seq2seq` tool, I approached the model with a **dynamic** design and implementation.
- The whole project is divided into four ipython files. Running the `main` will automatically import the other three files.

## 💡 Key Features

- **Batch Training**: For efficient learning, I adopted the batch training technique to process data in batches.
- **Separated Encoder and Decoder**: I've designed the Encoder and Decoder as distinct structures, allowing for intricate adjustments and optimizations.
- **Dynamic Seq2Seq**: I've adjusted and used TensorFlow's predefined graph in a more flexible manner.
- **Attention Mechanism**: I enhanced the accuracy of translations using a dot product attention mechanism within the Decoder.

## 📚 Study Content

While utilizing TensorFlow, I delved deep into studying the following core topics:

- `get_variable_scope`, `get_variable`, `variable_scope`
- Various applications of `tf.scan`
- Usage of `place_holder`, `sparse_place_holder`, etc.

## 📌 Note

This project was inspired by the pytorch tutorial, so some similarities in structure or content might be observed.
