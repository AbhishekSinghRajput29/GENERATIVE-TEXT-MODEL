# GENERATIVE TEXT MODEL

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: ABHISHEK SINGH RAJPUT

*INTERN ID*: CT04DG3397

*DOMAIN*: ARTIFICIAL INTELLIGENCE

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH

#GENERATIVE TEXT MODEL

```markdown
#  Generative Text Model Using GPT and LSTM

##  Project Overview

This project aims to explore the capabilities of generative text models using two widely known architectures: **GPT (Generative Pre-trained Transformer)** and **LSTM (Long Short-Term Memory)**. The primary goal is to create a system that can generate coherent paragraphs based on specific user-defined prompts. This kind of system can be used in applications like AI content generation, writing assistants, chatbots, storytelling, and educational tools.

The deliverable is a **Jupyter Notebook** that demonstrates the functionality of both models (GPT and optionally LSTM), allowing users to input custom prompts and generate text relevant to the topic.


##  Project Objectives

-  Load and use a pre-trained GPT model from the Hugging Face Transformers library
-  (Optional) Build and train an LSTM-based text generator using a sample corpus
-  Take user-defined prompts as input and generate coherent, topic-specific paragraphs
-  Compare the performance and quality of GPT vs. LSTM
-  Provide clear and modular code in a Jupyter notebook format for ease of understanding and experimentation


##  Tools and Libraries Used

- `transformers`: To load and use pre-trained GPT-2 models
- `torch`: Backend for GPT-based models
- `tensorflow` / `keras`: For building and training LSTM models
- `numpy`, `pandas`: Data processing
- `matplotlib`: For visualizing training progress (if using LSTM)
- `tqdm`: For progress bars
- `Jupyter Notebook`: Interactive development environment


##  Project Structure

```

text-generation-project/
│
├── data/
│   └── sample_texts.txt           # (Optional) Your custom training text
│
├── models/
│   └── lstm_model.h5              # Saved LSTM model
│
├── notebook/
│   └── text_generation_demo.ipynb # Main notebook
│
├── outputs/
│   └── generated_texts.txt        # Text generated by the model
│
├── requirements.txt               # Required packages
└── README.md                      # Project description


````


##  How It Works

### GPT Model:
1. The notebook loads a pre-trained GPT-2 model from Hugging Face.
2. The user enters a prompt (e.g., "The future of space exploration").
3. The model generates a coherent paragraph that follows from the prompt.
4. Results are printed directly and optionally saved.

### LSTM Model (Optional):
1. A dataset (`sample_texts.txt`) is tokenized and vectorized.
2. An LSTM model is built using Keras.
3. The model is trained to predict the next word in a sequence.
4. A text prompt is seeded, and new words are generated recursively.


##  How to Run the Project

1. Clone or download the repository.
2. (Optional) Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
````

3. Install required packages:

   ```bash
   pip install -r requirements.txt
   ```
4. Launch the notebook:

   ```bash
   jupyter notebook notebook/text_generation_demo.ipynb
   ```
5. Run all cells or step through interactively. Provide your own prompts in the designated cells.


##  Example Prompts & Outputs

```python
prompt = "Artificial intelligence in healthcare is"
```

**GPT Output:**

> Artificial intelligence in healthcare is revolutionizing diagnostics, patient care, and personalized medicine. With the ability to process vast amounts of data...


##  Conclusion

This project demonstrates the practical use of generative language models in a controlled environment. GPT-2 produces fluent and relevant paragraphs with minimal training required, showcasing the power of transformer-based architectures. The LSTM model, while more limited in fluency, provides a great learning exercise in understanding sequence modeling from scratch.

By comparing both models, we gain insight into the trade-offs between traditional RNNs (like LSTM) and cutting-edge transformers. The notebook is modular and can be extended to fine-tune models on specific domains, evaluate performance, or serve as a foundation for more complex NLP applications.

