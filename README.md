🏡 California Housing Price Predictor
A simple and interactive web application built with Streamlit that predicts housing prices in California based on various demographic and geographic features. Powered by a pre-trained regression model, this tool helps users estimate home values with just a few sliders.

🚀 Features
Predict housing prices in California using:
Median income
House age
Average number of rooms and bedrooms
Population
Occupancy rate
Geolocation (latitude and longitude)
Interactive user interface built with Streamlit
Real-time prediction updates
Simple and lightweight app—ideal for demos, educational purposes, or prototyping

📦 Project Structure
├── model.pkl               # Trained regression model (pickled)
├── app.py                  # Streamlit application code
├── requirements.txt        # Project dependencies
└── README.md               # Project documentation

⚙️ Setup Instructions
1. Clone the Repository
git clone https://github.com/your-username/california-housing-predictor.git
cd california-housing-predictor

2. Create Virtual Environment (Optional but Recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

4. Install Dependencies
pip install -r requirements.txt
If you don’t have a requirements.txt, you can create one manually:

streamlit
numpy
scikit-learn

4. Place the Model File
Make sure the regression_model.pkl (your trained model) is in the same directory as app.py.

▶️ Running the App
Launch the Streamlit app locally using:
streamlit run app.py

🔧 Configuration
You can customize the default values and ranges of the sliders directly in the app.py script:
# Example customization:
MedInc = st.slider("Median Income", 0.0, 150000.0, 50000.0)
If you'd like to modify the model or preprocessing, retrain your regression model and re-export it using pickle.

🤝 Contributing
Contributions are welcome! Feel free to submit pull requests or report issues.
