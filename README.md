# Swing Contract Pricing

Swing contract valuation project for energy markets using Monte Carlo simulation methods.

## Description

This project implements a pricing model for Swing options (flexibility contracts) commonly used in energy markets (gas, electricity). The model uses:

- **Spot price modeling**: mean-reverting process with jumps
- **Valuation method**: Monte Carlo simulation
- **Calibration**: on historical spot and futures price data

## Project Structure

```
SwingContractPricing/
├── main.ipynb          # Main notebook with implementation
├── requirements.txt    # Python dependencies
├── README.md
├── data/
│   ├── futures.xlsx    # Futures price data
│   └── spot_price_*.xlsx  # Historical spot prices (2016-2025)
└── doc/
    └── *.pdf           # Reference documentation and papers
```

## Installation

1. Clone the repository:
```bash
git clone <repo-url>
cd SwingContractPricing
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # macOS/Linux
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

Open and run the notebook `main.ipynb`:
```bash
jupyter notebook main.ipynb
```

## Dependencies

- pandas
- numpy
- matplotlib
- scipy
- scikit-learn
- openpyxl

## Data

The `data/` folder contains:
- **futures.xlsx**: futures price curve
- **spot_price_XX.xlsx**: historical spot prices by year (2016-2025)

## References

See the `doc/` folder for reference papers and documentation on:
- Mean-reverting spot price models with jumps
- Swing option valuation using Monte Carlo
