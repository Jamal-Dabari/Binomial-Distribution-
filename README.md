# Beta-Binomial Distribution Analysis

## 📊 Overview

This project explores the differences between Beta-binomial and standard Binomial distributions through simulation and statistical analysis. The main focus is understanding over-dispersion - a phenomenon where data shows more variability than what a simple Binomial model would predict.

## 🎯 What This Code Does

The analysis generates random samples from both distributions and compares their statistical properties:

- **Beta-binomial simulation**: Models scenarios where the probability of success varies between trials (following a Beta distribution)
- **Binomial simulation**: Models scenarios with a fixed probability of success
- **Variance comparison**: Demonstrates how Beta-binomial data exhibits greater variance than traditional Binomial data

## ⚙️ Key Parameters

| Parameter | Value | Description |
|-----------|--------|-------------|
| Trials per experiment | 30 | Number of trials in each simulation |
| Alpha (α) | 2 | Beta distribution shape parameter |
| Beta (β) | 3 | Beta distribution shape parameter |
| Sample size | 10,000 | Total number of simulations |
| Mean probability | 0.4 | Derived from Beta parameters (α/(α+β)) |

## 📈 Expected Results

The simulation typically shows:
- Both distributions have similar means (~12)
- Beta-binomial variance is significantly higher (~43) compared to Binomial variance (~7)
- Over-dispersion factor of approximately 6x

## 🚀 Getting Started

### Prerequisites
```bash
pip install numpy scipy
```

### Running the Analysis
1. Open `Project2.ipynb` in Jupyter Notebook or Google Colab
2. Run all cells to see the simulation results
3. Each run will produce slightly different values due to randomization

## 💡 Why This Matters

This analysis is relevant for:
- **Quality control**: When success rates vary between batches or conditions
- **Clinical trials**: Where patient response rates may differ across subgroups
- **Marketing analytics**: When conversion rates fluctuate over time
- **Risk modeling**: When event probabilities aren't constant over time

## 📝 Technical Notes

The Beta-binomial distribution is particularly useful when you suspect that your "probability of success" isn't actually constant across all trials. This creates what statisticians call "over-dispersion" - more spread in your data than a simple Binomial model would predict.

Understanding this distinction helps in:
- Choosing the right statistical model for your data
- Avoiding incorrect assumptions about variability
- Better quantifying uncertainty in your results

## 📁 File Structure
```
├── Project2.ipynb          # Main analysis notebook
└── README.md              # This file
```

## 🤝 Contributing

Feel free to fork this project and submit pull requests for improvements or additional analyses!

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
