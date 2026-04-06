# CS 6350 - Big Data Management & Analytics
## Assignment 2

**Authors:** Sreevasan Sivasubramanian (sxs220434), Rithwik Chittineni (rvc220000)

---

## Requirements

- Python 3.x
- Apache Spark 3.5.x
- PySpark
- NLTK

## Installation

```bash
pip install pyspark nltk
```

---

## Files

- `friend_recommendation_mapreduce.py` — Part 1.1: Friend recommendation using MapReduce
- `ALS_friend_recommendation.py` — Part 1.2: Friend recommendation using ALS collaborative filtering
- `NaiveBayesClassifier.py` — Part 2: Naive Bayes text classifier using MapReduce
- `CS 6350 Report.pdf` — Report covering all three parts
- `CS6350_CoverPage.pdf` — Cover page

---

## Running the Code

### Part 1.1 — MapReduce Friend Recommendation
```bash
spark-submit friend_recommendation_mapreduce.py
```

### Part 1.2 — ALS Friend Recommendation
```bash
spark-submit ALS_friend_recommendation.py
```

### Part 2 — Naive Bayes Classifier
```bash
spark-submit NaiveBayesClassifier.py
```

---

## Notes

- All datasets are downloaded automatically on first run — no local paths are hardcoded
- The LiveJournal dataset is downloaded from: https://an-ml.s3.us-west-1.amazonaws.com/soc-LiveJournal1Adj.txt
- The SMS Spam dataset is downloaded from: https://raw.githubusercontent.com/5sansiva/CS6350-Assignment2/refs/heads/main/SPAM%20text%20message%2020170820%20-%20Data.csv
- All scripts use `random.seed(42)` for reproducibility
- Parts 1.1 and 1.2 generate recommendations for the same 10 users
- The LiveJournal dataset is large (~4M users) — Part 1.1 and 1.2 may take several minutes to run locally

