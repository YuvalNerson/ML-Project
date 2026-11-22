# Applied Machine Learning: Final Project

Two applied machine learning tasks completed for the Applied Machine Learning course at Bar Ilan University.

## Part I: Cross Sectional Alpha Research

Built 21 time series and cross sectional features and compared 140 MLP and LSTM configurations for next day stock return ranking. The submitted notebook reports 16 selected alphas on an 894 date holdout from 2020 to 2023.

Reported holdout metrics: minimum Sharpe 1.2589, maximum turnover 0.6480, maximum pairwise PnL correlation 0.4974, and combined Sharpe 3.4604. These historical results do not establish future performance.

## Part II: Image Colorization

Implemented an encoder and decoder network that maps a 256 × 256 grayscale image to an RGB image. Training used 12,000 Caltech256 images and validation used 2,000 images. The notebook provides load_model() and colorize() for inference.

Reported validation metrics: L1 loss 0.048246, MSE 0.007795, and PSNR 21.082 dB. The grayscale baseline reports MSE 0.008974 and PSNR 20.470 dB.

## Repository Status

This repository currently contains this project overview only. The submitted notebooks and trained model artifacts are prepared in a separate project bundle and have not been added here yet. The course financial data and its provided toolkit are also omitted.
