# UBI Impact Detection

This project explores whether macroeconomic indicators can be used to detect patterns associated with Universal Basic Income (UBI) implementation. By analyzing global economic data from countries like Finland, Kenya, and the United States, the goal is to build a machine learning model that identifies regions exhibiting UBI-like economic behavior.

## 📌 Project Motivation

The rise of UBI as a potential tool to reduce poverty, respond to automation, and promote economic security has sparked global interest. However, there's limited infrastructure for detecting where UBI-like interventions may already be producing change — especially in countries without formal trials. This project aims to bridge that gap using classification models and open economic data.

## 🧠 Methods

- **Data Sources**: World Bank macroeconomic indicators — poverty rates, unemployment, government transfers
- **Preprocessing**: Rolling averages, year-over-year change, volatility indicators
- **Models**: Decision Tree, Random Forest, K-Nearest Neighbors
- **Evaluation**: Accuracy, cross-validation, feature importance

## 📁 Project Structure

```
ubi_impact/
├── data/                 # Raw and processed datasets
│   ├── raw/              # Uploaded CSVs from World Bank
├── notebooks/            # Exploratory and modeling notebooks
│   └── 01_modeling_and_analysis.ipynb
├── reports/              # Any figures or visual outputs
├── src/                  # Placeholder for modular Python code
├── requirements.txt      # Python dependencies
├── .gitignore            # Git exclusions
└── README.md             # This file
```

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ubi_impact.git
   cd ubi_impact
   ```

2. Create a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate  # or venv\Scripts\activate on Windows
   pip install -r requirements.txt
   ```

3. Open the notebook:
   ```bash
   jupyter notebook notebooks/01_modeling_and_analysis.ipynb
   ```

## 🔄 Running the Pipeline

The full data processing and model training pipeline is contained in `notebooks/01_modeling_and_analysis.ipynb`.

1. Open the notebook.
2. Run all cells in order to:
   - Load and clean data
   - Engineer features
   - Train classification models
   - Evaluate performance and display results

## 📊 Model Evaluation

Model performance is evaluated using:
- Accuracy score
- Cross-validation accuracy
- Feature importance (Random Forest)

These metrics are printed and visualized in the final notebook cells.

## ♻️ Reproducibility Notes

- All random seeds are set using `random_state=42` in model training steps.
- Input data files are located in `data/raw/` and loaded directly in the notebook.
- Ensure notebook is run top-to-bottom without skipping cells.

## 📚 References

A full list of data sources and citations can be found in the report document.
