# PHI-ISIIL Phishing URL Dataset

## Overview
The **PHI-ISIIL Phishing URL Dataset** is a publicly available dataset designed to support research in cybersecurity, specifically in detecting phishing websites. The dataset contains labeled URLs categorized as either **phishing** or **legitimate**, making it suitable for training and evaluating machine learning models in phishing detection.

## Dataset Source
- **Original Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/967/phiusiil+phishing+url+dataset)
- **Contributors:** Safaa Zareapoor and Abdullah Gani
- **Domain:** Cybersecurity, Machine Learning, Phishing Detection

## Dataset Description
The dataset consists of a collection of URLs with various extracted features that help distinguish phishing sites from legitimate ones. It includes:
- **URL-based features:** Characteristics derived from the structure and composition of the URL.
- **Domain-based features:** Information about the domain, such as age, DNS records, and WHOIS details.
- **Content-based features:** Features extracted from the website’s HTML and JavaScript.

## Data Format
The dataset is typically provided in CSV format with the following columns:
- `URL`: The web address being analyzed.
- `Features`: A set of numerical and categorical attributes extracted from the URL and web content.
- `Label`: A binary classification label where:
  - `0` represents a **legitimate** website.
  - `1` represents a **phishing** website.

## Usage
This dataset can be utilized for:
- Training and testing machine learning models for phishing detection.
- Feature engineering and selection to improve classification performance.
- Benchmarking different cybersecurity approaches in phishing prevention.

## How to Use
1. **Download the Dataset:**
   - Clone this repository or manually download the dataset files.
   - Alternatively, fetch the dataset directly from the [UCI Repository](https://archive.ics.uci.edu/dataset/967/phiusiil+phishing+url+dataset).


2. **Load the Dataset in Python:**
   ```python
   import pandas as pd

   # Load dataset
   df = pd.read_csv('PHI_ISIIL_Phishing_URL_Dataset.csv')

   # Display first few rows
   print(df.head())
   ```

3. **Train a Machine Learning Model:**
   ```python
   from sklearn.model_selection import train_test_split
   from sklearn.ensemble import RandomForestClassifier
   from sklearn.metrics import accuracy_score

   # Splitting data
   X = df.drop(columns=['URL', 'Label'])
   y = df['Label']
   X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

   # Train model
   model = RandomForestClassifier()
   model.fit(X_train, y_train)

   # Evaluate model
   y_pred = model.predict(X_test)
   print("Accuracy:", accuracy_score(y_test, y_pred))
   ```

## Citation
If you use this dataset in your research, please cite:
```
@misc{phiisiil2023,
  title={PHI-ISIIL Phishing URL Dataset},
  author={Safaa Zareapoor and Abdullah Gani},
  year={2023},
  url={https://archive.ics.uci.edu/dataset/967/phiusiil+phishing+url+dataset}
}
```

## License
This dataset is provided for research purposes. Please refer to the original source for licensing details.


---
This repository serves as a research resource to help combat cyber threats through machine learning techniques. Happy coding!

