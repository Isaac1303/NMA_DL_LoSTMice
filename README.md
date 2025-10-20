# Neural Decoding of Mouse Decisions using LSTM (Neuromatch 2025)

This project explores whether neural activity in the Steinmetz 2019 dataset contains decodable information about a mouse's left vs right decisions during a visual decision-making task. We implement deep learning models to decode behavior from cortical activity.

## Dataset
Steinmetz et al. (2019) — large-scale Neuropixels recordings during a two-alternative unforced choice task.

## Model
We implemented a three-headed LSTM architecture in PyTorch:
- Head 1: Go-Cue aligned neural activity
- Head 2: Movement aligned neural activity
- Head 3: Feedback aligned neural activity  
Final hidden state → classifier → left/right prediction

## Current Results
Both classical models (logistic regression, random forest) and LSTM models performed near chance accuracy, suggesting the dataset segment used may not contain discriminative choice-related information.

## Technologies Used
- PyTorch
- NumPy / Pandas
- scikit-learn
- Matplotlib / Seaborn

## Large Data File
Due to GitHub size limits, one of the preprocessed data files (~300MB, .pkl) used as input to the model is stored externally.

Download link:
https://drive.google.com/file/d/1lr2oy19n4KiirtvtXd96DAF0t0_EWM63/view?usp=sharing

## Collaborators
Abu Mohammed - Heriot Watt University 
Isaac Thu - University of Washington Seattle
Keming Liu - Wesleyan University
Iyad Ba Gari - Univeristy of Southern California

## Status
Project completed as part of Neuromatch — no further development planned.
