# NFR-Classification-ULMFiT

# ULMFiT for NFR Classification

This repository contains the implementation of ULMFiT (Universal Language Model Fine-tuning) for classifying Non-Functional Requirements (NFR) sentences. The project includes a Jupyter notebook implementing the ULMFiT model using the FastAI library, as well as the dataset used for training, results, and checkpoint files.

## Overview

The Universal Language Model Fine-tuning (ULMFiT) is a transfer learning technique introduced by Jeremy Howard and Sebastian Ruder in their paper ["Universal Language Model Fine-tuning for Text Classification"](https://arxiv.org/abs/1801.06146). It enables effective transfer learning for NLP tasks even with limited annotated data.

In this project, we apply ULMFiT to classify Non-Functional Requirements (NFR) sentences. NFRs represent constraints or criteria that specify how a system should behave, as opposed to what the system should do (Functional Requirements).

## Dataset

The dataset used in this project is located in the `data` directory. It includes a CSV file (`NFR_Dataset.csv`) containing NFR sentences. The dataset is split into training and validation sets using the Data Block API provided by the FastAI library.

## Model Training

The ULMFiT model is trained using the FastAI library within a Jupyter notebook (`ULMFiT_NFR_Classification.ipynb`). The notebook covers the following steps:

1. Data preprocessing and loading using the FastAI `TextList` API.
2. Language model training to fine-tune a pre-trained model on the NFR dataset.
3. Encoder prediction example.
4. Classifier training using the fine-tuned language model.
5. Model evaluation and interpretation.

## Results

The trained model achieves competitive performance on the NFR classification task. Detailed results, including accuracy metrics, loss curves, and examples of misclassified sentences, are provided in the notebook.

## Checkpoint Files

The trained model checkpoints (`fit_head.pth`, `fine_tuned.pth`, `first.pth`, `second.pth`, `third.pth`, `fourth.pth`, `fine_tuned_enc.pth`) are saved in the repository for reproducibility and further experimentation.

## Requirements

- Python >= 3.6
- FastAI
- PyTorch

## Usage

To replicate the experiment or apply the trained model to new data, follow these steps:

1. Clone this repository:

```
git clone https://github.com/your-username/ULMFiT_NFR_Classification.git
```

2. Install the required dependencies:

```
pip install -r requirements.txt
```

3. Run the Jupyter notebook `ULMFiT_NFR_Classification.ipynb` in your local environment.

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to FastAI and PyTorch for providing powerful libraries for deep learning.
- The dataset used in this project is sourced from [provide dataset source if applicable].

## Author

Cody Baker - https://github.com/cbgithub7

```
