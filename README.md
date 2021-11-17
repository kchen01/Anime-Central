# Anime Central

## Homepage:
<img width="1440" alt="Screen Shot 2021-11-16 at 7 30 12 PM" src="https://user-images.githubusercontent.com/52056529/142127763-79662570-f597-4ef3-b8fe-e269a47b1eec.png">

## Search result example:
<img width="1440" alt="Screen Shot 2021-11-16 at 7 31 02 PM" src="https://user-images.githubusercontent.com/52056529/142127811-8f374150-4b69-4af9-8748-1f7919721d88.png">

## Individual anime page example
<img width="1440" alt="Screen Shot 2021-11-16 at 7 31 47 PM" src="https://user-images.githubusercontent.com/52056529/142127823-3cff87e8-c628-4b0b-9086-43c24de9ae96.png">

## User watchlist example
<img width="1440" alt="Screen Shot 2021-11-16 at 7 32 09 PM" src="https://user-images.githubusercontent.com/52056529/142127864-03bf4914-67d6-40c0-9906-ad0103b06bfe.png">


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
