(SQAC TASK)
This project automatically categorizes expense transactions
Objective
To develop a **Smart Expense Categorizer** that:
- Reads transaction text (e.g., `Swiggy 250`, `Uber 300`, etc.)
- Classifies it into an appropriate expense category using **TF-IDF** + **Logistic Regression**

Used
- Python 
- Google Colab  
- Pandas  
- Scikit-learn (TF-IDF, Logistic Regression)  
- NumPy  

Dataset
The dataset (`transactions_1000.csv`) contains 1000 labeled examples like:
| Swiggy 250 | Food |
| Uber 300 | Travel |
| Flipkart 1200 | Shopping |
| Netflix 499 | Entertainment |
| Apollo Pharmacy 1500 | Medical |

How It Works
1. Data Loading: CSV dataset is read using `pandas`.  
2. Feature Extraction: Transaction text is converted to numerical form using TF-IDF Vectorizer.  
3. Model Training: A Logistic Regression** model is trained on these TF-IDF vectors.  
4. Prediction: The model predicts the category for new transactions.  
5. Evaluation: Model accuracy is calculated using `accuracy_score`.

Results
After training on 1000 rows, the model achieved:
**Accuracy: 1.0 (100%)**

Example Prediction
| Input Text | Predicted Category |
|-------------|--------------------|
| "Zomato 400" | Food |
| "Uber 250" | Travel |
| "Spotify Premium 119" | Entertainment |


Files Included
| File | Description |
|------|--------------|
| `SQAC_Project.ipynb` | Google Colab notebook with code |
| `transactions_1000.csv` | Dataset used for training |
| `README.md` | Project documentation |


Author
**Ajeet Singh**  
ML enthusiast and CSE UG  

How to Run
1. Clone this repository:
   git clone https://github.com/AjeetSingh21/Project-SQAC.git
