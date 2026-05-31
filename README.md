# AI Resume Analyzer

## Overview

AI Resume Analyzer is a Natural Language Processing (NLP) project that analyzes resumes and compares them with job descriptions to evaluate candidate suitability.

The system extracts text from resumes, processes the content, identifies important skills, and calculates the similarity between a resume and a target job role. This helps recruiters and job seekers quickly assess resume relevance.

---

## Features

- Resume text extraction
- Job description analysis
- NLP-based text preprocessing
- Skill matching
- Resume-job similarity scoring
- Candidate ranking support
- Automated resume evaluation

---

## Technologies Used

- Python
- Pandas
- NumPy
- NLTK
- Scikit-learn
- TF-IDF Vectorization
- Cosine Similarity
- Google Colab

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/ai-resume-analyzer.git
cd ai-resume-analyzer
```

### Install Dependencies

```bash
pip install pandas numpy nltk scikit-learn
```

---

## Project Workflow

1. Load resume data
2. Load job description
3. Clean and preprocess text
4. Remove stopwords and unwanted characters
5. Convert text into numerical vectors using TF-IDF
6. Calculate similarity scores
7. Rank resumes based on relevance
8. Display matching results

---

## Data Preprocessing

The text preprocessing stage includes:

- Lowercase conversion
- Punctuation removal
- Stopword removal
- Tokenization
- Text normalization

Example:

```python
text = text.lower()
```

---

## Feature Extraction

TF-IDF Vectorization is used to convert textual information into numerical features.

```python
from sklearn.feature_extraction.text import TfidfVectorizer

vectorizer = TfidfVectorizer()
```

---

## Similarity Calculation

Cosine Similarity is used to compare resumes with job descriptions.

```python
from sklearn.metrics.pairwise import cosine_similarity

similarity = cosine_similarity(tfidf_matrix)
```

---

## Usage

Run the notebook and provide:

- Resume content
- Job description

The model will generate a similarity score indicating how closely the resume matches the target role.

---

## Example Output

```text
Resume Match Score: 87.5%
```

### Interpretation

| Score Range | Meaning |
|------------|---------|
| 80% - 100% | Excellent Match |
| 60% - 79% | Good Match |
| 40% - 59% | Moderate Match |
| Below 40% | Weak Match |

---

## Project Structure

```text
AI_Resume_Analyzer.ipynb
README.md
```

---

## Applications

- Resume screening
- Candidate ranking
- Recruitment automation
- Job recommendation systems
- HR analytics

---

## Future Improvements

- PDF Resume Upload Support
- Skill Gap Analysis
- ATS Compatibility Scoring
- Resume Recommendations
- Deep Learning-based Resume Ranking
- Web Application Deployment
- Multi-Resume Comparison

---

## License

This project is intended for educational and learning purposes.
