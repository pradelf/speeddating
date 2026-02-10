# Installation rapide

## 1. Prérequis

- Python 3.10 ou plus récent
- avoir virtuelenv d'installer sur sa machine.
- `pip` à jour
- (Optionnel) `git` si vous clonez le dépôt
- Environ 200 Mo d’espace libre pour l’environnement virtuel et les données

## 2. Récupérer le projet

Si vous partez de GitHub :

```
git clone https://github.com/pradelf/speeddating.git
cd speeddating
```

Sinon, placez-vous simplement dans le dossier du projet (celui qui contient `README.md`).

## 3. Charger l'environnement virtuel

```
# macOS / Linux
source .venv/bin/activate
```

## 4. Vérifier / placer les données

Les jeux de données doivent rester dans `Data/` :

- `Speed+Dating+Data.csv`
- `speed_dating_cleaned.csv`
- `Speed+Dating+Data+Key.doc` (dictionnaire de variables)

## 5. Ouvrir le notebook

Activez l’environnement virtuel puis lancez :

```
jupyter notebook 01-Speed_Dating_FPr.ipynb
```

Ou avec JupyterLab :

```
jupyter lab 01-Speed_Dating_FPr.ipynb
```

## 6. (Optionnel) Exporter le notebook en HTML

```
jupyter nbconvert --to html 01-Speed_Dating_FPr.ipynb
```

Vous êtes prêt : exécutez les cellules dans l’ordre pour reproduire l’analyse.
