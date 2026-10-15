# USEReady AI/ML Internship Assignment 2
## Power System Load Type Prediction

### Objective
Predict `Load_Type` (`Light_Load`, `Medium_Load`, `Maximum_Load`) from historical electricity/power-system measurements.

### Dataset
Place `load_data.csv` in the same folder as `Load_Type_Prediction.ipynb`.

### Setup
Python 3.10 or 3.11 is recommended.

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
jupyter notebook
```

Open `Load_Type_Prediction.ipynb` and run all cells from top to bottom.

### Method
The notebook includes data inspection and cleaning, EDA, time-derived features, a chronological validation split, comparison against a majority baseline and multiple classifiers, selection using validation macro-F1, refitting on all pre-test data, and final evaluation on the last calendar month.

### Metrics
The final test evaluation reports accuracy, macro precision, macro recall, macro F1, a classification report, and a confusion matrix.

### Outputs
The notebook writes the following files to `outputs/`:
- `load_type_classifier.joblib`
- `test_predictions.csv`
- `test_metrics.csv`

### Important
The final month is reserved for testing as requested in the problem statement. Model scores are not included in advance; run the notebook on the provided data to generate the actual results.
