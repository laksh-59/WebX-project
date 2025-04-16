# Iris Flower Oracle 🌸

A machine learning application that predicts iris flower species based on measurements.

## Project Overview

Iris Flower Oracle is an educational tool that demonstrates the practical application of machine learning for botanical classification. The application consists of:

- A React frontend built with TypeScript, Tailwind CSS, and shadcn/ui
- A Flask backend with a trained machine learning model

## Features

- 🌱 Predict iris species (Setosa, Versicolor, or Virginica) based on measurements
- 📊 Interactive dataset visualization
- 📱 Responsive design for all devices
- ⚡ Local prediction fallback when the backend is unavailable

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- Python 3.8 or higher
- pip (Python package manager)

### Frontend Setup

1. Clone this repository
2. Navigate to the frontend directory:
   ```
   cd frontend
   ```
3. Install dependencies:
   ```
   npm install
   ```
4. Start the development server:
   ```
   npm run dev
   ```
5. Open your browser and visit: `http://localhost:8080`

### Backend Setup

1. Navigate to the flask-backend directory:
   ```
   cd flask-backend
   ```
2. Create a virtual environment (optional but recommended):
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
4. Start the Flask server:
   ```
   python app.py
   ```
5. The API will be available at: `http://localhost:5000`

## Project Structure

```
iris-flower-oracle/
├── frontend/               # React frontend application
│   ├── public/             # Static assets
│   ├── src/                # Source files
│   │   ├── components/     # UI components
│   │   ├── hooks/          # Custom React hooks
│   │   ├── pages/          # Application pages
│   │   ├── utils/          # Utility functions
│   │   └── types/          # TypeScript types
│   └── package.json        # Frontend dependencies
│
├── flask-backend/          # Flask backend application
│   ├── app.py              # Main Flask application
│   ├── model/              # ML model files
│   │   ├── iris_model.py   # Model training and prediction
│   │   └── iris_model.pkl  # Saved trained model
│   └── requirements.txt    # Backend dependencies
│
└── README.md               # Project documentation
```

## Tech Stack

### Frontend
- React with TypeScript
- Tailwind CSS for styling
- shadcn/ui component library
- React Router for navigation
- Vite for fast development

### Backend
- Flask Python web framework
- scikit-learn for machine learning
- pandas for data processing
- Flask-CORS for cross-origin requests

## Troubleshooting

**Backend Connection Issues**
- Ensure Flask server is running at http://localhost:5000
- Check for CORS configuration issues
- The frontend includes a fallback prediction when the backend is unavailable

**Model Prediction Errors**
- Verify that input measurements are valid numbers
- Check console logs for detailed error information

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- The Iris dataset from UC Irvine Machine Learning Repository
- Original dataset by R.A. Fisher
