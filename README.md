# Plant Disease Classifier

This project is a web application that allows users to upload an image of a plant leaf, and it will predict the disease affecting the plant based on the image. The model is trained using TensorFlow and Keras and is deployed using Streamlit.

## Features

- Upload an image of a plant leaf in `.jpg`, `.jpeg`, or `.png` format.
- The model classifies the image and predicts the disease affecting the plant.
- Simple and intuitive web interface using Streamlit.

## How It Works

1. The user uploads an image of a plant leaf.
2. The image is preprocessed (resized, normalized) and passed to a pre-trained TensorFlow model.
3. The model predicts the class (disease) of the plant based on the uploaded image.
4. The prediction result is displayed on the web interface.

## Project Structure

```bash
plant-disease-classifier/
│
├── trained_model/
│   └── plant_disease_prediction_model.h5  # Pre-trained model
├── class_indices.json                     # Mapping of class indices to disease names
├── app.py                                 # Main application file
└── README.md                              # Project documentation
```
## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/plant-disease-classifier.git
   cd plant-disease-classifier
   ```
2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```
5. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```
## Usage
- Open your browser and go to http://localhost:8501.
- Upload an image of a plant leaf.
- Click on the "Classify" button to see the prediction.

## Model Information
- The model used in this project is a pre-trained TensorFlow model (plant_disease_prediction_model.h5).
- The model was trained on a dataset of plant leaf images labeled with different diseases.
