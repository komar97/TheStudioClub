The Studio Club - Stock
=======================

Version simplifiee OneDrive.

Ce que fait l'application :
- stocke la base locale dans le fichier stock.db, a cote de app.py ;
- a chaque validation des mouvements, cree uniquement un fichier Excel dans OneDrive ;
- n'envoie pas de mail ;
- ne copie plus stock.db dans OneDrive.

Dossier OneDrive utilise :
C:\Users\MARKO\OneDrive\MARCO\TheStudioClub\Historique_Excel

Organisation automatique :
Historique_Excel\AAAA-MM\Stock_AAAA-MM-JJ_HH-MM-SS.xlsx

Contenu de chaque Excel :
1. Stock actuel : tous les articles du stock, pas seulement les alcools
2. Mouvements du jour : uniquement les mouvements valides au moment de la validation
3. Resume : totaux, personne, date, heure, nombre d'articles, stock faible

Installation :
1. Dezipper le dossier.
2. Installer les dependances :
   pip install -r requirements.txt
3. Lancer l'application :
   streamlit run app.py

Important :
Le chemin OneDrive est defini en haut du fichier app.py :
ONEDRIVE_REPORTS_DIR = Path(r"C:\Users\MARKO\OneDrive\MARCO\TheStudioClub") / "Historique_Excel"
