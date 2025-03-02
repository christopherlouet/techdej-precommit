
# installation de pre-commit

```bash
pip install pre-commit
poetry : pyproject.toml
mise use pre-commit
```

# Configuration pre-commit

Initialisation du fichier .git/hooks/pre-commit

```bash
pre-commit install
```

Générer le fichier de configuration .pre-commit-config.yaml

```bash
pre-commit sample-config > .pre-commit-config.yaml
```

Exécuter le hook pre-commit

```bash
pre-commit run --all-files
```

Mettre à jour les repositories

```bash
pre-commit autoupdate 
```

# Fichier de configuration pre-commit

```bash
repos:
-   repo: https://github.com/pre-commit/pre-commit-hooks
    rev: v2.3.0
    hooks:
    -   id: check-yaml
    -   id: end-of-file-fixer
    -   id: trailing-whitespace
```
