# GoFlieDownLoader_French
📥 GoFileDownloader

GoFileDownloader est un outil en Python permettant de télécharger facilement des fichiers ou des albums depuis GoFile.io
.
Il supporte :

les albums simples,

les albums protégés par mot de passe,

le téléchargement en lot (plusieurs liens à la fois),

la personnalisation du dossier de destination,

et un suivi visuel de la progression grâce à la librairie rich.

🚀 Installation

Télécharger le projet

Via Git :

git clone https://github.com/l3gl1tch3r/GoFileDownloader.git
cd GoFileDownloader


Ou bien, télécharge le ZIP depuis GitHub, puis décompresse-le.

Installer Python 3.9+
Vérifie l’installation :

python --version


Installer les dépendances
Dans le dossier du projet, lance :

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


Lance la commande :

python main.py

4. Choisir un dossier de destination

Par défaut, les fichiers sont enregistrés dans Downloads.
Pour changer le dossier :

python main.py --custom-path "C:/MonDossier"

📝 Journal (Logs)

Le script génère un fichier session_log.txt qui contient :

les téléchargements réussis,

les erreurs rencontrées (liens invalides, mot de passe manquant, etc.).

⚠️ Remarques importantes

Utilise uniquement cet outil pour des fichiers que tu es autorisé à télécharger.

Si GoFile modifie son site ou son API, le script peut nécessiter une mise à jour.

Les albums volumineux peuvent prendre un certain temps à se télécharger.
