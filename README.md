
# mlops-ml-project — baseline ML reproductible

## Description
Ce projet MLOps permet d'entraîner et d'évaluer un modèle
de classification sur le dataset Iris.

## Installation
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

## Entraînement
```powershell
python scripts/train.py
```

## Évaluation
```powershell
python scripts/evaluate.py
```

## Tests
```powershell
python -m pytest -q
```

## Artefacts (générés dans artifacts/, non versionnés)
- model.joblib : pipeline entraîné
- metrics.json : accuracy et f1_macro sur le jeu de test
- confusion_matrix.png : matrice de confusion
- report.json : rapport de classification détaillé

## Configuration
Les paramètres sont définis dans config/train.yaml.
