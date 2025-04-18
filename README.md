# Shakespeare-Text-Generation-using-RNNs-LSTMs-and-GRUs

📌 Project Overview

This project explores the use of advanced Recurrent Neural Networks (RNNs) to perform creative text generation in the style of Shakespeare. Using the original plays as training data, the model learns to generate new, stylistically consistent text sequences.

We compare different RNN variants — Vanilla RNN, LSTM, and GRU — and evaluate them using quantitative (perplexity) and qualitative (text fluency) measures. To boost performance and realism, we also implement:

	•	Temperature-controlled sampling
	•	Beam search
	•	Teacher forcing
	•	Gradient clipping

⸻

🎯 Objectives

	•	Train and compare Vanilla RNN, LSTM, and GRU for text generation
	•	Improve training stability and generation quality using advanced sequence modeling techniques
	•	Evaluate text generation using perplexity, coherence, and fluency
	•	Provide a reproducible pipeline for sequence generation with customizable hyperparameters

⸻

💡 Value Proposition

	•	Demonstrates deep learning proficiency in sequence modeling
	•	Showcases creativity in model evaluation via both quantitative and qualitative analysis
	•	Applies state-of-the-art generation techniques relevant to real-world NLP applications: chatbots, creative writing tools, summarizers, etc.
	•	Offers employers a hands-on look at PyTorch NLP fluency, model tuning, and sequence generation expertise

⸻

🧪 Techniques Used

📚 Dataset

	•	Source: Shakespeare Corpus (shakespeare_plays.csv)
	•	Filtered to use 3 representative plays: Hamlet, Coriolanus, and Richard III
	•	Tokenized using Byte-Pair Encoding (BPE) with ByteLevelBPETokenizer

🧼 Data Preprocessing

	•	Character-level and subword tokenization
	•	Sequence windowing with input-target pairs
	•	Train-validation split and batching using torch.utils.data.DataLoader

🧠 Model Architectures

	•	Vanilla RNN: Simple RNN layers with hidden state propagation
	•	LSTM (Long Short-Term Memory): Adds memory cell gates to improve long-term retention
	•	GRU (Gated Recurrent Unit): A more efficient alternative to LSTM
	•	All architectures use embedding layers and are implemented using PyTorch

⚙️ Training Optimization

	•	Teacher Forcing: To accelerate convergence and stability
	•	Gradient Clipping (clip_grad_norm_): Prevents exploding gradients
	•	Optimizer: Adam
	•	Loss: Cross-entropy

🔍 Text Generation Strategies

	•	Temperature-controlled sampling: Adjusts randomness in word selection
	•	Beam Search: Produces more coherent outputs by keeping top-k sequences at each time step
	•	Generation starts with seed input and stops at a pre-set length or punctuation

📊 Evaluation

	•	Perplexity: Measures model uncertainty; lower = better
	•	Qualitative: Side-by-side comparison of text generated by different models
	•	Samples include both default and beam search generations for each RNN type

⸻
Future Enhancements

	•	Integrate Transformer-based models (e.g., GPT-2, BART) for next-gen performance
	•	Enable live deployment as a Shakespearean chatbot via Streamlit or Flask
	•	Expand to multi-author stylized generation (e.g., compare Shakespeare vs. modern poetry)****
