# Resea: Virtual Research Assistant

Resea is a research automation agent built using Python, Hugging Face Transformers, and Gradio.
It provides structured research reports by retrieving, summarizing, and evaluating sources from Wikipedia and the web.

## 💻 Features
- Topic-based content retrieval
- Real-world article retrieval using SerpAPI
- Wikipedia-based summaries and citations
- Article summarization using Hugging Face's BART model
- Source credibility evaluation
- Report generation in `.docx` and `.pdf` formats
- Gradio UI with mascot and file downloads (.docx + .pdf)

## Technologies Used
- Gradio (web interface)
- Hugging Face Transformers (`facebook/bart-large-cnn`)
- SerpAPI (search)
- newspaper3k (article parsing)
- ReportLab & python-docx (PDF + Word generation)

## 🚀 How to Use (Colab)
1. Open the notebook in Google Colab.
2. Run all cells top to bottom.
3. Upload your mascot image when prompted.
4. Enter a topic and click 'Generate Report'.
5. Download the resulting files.

## 🛠 Setup (Locally)
1. Clone repo:
```bash
git clone https://github.com/yourusername/resea-agent.git
cd resea-agent
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Add your API key to `config.py`:
```python
SERPAPI_KEY = "your-serpapi-key-here"
```

4. Run the app:
```bash
python main.py
```

## 📁 Files Included
- `main.py`: Main Resea assistant logic
- `requirements.txt`: All dependencies
- `config.txt`: For setting Agent (excluding keys)

## Notes
- No OpenAI API required
- Ensure your mascot image is named `resea_mascot.png`
- Output reports are generated dynamically and downloadable via Gradio

## License
This project is licensed under the MIT License.
