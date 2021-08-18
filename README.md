# Anime Central

How to run:

1. Install PostgresSQL on your computer(via Homebrew or directly from website)

2. Create a database in Postgres that you would like to dump the anime data into. Call it something like "animeCentral" or whatever you'd like.

3. After cloning this repository, cd into "webapp" and run the following command: "psql -U yourUsername yourDatabaseName < data.sql". "yourUsername" is your Postgres username and "yourDatabaseName" is the name of the Postgres database that you just created.

4. Create a file called "config.py" within "webapp" as follows:
    
    user = "yourUsername"
    password = "yourPassword"
    database = "yourDatabaseName"
    
5. Run the following command: python3 app.py localhost 5000. Then, go to http://localhost:5000 to see the website!

_______________________________________________________________________________

AUTHORS: Kevin Chen(kchen01), James Marlin(jamesmarlin), Quoc Nguyen(quocodile)

DATA: A dataset consisting of animes that contains the anime's rating, name, # of episodes, etc

Copyright info: CC0: Public Domain
Link for DATA: https://www.kaggle.com/CooperUnion/anime-recommendations-database?select=anime.csv


Features:
- Search anime by title or genre.
- Write a review for an anime.
- Add/remove anime from watchlist
- Signup/Login
- Browse various anime by genre on home page.
- Help page
