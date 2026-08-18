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
Part I — Status (Alpha Research)
[x] Data loading + fixed two structural bugs (date format, holiday ghost rows)

[x] Built a superset of 18 features across different economic families

[x] Full pipeline: build_alpha → config search → evaluation → submission saving

[x] Fixed the evaluation logic to actually enforce the assignment's Sharpe/turnover requirements

[x] Verified ≥10 alphas meeting all requirements (Sharpe > 1.2, turnover < 0.8, correlation ≤ 0.5)

Full methodology, findings, and rationale for each feature are documented in overview.tex.

Part II — Status (Image Colorization)
[ ] Not started yet.

Running the Notebook
The notebook is built to run on Google Colab.
Ensure the data is placed in a data/ folder parallel to the code folder (see the first os.chdir cell in the notebook).
