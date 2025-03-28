# Fine-Tuning Phi-2 for Text-to-SQL Conversion

This project focuses on fine-tuning Microsoft's Phi-2 language model to enhance its performance in translating natural language queries into SQL statements. By leveraging the [Spider Text-to-SQL dataset](https://www.kaggle.com/datasets/mohammadnouralawad/spider-text-sql), the model is trained to generate accurate SQL queries from plain English questions.

## Project Structure

```
phi2_text2sql_finetuned/
├── data/
│   ├── train_data.json               # Processed training dataset
│   └── Datapreprocessing.ipynb       # Jupyter notebook for data preprocessing
├── notebook/
│   └── Phi2_SQL_FineTuning.ipynb     # Jupyter notebook for model fine-tuning
├── scripts/
│   ├── train.py                      # Script for training the model
│   └── evaluate.py                   # Script for evaluating the model
├── requirements.txt                  # List of required Python packages
└── README.md                         # Project documentation
```

## Dataset

The training data is sourced from the [Spider Text-to-SQL dataset](https://www.kaggle.com/datasets/mohammadnouralawad/spider-text-sql), a large-scale, complex, and cross-domain semantic parsing and text-to-SQL dataset. Special thanks to [Mohammad Nour Alawad](https://www.kaggle.com/mohammadnouralawad) for providing this valuable resource.

## Setup and Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/tarakantaacharya/phi2_text2sql_finetuned.git
   cd phi2_text2sql_finetuned
   ```

2. **Install Dependencies:**

   Ensure you have Python 3.8 or higher installed. Install the required packages using pip:

   ```bash
   pip install -r requirements.txt
   ```

## Data Preprocessing

Before training the model, the raw dataset undergoes preprocessing to format it appropriately for the fine-tuning process. The `Datapreprocessing.ipynb` notebook in the `data/` directory provides a step-by-step guide on how the data is cleaned, transformed, and prepared.

## Model Fine-Tuning

The fine-tuning process is detailed in the `Phi2_SQL_FineTuning.ipynb` notebook located in the `notebook/` directory. This notebook outlines the steps to:

- Load the pre-trained Phi-2 model.
- Prepare the dataset for training.
- Fine-tune the model on the text-to-SQL task.
- Save the fine-tuned model for evaluation and inference.

## Training and Evaluation Scripts

For users who prefer command-line operations, the `scripts/` directory contains:

- `train.py`: Script to initiate model training.
- `evaluate.py`: Script to assess the model's performance on a validation dataset.

Execute these scripts as follows:

```bash
python scripts/train.py
python scripts/evaluate.py
```

## Contributing

Contributions to this project are welcome. If you have suggestions, improvements, or encounter issues, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

*Acknowledgment: This project utilizes the [Spider Text-to-SQL dataset](https://www.kaggle.com/datasets/mohammadnouralawad/spider-text-sql) provided by [Mohammad Nour Alawad](https://www.kaggle.com/mohammadnouralawad). We appreciate their contribution to the research community.* 
