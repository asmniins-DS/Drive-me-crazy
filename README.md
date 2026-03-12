# Welcome to Drive Me Crazy
 ***

## Task

I set out to tackle the problem of predicting traffic flow across multiple datasets, including PeMS04, PeMS07, PeMS08 and NYC Taxi. The challenge is two‑fold: handling multivariate time series data from different sources, and providing a baseline so that a more advanced model (PDFormer) can be benchmarked against a traditional LSTM.

## Description

I solved the problem by implementing a self‑contained pipeline in Jupyter notebooks. The notebooks load and preprocess raw data, convert it into sliding windows, normalize by training statistics, and then train a vanilla LSTM model on each dataset. The results are evaluated using MAE, RMSE and MAPE, and visualized to compare predictions with ground truth.

## Installation

The project is lightweight and relies on standard Python libraries. To set it up I installed the dependencies via pip. From the workspace root I run the following once:

```bash
pip install numpy pandas matplotlib torch scikit-learn
```

Everything else is contained within the notebooks; there is no build system or additional compilation step.

## Usage

To use the project I open one of the provided notebooks (`drive_me_crazy_pdformer.ipynb` or `drive_me_crazy_tradi.ipynb`) in Jupyter. The notebooks are executable end‑to‑end: I run each cell sequentially and they load the datasets, train the LSTM models, save checkpoints and plots, and output a CSV summary of results. For a quick check I can re‑execute the prediction visualization cell to see model outputs for any dataset.

Feel free to adapt hyperparameters or replace the model with a different architecture as needed.

```
```

### The Core Team

Abubakar Sadik Nasir

<span><i>Made at <a href='https://qwasar.io'>Qwasar SV -- Software Engineering School</a></i></span>
<span><img alt='Qwasar SV -- Software Engineering School's Logo' src='https://storage.googleapis.com/qwasar-public/qwasar-logo_50x50.png' width='20px' /></span>
