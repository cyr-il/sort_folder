# Tri automatique de fichiers dans un dossier

Ce script Python permet de trier automatiquement les fichiers d'un dossier selon leur extension, en les déplaçant dans des sous-dossiers thématiques (Images, Documents, Musique, etc.) et par date de modification. Accompagné du fichier .reg, il permet d'ajouter une option de tri dans le menu contextuel de l'explorateur Windows (clic droit sur un dossier).

## Fonctionnalités

- Classement des fichiers par type (Images, Documents, Musique, Vidéos, etc.)
- Création automatique des dossiers nécessaires
- Organisation par mois et année de modification
- Gestion des fichiers inconnus dans un dossier "Autres"
- Affichage d'un résumé du tri avec statistiques
- Utilisation d'emojis pour une meilleure lisibilité
- Barre de progression grâce à `tqdm`
- Couleurs dans le terminal grâce à `colorama`

## Prérequis

- Python 3.x
- Modules : `colorama`, `tqdm`

Installez les dépendances avec :
```powershell
pip install colorama tqdm
```

## Utilisation

Soit vous placez le script n'importe où sur votre pc et vous lancez le .reg en double-cliquant dessus pour ajouter l'option de tri dans le menu contextuel de l'explorateur Windows, soit vous utilisez le script directement. Pour cela, placez le script dans le dossier à trier et lancez-le avec Python ou indiquez le chemin du dossier en argument :

```powershell
python sort_folder.py "chemin/vers/le/dossier"
```

Si aucun argument n'est donné, le script trie le dossier où il se trouve.

## Exemple

Après exécution, les fichiers seront déplacés dans des sous-dossiers comme :
```
Images/
    07-2025/
        photo.png
Documents/
    06-2024/
        rapport.pdf
Autres/
    bak/
        archive.bak
```

## Auteur

Script réalisé par Cyril