# IMDB-Sentiment-Classifier-with-BERT-Gradio-UI

IMDB Sentiment Classifier (BERT + Gradio)A machine learning application that performs binary sentiment analysis on movie reviews using a fine-tuned BERT (Bidirectional Encoder Representations from Transformers) model. The project includes a sleek, interactive web interface powered by Gradio for real-time predictions.🚀 OverviewThis repository demonstrates how to leverage State-of-the-Art (SOTA) NLP models to classify text. By fine-tuning the bert-base-uncased model on the IMDB dataset, the classifier achieves high accuracy by understanding the context and nuance of cinematic reviews.Key FeaturesTransformer-based Logic: Utilizes the Hugging Face transformers library.Interactive UI: A simple, browser-based interface to test custom reviews.Pre-processing Pipeline: Automated tokenization and padding for raw text input.Efficiency: Designed to run on both GPU (CUDA) and CPU.🛠️ Tech StackModel: BERT (via Hugging Face)Framework: PyTorchUI: GradioDataset: IMDB Movie ReviewsLanguage: Python 3.8+📦 InstallationClone the RepositoryBashgit clone https://github.com/your-username/IMDB-Sentiment-Classifier.git
cd IMDB-Sentiment-Classifier
Create a Virtual EnvironmentBash    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3.  **Install Dependencies**
    ```bash
    pip install -r requirements.txt
    ```

---

## 🖥️ Usage

### 1. Training (Optional)
If you wish to re-train the model or fine-tune it further:
```bash
python train.py
2. Launch the Web UITo start the Gradio interface and test the model:Bashpython app.py
After running, a local URL (typically [http://127.0.0.1:7860](http://127.0.0.1:7860)) will be provided in your terminal.🧠 Model PerformanceThe model was fine-tuned with the following hyperparameters:Max Length: 128-512 tokensBatch Size: 16Optimizer: AdamWLearning Rate: $2 \times 10^{-5}$MetricScoreAccuracy~92%F1-Score0.91📂 Project StructurePlaintext├── models/               # Saved model weights and configs
├── notebooks/            # EDA and experimental training scripts
├── app.py                # Gradio interface script
├── train.py              # Model training and evaluation script
├── requirements.txt      # List of dependencies
└── README.md             # Project documentation
🤝 ContributingContributions make the open-source community an amazing place to learn and create.Fork the Project.Create your Feature Branch (git checkout -b feature/AmazingFeature).Commit your Changes (git commit -m 'Add some AmazingFeature').Push to the Branch (git push origin feature/AmazingFeature).Open a Pull Request.
