# LDA Grievance Topic Modeling

Advanced Latent Dirichlet Allocation (LDA) topic modeling system for analyzing grievance-related documents and extracting meaningful topics from organizational texts.

## Project Overview

This project implements a comprehensive topic modeling analysis using LDA to identify patterns and themes in grievance documents. The analysis processes large volumes of text data to discover hidden topics and provide insights into organizational grievance patterns.

## Key Results

- **Documents Analyzed**: 2,957 grievance-related documents
- **Optimal Topics Identified**: 18 topics
- **Coherence Score**: 0.3373
- **Vocabulary Size**: 19,486 unique terms
- **Average Document Length**: 920.8 words

## Features

- Automated text preprocessing and cleaning
- Optimal topic number detection using coherence scores
- Interactive visualizations with pyLDAvis
- Word cloud generation for each topic
- Comprehensive document-topic distribution analysis
- Grievance keyword mapping and analysis
- Statistical performance metrics

## Installation

1. Clone the repository:
```bash
git clone https://github.com/rozaghaedi/lda-grievance-topic-modeling.git
cd lda-grievance-topic-modeling
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

3. Download NLTK data (run in Python):
```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('wordnet')
nltk.download('omw-1.4')
nltk.download('punkt_tab')
```

## Usage

### Running the Analysis
1. Open the Jupyter notebook: `LDA_Grievance_Topic_Modeling.ipynb`
2. Upload your Excel file containing grievance data when prompted
3. Execute all cells to perform the complete analysis

### Data Format
Your input data should be an Excel file with text content in columns such as:
- 'PDFText'
- 'Description' 
- 'Content'
- Or similar text-based columns

The system automatically identifies the most suitable text column for analysis.

## Methodology

1. **Data Preprocessing**: Text cleaning, tokenization, stop word removal, lemmatization
2. **Topic Optimization**: Coherence score analysis to determine optimal number of topics
3. **Model Training**: LDA model training with optimized parameters
4. **Visualization**: Interactive topic visualization and word cloud generation
5. **Analysis**: Document-topic distribution analysis and keyword mapping

## Output

The analysis generates:
- Topic coherence and perplexity scores
- Interactive topic visualization (HTML)
- Word clouds for each identified topic
- Document-topic probability distributions
- Grievance keyword analysis across topics
- Statistical summaries and performance metrics

## Model Performance

- **Model Type**: Latent Dirichlet Allocation (LDA)
- **Topics**: 18 (optimized via coherence analysis)
- **Coherence Score**: 0.3503 (final model)
- **Perplexity**: -7.5573
- **Processing Time**: Approximately 10-15 minutes for full analysis

## Technical Details

- **Language**: Python
- **Primary Libraries**: Gensim, pyLDAvis, NLTK, pandas
- **Visualization**: Matplotlib, Seaborn, WordCloud, Plotly
- **Environment**: Jupyter Notebook / Google Colab compatible

## Requirements

- Python 3.7+
- See `requirements.txt` for complete dependency list
- Minimum 4GB RAM recommended for processing large datasets
- Internet connection required for NLTK data downloads


