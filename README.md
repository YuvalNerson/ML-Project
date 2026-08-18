# Final Project — Applied Machine Learning

Final assignment for the Applied Machine Learning course, Bar-Ilan University. The project consists of two separate parts:

* **Part I — Cross-Sectional Alpha Research:** Building a daily long/short book based on stock return predictions.
* **Part II — Image Colorization:** Training a model that turns a grayscale image into a color image.

## Repo Structure

```text
.
├── README.md
├── overview.tex                   # Methodology summary document (LaTeX, Overleaf)
├── part1_alpha_research/
│   ├── financial_template.ipynb   # The full notebook
│   ├── financial_toolkit.py       # Base framework (FIXED, not edited)
│   ├── directives.txt             # Original assignment instructions
│   └── output/
│       └── params.json            # Saved alphas + their feature subsets
│                                  # (model_<i>.pt files are not included — see .gitignore)
├── part2_colorization/
│   └── (in progress)
└── data/                          # Not included in the repo — large CSV files, see .gitignore
