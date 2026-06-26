THE STUDIO CLUB - STOCK

Installation locale :
1. Ouvrir un terminal dans ce dossier.
2. Installer les dependances : pip install -r requirements.txt
3. Lancer : streamlit run app.py

Sur Streamlit Cloud :
- Mettre app.py et requirements.txt sur GitHub.
- Le fichier stock.db est local a l'application Streamlit.
- Apres chaque validation de mouvements, un rapport Excel est genere.
- Le navigateur tente de le telecharger automatiquement.
- Si le telechargement automatique est bloque, cliquer sur le bouton : Telecharger le rapport Excel.

Acces :
- Onglet Stock : mot de passe 01234
- Onglet Admin : mot de passe 1234

Dernieres modifications :
- Ajout du mot de passe pour acceder a l'onglet Stock.
- Recherche article filtree sur les articles qui commencent par le texte saisi.
- Saisie possible des quantites directement dans les champs Sortie et Entree.
- Conservation des boutons + et - autour du champ de quantite.
- Suppression complete de la logique OneDrive.
