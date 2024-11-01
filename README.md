Tracking stats and player performance through this spreadsheet. https://docs.google.com/spreadsheets/d/1j79Y-Pbl1Ta-MkRT-7R2-AS62iYtRgH5iEYHH7m5MuE/edit?userstoinvite=wockwarlockttv%40gmail.com&sharingaction=manageaccess&role=writer&gid=0#gid=0

Going to be making tournaments and in house games as well.

## Development Ideas
### Update Frequency
- Automatically updates at the end of each day
- Update Now Feature (run through command through discord)

### Stats
- Save all of the stats for the user 
    - Do not save puuid, summonerId, and other personal non-development data
- Grab 100 Games

### Storage
- Storage for everything through CSV but uploaded to Google Sheets
    - This keeps memory down when loading in csv data (C# pandas library)


### Commands/Interactions
- /playerLookup <username#tagline> [optionalStat]
    - Returns Overall Player Stats of All Champions

- /champLookup <username#tagline> <championName> [optionalStat]
    - Returns Overall Player Stats of the Selected Champions

- /matchUpLookup <username#tagline> <championName> <opponentName> [optionalStat]
    - Returns Overall player stats of the selected champion against the selected opponent (must be in same lane)

- /customResult <tournamentCode> [optionalStat]
    - Returns data on the result of the scrim/tournament game result

- /feedback <message> 
    - Sends a message to developers about any feedback with the bot


### Blockers
- API Key with a high enough rate limit so that I can get the games that I need (production and verified level key)
- Memory usage needs to be low enough so that the program doesn't crash (hopefully under 1gb limit)
- Storage usage needs to be low enough so that compute engine doesn't run out of space (really shouldn't be an issue)
