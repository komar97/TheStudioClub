The Studio Club - version avec base persistante

Cette version garde SQLite en local pour les tests, mais utilise PostgreSQL/Supabase si DATABASE_URL est defini.

Installation recommandee avec Supabase:
1. Creer un projet Supabase dedie a The Studio Club, ou reutiliser le meme projet avec des tables separees / un schema separe.
2. Recuperer l'URL de connexion PostgreSQL, format SQLAlchemy:
   postgresql+psycopg2://USER:PASSWORD@HOST:5432/postgres
3. Dans Streamlit Cloud, ajouter dans Secrets:
   DATABASE_URL = "postgresql+psycopg2://USER:PASSWORD@HOST:5432/postgres"
4. Deployer l'app. Les tables articles et mouvements seront creees automatiquement.

Conseil : pour eviter de melanger les stocks Jukeboxx et The Studio Club, le plus simple est de creer un nouveau projet Supabase pour The Studio Club.

Test local sans Supabase:
- streamlit run app.py
- L'app utilisera stock.db localement.

Notes:
- Ne pas mettre DATABASE_URL dans GitHub en dur.
- Le fichier stock.db reste utile seulement pour le developpement local.
