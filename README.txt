The Studio Club - Application de stock

Installation locale :
1. Installer Python
2. Ouvrir un terminal dans ce dossier
3. Lancer : pip install -r requirements.txt
4. Lancer : streamlit run app.py

Fonctionnement :
- Onglet Stock protege par mot de passe : 01234
- Onglet Admin protege par mot de passe : 1234
- Recherche instantanee par debut de nom d'article
- Sorties et entrees saisissables avec boutons -/+ ou au clavier
- A chaque validation, un rapport Excel est prepare au telechargement
- Nom du fichier : The_Studio_Club_Stock_YYYY-MM-DD_HH-MM-SS.xlsx

Important Streamlit Cloud :
La base stock.db locale n'est pas un stockage permanent garanti. Pense a utiliser Supabase/PostgreSQL pour garder les donnees en production.
