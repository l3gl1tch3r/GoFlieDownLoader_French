# GoFlieDownLoader_French
📥 GoFileDownloader

GoFileDownloader est un outil Python permettant de télécharger facilement des fichiers ou albums depuis GoFile.io
.

Il prend en charge :

Les albums simples

Les albums protégés par mot de passe

Le téléchargement en lot (batch)

La personnalisation du dossier de destination

Le suivi visuel de la progression grâce à la librairie rich

🗂 Structure du projet
/src/
  config.py
  download_utils.py
  file_utils.py
  general_utils.py
  gofile_utils.py
  /managers/
    live_manager.py
    log_manager.py
    progress_manager.py
    __init__.py
  __init__.py
downloader.py
main.py
requirements.txt
CONTRIBUTING.md
LICENSE
/assets/
  demo.gif
  logo-small-70.png

🚀 Installation

Télécharger le projet

Avec Git :

git clone https://github.com/l3gl1tch3r/GoFileDownloader.git
cd GoFileDownloader


Ou télécharger le ZIP depuis GitHub et décompresser.

Installer Python 3.9+
Vérifie l’installation :

python --version


Installer les dépendances

python -m pip install -r requirements.txt

📂 Utilisation
1. Télécharger un album unique
python downloader.py <lien_go_file>

2. Télécharger un album protégé par mot de passe
python downloader.py <lien_go_file> <mot_de_passe>

3. Télécharger plusieurs liens à la suite (batch)

Crée un fichier URLs.txt à la racine du projet, un lien GoFile par ligne :

https://gofile.io/d/abc123
https://gofile.io/d/def456
https://gofile.io/d/ghi789


Lance le script principal :

python main.py

4. Choisir un dossier de destination

Par défaut, les fichiers sont enregistrés dans Downloads.
Pour changer le dossier :

python main.py --custom-path "C:/MonDossier"

📝 Journal (Logs)

Le script crée un fichier session_log.txt contenant :

les téléchargements réussis

les erreurs rencontrées (liens invalides, mot de passe manquant, etc.)

⚠️ Remarques importantes

Utilise cet outil uniquement pour des fichiers que tu es autorisé à télécharger

Si GoFile modifie son site ou son API, le script peut nécessiter une mise à jour

Les albums volumineux peuvent prendre un certain temps à se télécharger
