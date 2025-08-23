
# 📚 Book Recommendation System  

**Book Recommendation System** is a machine learning project that suggests books to users based on **Popularity-Based Filtering** and **Content-Based Filtering**.  
It allows users to discover trending books and also find books similar to the ones they love — making reading choices smarter and more personalized.  
## 📊 Dataset  

This project uses the **Books Dataset from Kaggle**:  
📌 [Kaggle Dataset - Book Recommendation Dataset](https://www.kaggle.com/datasets/arpitpadmani/ml-book-recommendation-system)  

It includes:  
- **Users** (user IDs, demographics)  
- **Books** (title, author, publisher, etc.)  
- **Ratings** (explicit/implicit feedback)  
## 📽️ Demo Video  

Watch the demo of **Book Recommendation System** in action:  

[![Watch the video](https://img.youtube.com/vi/6b5e3ba4-0b73-46de-9d1f-9a850f6e1470/0.jpg)](https://github.com/user-attachments/assets/6b5e3ba4-0b73-46de-9d1f-9a850f6e1470)  

---

## 🚀 Features  

- ⭐ **Popularity-Based Recommendations**  
  → Suggests top-rated and trending books based on user ratings.  

- 📖 **Content-Based Recommendations**  
  → Recommends books similar to a chosen one using author, genre, and metadata.  

- 🧠 **Hybrid Approach**  
  → Combines popularity and content similarity for better results.  

- 🌐 **Interactive Web App**  
  → Simple and user-friendly interface built with **Flask**.  

 

## 🧠 How It Works  

1. **Popularity-Based Filtering**:  
   - Aggregates ratings and calculates weighted score.  
   - Displays the most popular books across the dataset.  

2. **Content-Based Filtering**:  
   - Computes **cosine similarity** between book descriptions.  
   - Finds books with high similarity scores to the input.  

3. **Pre-processed Data**:  
   - Uses `.pkl` files (saved models) for faster predictions.  

 

## 🔧 Installation  

### 1. Clone the Repository  

```bash
git clone https://github.com/Arpit-Padmani/Book-Recommadation-System.git
cd book-recommendation-system
````


 
## 📁 Required Files and Folders  

- **Books.csv** → Contains book details.  
- **Ratings.csv** → Contains user ratings.  
- **Users.csv** → User details (for dataset reference).  
- **app.py** → Flask application entry point.  
- **books-recommandation-system.ipynb / news.ipynb** → Jupyter notebooks for model building & experimentation.  
- **.pkl files** → Precomputed models and data:  
  - `books.pkl` → Processed books data  
  - `popular.pkl` → Popularity-based recommendations  
  - `pt.pkl` → Pivot table matrix  
  - `similarity_scores.pkl` → Precomputed similarity scores  

- **templates/** (HTML templates for Flask UI):  
  - `index.html` → Home page (search or landing page)  
  - `recommend.html` → Displays recommended books  


## ▶️ Usage

Run the Flask app:

```bash
python app.py
```

Then open your browser at:

```
http://127.0.0.1:5000/
```

 

## 🛠️ Technologies Used

* **Programming Language**: Python
* **Data Handling**: Pandas, NumPy
* **Machine Learning**: Scikit-Learn, Cosine Similarity
* **Web Framework**: Flask
* **Visualization**: Matplotlib, Seaborn
* **Notebook Experiments**: Jupyter

 

## 📊 Example Recommendations

* If you like *Harry Potter and the Sorcerer’s Stone* → Get recommendations like *Percy Jackson* or *The Hobbit*.
* If you browse trending → See books like *The Da Vinci Code* or *The Alchemist*.

 

## 📦 Requirements

Dependencies are listed in `requirements.txt`:

```txt
Flask==2.3.2
pandas==2.0.3
numpy==1.24.3
scikit-learn==1.3.0
scipy==1.11.1
matplotlib==3.7.2
seaborn==0.12.2
joblib==1.3.1
notebook==7.0.2
```

Install them with:

```bash
pip install -r requirements.txt
```

 

## 📫 Contact

Developed by [Arpit Padmani](https://github.com/Arpit-Padmani)
💼 [LinkedIn](https://www.linkedin.com/in/arpitpadmani)

⭐ **Star this repo** if you found it useful!
=