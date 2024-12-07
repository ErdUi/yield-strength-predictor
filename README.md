# Yield Strength Predictor

A machine learning application that predicts the yield strength of materials with 99.9% confidence intervals. This application uses Random Forest regression with enhanced feature engineering to provide accurate predictions based on material properties.

## Features

- User-friendly GUI interface
- Load and process training data from CSV files
- Advanced feature engineering
- Random Forest model with optimized hyperparameters
- 99.9% confidence interval predictions
- Save and load trained models
- Standalone executable distribution

## Installation

### For Users
Download the latest release from the [Releases](../../releases) page and run the standalone executable.

### For Developers
1. Clone the repository:
```bash
git clone https://github.com/ErdUi/yield-strength-predictor.git
cd yield-strength-predictor
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

### Running the Application
```bash
python src/main.py
```

### Building the Executable
```bash
python build.py
```

The executable will be created in the `dist` folder.

### Training Data Format
The application expects a CSV file with the following columns:
- QC_Re
- QC_Rm
- QC_A
- Manufacturer
- Dimension
- Yield Strength [Mpa]

Use semicolon (;) as the delimiter.

## Project Structure
```
yield-strength-predictor/
├── src/
│   ├── main.py                 # Main application code
│   ├── icon.ico               # Application icon
│   └── default_model.pkl      # Pre-trained model (optional)
├── tests/                     # Test files
├── examples/                  # Example data files
├── requirements.txt           # Dependencies
├── build.py                  # Build script
└── README.md                 # This file
```

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Built with scikit-learn, pandas, and tkinter
- Random Forest implementation based on scikit-learn's ensemble methods