<div align="center">

# 🚗 Car Price Predictor

### Estimate a used car’s price with a machine learning model

[![Open App](https://img.shields.io/badge/🚀%20Try%20the%20App-Streamlit-FF4B4B?style=for-the-badge)](https://car-price-predictor-bzyu8andogdeoraoq2dtfi.streamlit.app/)
[![Built with Python](https://img.shields.io/badge/Python-3B82F6?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Built with Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white)](https://streamlit.io/)
[![Machine Learning](https://img.shields.io/badge/Machine%20Learning-scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)

</div>

---

## ✨ About

This project predicts the estimated price of a used car based on its **model, company, year, fuel type, and kilometers driven**.

It combines a machine learning pipeline built with **scikit-learn** and a simple interactive web app made with **Streamlit**.

<div align="center">

### 👉 [Launch the Car Price Predictor](https://car-price-predictor-bzyu8andogdeoraoq2dtfi.streamlit.app/)

</div>

---

## 🛠️ How to use

1. Select a **company**.
2. Choose a car name from the filtered list.
3. Enter the car’s **year** and **kilometers driven**.
4. Select the **fuel type**.
5. Click **Estimate car price** to see the prediction in rupees.

---

## 🧠 How it works

The model was developed in a Jupyter notebook using used-car listing data.

- Cleaned the data by removing invalid years, prices, and mileage values.
- Kept the first three words of each car name to create the model-name feature.
- Encoded car name, company, and fuel type using one-hot encoding.
- Trained a Linear Regression model inside a scikit-learn pipeline.
- Saved the trained pipeline and loaded it in the Streamlit app.

The app gathers the selected details, passes them to the saved pipeline, and displays the estimated price.

---

## 🧰 Built with

| Tool | Purpose |
|---|---|
| Python | App and model programming |
| pandas and NumPy | Data handling |
| scikit-learn | Preprocessing and Linear Regression model |
| Streamlit | Interactive web app |
| Jupyter Notebook | Model development |

---

## 💻 Run locally

```bash
# Clone the repository
git clone https://github.com/parvchaudhari/Car-Price-Predictor.git
cd Car-Price-Predictor

# Install dependencies
pip install -r requirements.txt

# Start the app
streamlit run App.py
