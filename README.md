# Systeme de gestion de l'apprentissage basé python et son framework célèbre django

## Créér par  [ndongomodounar@gmail.com](https://adilmohak1.pythonanywhere.com/)

### Access credentials:
  - username: **user**
  - password: **user**


Riche en fonctionalités de gestion des établissements d'enseignements



## Current features

- Tableau de bord : Démographie et analyses de l'école. Accès restreint uniquement aux administrateurs.
- Actualités et événements : Tous les utilisateurs peuvent accéder à cette page.
- L'administrateur gère les étudiants (Ajouter, Mettre à jour, Supprimer).
- L'administrateur gère les enseignants (Ajouter, Mettre à jour, Supprimer).
- Les étudiants peuvent ajouter et retirer des cours.
- Les enseignants soumettent les notes des étudiants : Présence, Examen de mi-semestre, Examen final, Devoirs.
- Le système calcule automatiquement le total, la moyenne, les points et les notes des étudiants.
- Commentaire sur la note pour chaque étudiant avec une mention réussi, échoué ou réussi avec avertissement.
- Page des résultats d'évaluation pour les étudiants.
- Page des résultats de notes pour les étudiants.
- Gestion des sessions/années et des semestres.
- Les évaluations et les notes seront regroupées par semestre.
- Téléchargement de vidéos et de documents pour chaque cours.
- Générateur PDF pour le reçu d'inscription des étudiants et le relevé de notes.
- Restriction d'accès aux pages.
- Stockage des résultats de quiz sous chaque utilisateur.
- Randomisation de l'ordre des questions.
- Les scores des précédents quiz peuvent être consultés sur la page de catégorie.
- Les bonnes réponses peuvent être affichées après chaque question ou toutes à la fin.
- Les utilisateurs connectés peuvent reprendre un quiz incomplet pour le terminer, et les utilisateurs non connectés peuvent terminer un quiz si leur session est toujours active.
- Le quiz peut être limité à une seule tentative par utilisateur.
- Les questions peuvent être classées par catégorie.
- Le taux de réussite pour chaque catégorie peut être suivi sur une page de progression.
- Une explication peut être donnée pour chaque résultat de question.
- Les notes de passage peuvent être définies.
- Type de question à choix multiple.
- Type de question vrai/faux.
- Type de question dissertation.
- Message personnalisé affiché pour ceux qui réussissent ou échouent à un quiz.
- Permission personnalisée (view_sittings) ajoutée, permettant aux utilisateurs ayant cette permission de voir les résultats des quiz des utilisateurs.
- Une page de notation qui liste les quiz terminés, peut être filtrée par quiz ou utilisateur, et est utilisée pour noter les questions à dissertation.


# Requirements:

> The following programs are required to run the project

- [Python3.8+](https://www.python.org/downloads/)
- [Redis](https://redis.io/docs/latest/operate/oss_and_stack/install/install-redis/)

# Installation

- Cloner le repositorie

```bash
git clone https://github.com/nourou-ndongo/learning management system.git
```

- Créé et activé un environnement viruel 

```bash
pip install -r requirements.txt
```

- Create `.env` file inside the root directory

- copier et coller tout ce qui est dans le fichier `.env.example` dans le fichier `.env`. Et ne pas oublier de changer les variables personnelles

```bash
python manage.py migrate
```

```bash
python manage.py createsuperuser
```

```bash
python manage.py runserver
```

Make sure your Redis server is running

```bash
redis-server
```

Start the celery worker

```bash
celery -A config.celery worker -l INFO
```




#### Show your support by ⭐️ this project!
