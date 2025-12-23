# Bollywood Movies Metadata — Cinelytics

This repository contains the **Bollywood Movies Metadata** dataset curated and published by *Cinelytics*. It provides structured information on Indian films covering metadata, sentiment indicators, financial performance, and commercial verdicts. The dataset supports research, analytics, sentiment studies, and predictive modeling in film industry data science.

## Dataset Overview

The dataset consists of **20,282 entries** with structured metadata for Indian feature films. Each row corresponds to a single movie and includes:

- **Title**  
- **Release Year, Opening Month, Opening Date**
- **Director, Cast, Genre, Production Studio**
- **Budget and Box Office Performance** (India and Worldwide)
- **Audience Sentiment Metrics** (from trailer comments and review text)
- **Commercial Verdict** (e.g., Hit, Flop, Disaster)

The dataset merges classical film metadata with sentiment features to enable a wide range of analytical and machine learning use cases.


### Key Attributes

| Feature Category | Example Fields |
|------------------|----------------|
| Basic Metadata   | `Title`, `Year`, `Genre`, `Director`, `Cast`, `Studio` |
| Financial        | `Budget`, `India Gross`, `Worldwide Gross_scraped` |
| Sentiment        | `Trailer_comment_positive`, `Trailer_comment_negative`, `Review_positive`, `Review_negative` |
| Derived Metrics  | `budget_num`, `india_gross_num`, `Verdict` |

Sample dataset excerpt (from DataHub KGP):

```

Title | Year | Opening_Month | Director | Cast | Genre | Budget | India Gross | Trailer_comment_positive | Review_negative | budget_num | india_gross_num | Verdict

````

> This dataset is suitable for film industry research, exploratory data analysis, sentiment analysis, predictive modelling, and data visualizations. :contentReference[oaicite:1]{index=1}

---

## Contents of This Repository

This repository includes:

- **Dataset_with_Verdict.csv**  
  The primary dataset file with movie metadata, financial numbers, sentiment features, and commercial verdicts.

- **Jupyter Notebooks**  
  Example analyses and workflows:
  - `Movie list.ipynb` — Movie list exploration
  - `Review sentiments.ipynb` — Sentiment feature extraction and visualization
  - `Sentiment Analysis.ipynb` — Model building and evaluation
  - `Youtube Trailer Comments and their sentiment analysis.ipynb` — Trailer comments scraping and sentiment extraction

- **Model Artifacts**
  - `binary_sentiment_model.pkl` — Pretrained binary sentiment classification model
  - `movie_reviews.csv` — Movie review dataset used for sentiment training

- **LICENSE**  
  MIT License governing dataset usage and repository content.

---

## Example Use Cases

The dataset can be employed for:

- **Exploratory Data Analysis**  
  Understand patterns in Bollywood movie releases, genres, and industry trends.

- **Sentiment Analysis**  
  Analyze the relationship between sentiment from reviews/trailers and box office performance.

- **Predictive Modelling**  
  Build models to predict movie success (e.g., verdict) using metadata and sentiment scores.

- **Data Visualization**  
  Visual storytelling with performance trends, genre impacts, cast/director correlations, etc.

---

## Getting Started

To begin using the dataset:

1. **Clone the Repository**
   ```bash
   git clone https://github.com/jainharsh524/Bollywood_Movies_Metadata-Cinelytics.git
   cd Bollywood_Movies_Metadata-Cinelytics
   ```

2. **Explore the Dataset**
   Open the dataset file (`Dataset_with_Verdict.csv`) in a spreadsheet or load it using Python (Pandas).

   ```python
   import pandas as pd

   df = pd.read_csv("Dataset_with_Verdict.csv")
   df.head()
   ```

3. **Run Example Analyses**
   Open the provided Jupyter notebooks to explore sentiment extraction, data visualizations, and modeling workflows.

---

## Citation

If you use this dataset in your research or project, please consider citing:

```
Indian Film Metadata, Box Office Performance, and Sentiment Dataset.
DataHub KGP: https://datahubkgp.org/datasets/datasetDetails.php?id=c8938ab30fc0ba3f3b11
```

---

## License

This repository and its contents are released under the **MIT License**.

---

## Contact

For questions or contributions, feel free to open an issue or submit a pull request.
