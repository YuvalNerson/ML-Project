# Applied Machine Learning: Final Project

Two applied machine learning tasks completed for the Applied Machine Learning course at Bar-Ilan University. The project covers cross sectional financial alpha research and image colorization.

## Part I: Cross Sectional Alpha Research

Built a feature and model search pipeline to rank stocks by expected next day return. The notebook engineers 21 time series and cross sectional features, evaluates 140 MLP/LSTM configurations on a chronological holdout, and saves the selected models with their feature lists.

The submitted package contains **16 selected alphas**. On the notebook's 2020–2023 holdout (894 dates), the reported results are:

Minimum Sharpe among selected alphas: **1.2589**. Maximum turnover: **0.6480**. Maximum pairwise PnL correlation: **0.4974**. Combined Sharpe: **3.4604**.

These are historical holdout results from the submitted notebook, not a guarantee of future performance. The data, the financial_toolkit.py file provided by the course, and other instructor materials are not included in this repository. See [Part I details](part1_financial_alpha/README.md) for setup notes and the submission artifacts.

## Part II: Image Colorization

Implemented a compact U Net that maps a 256 × 256 grayscale image to an RGB image. The notebook trains on a deterministic subset of 12,000 Caltech256 images, reserves 2,000 images for validation, and provides the required load_model() and colorize() inference functions. The saved state dictionary is included.

On the notebook's validation split, the final model reports L1 loss 0.048246, MSE 0.007795, and PSNR 21.082 dB. The grayscale baseline reports MSE 0.008974 and PSNR 20.470 dB. See [Part II details](part2_image_colorization/README.md).

## Repository Contents

Part I files: part1_financial_alpha/financial_alpha.ipynb and the 16 models plus params.json in part1_financial_alpha/submission/.

Part II files: part2_image_colorization/image_colorization.ipynb and the trained weights.pth.

The original course data is not committed. The financial CSV archives were supplied for the assignment; Caltech256 is downloaded by the colorization notebook when needed.
