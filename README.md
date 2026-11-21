# Predicting athlete fatigue

Machine Learning project, Centrale Lyon, 2026. Nael El Dajani, Elliot Aimard Gaillot, Chloé Savy.

We predict the fatigue index (`fatigue_index`, from 15 to 270) of a football or basketball player at the end of a training session, from the measurements of that session. Sessions are split at random: 60% train, 20% validation, 20% test.

We compare a decision tree, a random forest, a linear regression and a Lasso. Final model: **Lasso**, R2 = 0.69 and RMSE = 14.0 on the test set, with no overfitting. Training load is by far the main driver of fatigue.

## Files

- `data/multimodal_sports_injury_dataset_kaggle.csv`: the data (Kaggle)
- `fatigue.ipynb`: the whole project (data, preprocessing, models, results, demo)
- `README.md`: this file

## Run

```sh
uv sync
uv run jupyter notebook fatigue.ipynb   # run all the cells, the demo opens in the last one
```
