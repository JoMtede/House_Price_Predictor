#  House Price Prediction App

An end-to-end machine learning web application that predicts residential property values based on key structural features.
This project leverages an optimized ensemble model and is deployed as an interactive user interface for real-time predictions.
## Features
 **Interactive UI**: Users can adjust inputs via sliders and numerical fields to predict housing prices instantly.
 **Optimized Model**: Uses an ensemble learning algorithm fine-tuned via exhaustive search techniques.
 **Real-Time Inference**: Connects a localized Python backend directly to a cloud-based web interface.
 ##  Tech Stack
 **Frontend**: Streamlit
 **Machine Learning**: Python, Scikit-Learn, NumPy
 **Model Optimization**: GridSearchCV
 **Deployment**: Streamlit Community Cloud
 ## Dataset & Features
The model learns from historical housing data using the following input attributes:
1. **Number of Bedrooms** (e.g., 3)
2. **Number of Bathrooms** (e.g., 1)
3. **Living Area** (Square footage, e.g., 2000)
4. **Condition** (Overall property rating, e.g., 3)
5. **Number of Schools Nearby** (e.g., 1)
   ##  Model Performance & Tuning
Initially, a single Decision Tree Regressor was tested,followed by Linear Regression but resulted in a high evaluation error. 
To improve accuracy, the model was upgraded to a **Random Forest Regressor**. 
Using `GridSearchCV`, we systematically tuned critical hyperparameters including tree depth and
splitting criteria over 5-fold cross-validation to isolate the most robust structural settings.
##  How to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com
   cd YOUR_REPOSITORY_NAME
   ```
2. Install the required dependencies:
   ```bash
   pip3 install -r requirements.txt
   ```
3. Launch the Streamlit application:
   ```bash
   python3 -m streamlit run app.py
   ```
