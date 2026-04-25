🚖Uber Fare Prediction using Machine Learning

📖 Overview

This project presents a Machine Learning-based web application that predicts Uber ride fares based on trip details such as pickup and drop-off locations, passenger count, and temporal features.

The application is deployed using **Streamlit**, providing an interactive interface for real-time predictions.



 🎯 Objectives

* Develop a regression model to estimate ride fares
* Integrate the model into a web-based interface
* Enable real-time user input and prediction
* Ensure input validation and accurate distance calculation

---
 🧠 Model Details

* **Type:** Regression Model
* **Library:** Scikit-learn
* **Serialized Model:** `model.pkl`
* **Training Notebook:** `model.ipynb`

📌 Input Features

* Pickup Longitude
* Pickup Latitude
* Dropoff Longitude
* Dropoff Latitude
* Passenger Count
* Distance (calculated using Haversine formula)
* Hour, Day, Month

---

📂 Project Structure

```bash id="a3l9h7"
├── app.py              # Streamlit application
├── model.pkl           # Trained ML model
├── model.ipynb         # Model training notebook
├── uber.csv            # Dataset
├── requirements.txt    # Dependencies
```

---
⚙️ Installation

 1. Clone the Repository

```bash id="6c3w5s"
git clone <repository-url>
cd <project-folder>
```

 2. Install Dependencies

```bash id="c2y8pz"
pip install -r requirements.txt
```

Dependencies include: pandas, numpy, scikit-learn, streamlit 

---

▶️ Running the Application

```bash id="j9k2rm"
streamlit run app.py
```

The application will be available at:

```
http://localhost:8501
```

---

🖥️ Application Workflow

1. User inputs trip details
2. System validates latitude and longitude ranges
3. Distance is calculated using the Haversine formula 
4. Features are passed to the trained model
5. Predicted fare is displayed

---

 📊 Output

* Distance between pickup and drop-off locations
* Estimated fare (₹)

---

 ⚠️ Validation Rules

* Latitude range: **-90 to 90**
* Longitude range: **-180 to 180**
* Pickup and drop locations must not be identical

---

🛠️ Technologies Used

* Python
* Streamlit
* NumPy
* Pandas
* Scikit-learn

---

 🌐 Deployment Options

* Streamlit Community Cloud
* Render
* Heroku

---

 📸 Screenshots

<img width="610" height="398" alt="image" src="https://github.com/user-attachments/assets/044d7dd5-457c-4b34-9591-15a11ad40298" />
<img width="574" height="351" alt="image" src="https://github.com/user-attachments/assets/34aa17c2-dcb5-4153-ab4a-fb785b1d0b1e" />



---

🚀 Future Enhancements

* Integration with map APIs for location selection
* Improved feature engineering for higher accuracy
* Visualization dashboard for fare trends

---

👩‍💻 Author

**Aditi Deshpande**

---

📄 License

This project is for educational purposes.

---

 ⭐ Acknowledgement

This project demonstrates the integration of Machine Learning with Streamlit to build an end-to-end predictive web application.
