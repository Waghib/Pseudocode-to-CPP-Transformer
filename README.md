# Pseudocode to C++ Transformer

A bidirectional translation system powered by transformer neural networks that converts between pseudocode and C++ code. This project implements two separate transformer models: one that translates pseudocode to C++ and another that converts C++ code to pseudocode, providing a valuable tool for programming education and development.

## 🚀 Features

- **Bidirectional Translation**: Convert from pseudocode to C++ and vice versa
- **Transformer Architecture**: Utilizes state-of-the-art transformer neural networks for accurate translations
- **Interactive UI**: Built with Streamlit for an intuitive user experience
- **Local Deployment**: Easily run the application on your local machine

## 📋 Requirements

- Python 3.8+
- PyTorch
- Streamlit
- Other dependencies listed in `requirements.txt`

## 🔧 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Waghib/Pseudocode-to-CPP-Transformer.git
   cd Pseudocode-to-CPP-Transformer
   ```

2. Set up a virtual environment (recommended):
   ```bash
   python -m venv poetry_env
   # On Windows
   .\poetry_env\Scripts\activate
   # On Unix or MacOS
   source poetry_env/bin/activate
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## 💻 Usage

1. Activate the virtual environment if you haven't already:
   ```bash
   # On Windows
   .\poetry_env\Scripts\activate
   # On Unix or MacOS
   source poetry_env/bin/activate
   ```

2. Run the Streamlit application:
   ```bash
   python -m streamlit run app.py
   ```

3. Open your web browser and navigate to:
   ```
   http://localhost:8501
   ```

4. Use the interface to:
   - Select the translation mode (C++ → Pseudocode or Pseudocode → C++)
   - Enter your code in the text area
   - Click "Translate" to generate the translation

## 🧠 Model Architecture

The translation system uses a sequence-to-sequence transformer architecture with:

- **Embedding Layer**: Converts tokens to vector representations
- **Positional Encoding**: Adds positional information to the embeddings
- **Transformer Encoder-Decoder**: Processes the input sequence and generates the output sequence
- **Multi-head Attention**: Allows the model to focus on different parts of the input sequence
- **Feed-forward Networks**: Processes the attention outputs

### Model Parameters:
- Vocabulary Size: 12,006 tokens
- Maximum Sequence Length: 100 tokens
- Embedding Dimension: 256
- Number of Attention Heads: 8
- Number of Transformer Layers: 2
- Feedforward Dimension: 512
- Dropout Rate: 0.1

## 📁 Project Structure

- `app.py`: Main Streamlit application for the user interface
- `transformer.ipynb`: Jupyter notebook containing model training code
- `vocabulary.json`: JSON file containing the vocabulary for tokenization
- `transformer_epoch_1.pth`: Trained model for pseudocode to C++ translation
- `cpp_to_pseudo_epoch_1.pth`: Trained model for C++ to pseudocode translation
- `requirements.txt`: List of Python dependencies
- `README.md`: Project documentation

## 🔄 Training Process

The models were trained on a dataset of paired pseudocode and C++ code examples. The training process involved:

1. Data preprocessing and tokenization
2. Training the transformer models with teacher forcing
3. Evaluating the models on validation data
4. Saving the best-performing models

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 📧 Contact

For any questions or feedback, please reach out to the repository owner.

---

*This project was developed as part of advanced research in programming language translation using transformer neural networks.*
