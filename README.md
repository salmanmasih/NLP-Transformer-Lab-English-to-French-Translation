🧠 NLP Transformer Lab: English to French Translation
This project demonstrates how to fine-tune a pre-trained MarianMT Transformer model on a custom dataset of English–French sentence pairs. It includes full training, evaluation, and error analysis — built with Hugging Face Transformers and Datasets.

🚀 Features
✅ Load and tokenize parallel English–French data

✅ Fine-tune Helsinki-NLP/opus-mt-en-fr using 🤗 Transformers

✅ BLEU score evaluation on test set

✅ Custom error analysis with category breakdowns

✅ Visualization of translation performance

📂 Project Structure
bash
Copy
Edit
nlp-translation-lab/
│
├── translate_lab.ipynb        # Main notebook: data, training, evaluation
├── eng-french.csv             # Sample dataset (first 500 parallel sentences)
├── analyze_translation.py     # (Optional) Script for running error analysis
├── requirements.txt           # Python dependencies
└── README.md                  # Project documentation
🧪 Dataset
The dataset used for training is a parallel corpus of English–French sentences. You can swap in your own dataset by replacing eng-french.csv.

📊 Evaluation Metrics
BLEU Score using sacrebleu

Custom error categories:

Perfect/Near Perfect

Minor Issues

Major Errors

Completely Wrong

📈 Visualizations
BLEU score per sentence (bar chart)

BLEU score vs. sentence length (scatter plot)

📦 Installation
Make sure you have Python 3.8+ installed, then run:

bash
Copy
Edit
pip install -r requirements.txt
🏃 Usage
Launch the main notebook:

bash
Copy
Edit
jupyter notebook translate_lab.ipynb
Or run the script directly:

bash
Copy
Edit
python analyze_translation.py
📈 Sample Output
yaml
Copy
Edit
Test BLEU Score: 26.97
Perfect translations: 4 / 6
Major Errors: 1 | Completely Wrong: 1
📚 Dependencies
transformers

datasets

evaluate

sacrebleu

sentencepiece

matplotlib

pandas

numpy

🧠 Acknowledgments
Built using:

Hugging Face Transformers

MarianMT for Machine Translation

🔖 License
MIT License – feel free to use, share, and modify!

