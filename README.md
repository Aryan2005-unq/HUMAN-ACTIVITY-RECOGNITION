# Human Activity Recognition (HAR) System with CNN-LSTM

This project is a Human Activity Recognition (HAR) system that uses a deep learning model (CNN + LSTM) to predict human activities from sensor data. The system features an interactive Gradio web interface for predictions, exploratory data analysis (EDA), and batch processing.

## Features
- **Predict Activity:** Predicts human activity from sensor data using a trained CNN+LSTM model.
- **Prediction History:** Displays the last 10 predictions for easy tracking.
- **Batch Prediction:** Upload your own CSV file for batch activity prediction.
- **EDA Tabs:**
  - Activity distribution in the training set
  - Feature statistics
  - Confusion matrix
  - Per-class accuracy

## Requirements
- Python 3.7+
- gradio
- pandas
- numpy
- scikit-learn
- tensorflow
- matplotlib
- Pillow

Install dependencies with:
```bash
pip install -r requirements.txt
```

## Dataset
The code expects the following CSV files:
- `train_har.csv` (training data)
- `test.csv` (test data)

Update the paths in `HAR_system.py` if your data is located elsewhere.

## Usage
1. Ensure your datasets are available at the specified paths.
2. Install the required packages.
3. Run the application:
   ```bash
   python HAR_system.py
   ```
4. Access the Gradio interface in your browser (the URL will be shown in the terminal).

## File Structure
- `HAR_system.py` — Main application code
- `requirements.txt` — Python dependencies
- `readme.md` — Project documentation

## Example CSV Format
Your CSV files should have columns for all sensor features, plus `Activity` and `subject` columns. Example:

| feature1 | feature2 | ... | Activity | subject |
|----------|----------|-----|----------|---------|
| 0.12     | -0.34    | ... | Walking  | 1       |
| ...      | ...      | ... | ...      | ...     |

## License
This project is for educational and research purposes.
