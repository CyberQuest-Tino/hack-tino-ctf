# CupertinoHacks CTF

- made in like 6 hours...please be lenient with poor coding practices ❤️

- each repository contains readme's and content regarding the individual subrepo, but shared links are here:
  - [CTF Submission Form](https://docs.google.com/forms/d/e/1FAIpQLSfvDLGmWAheDFyfwfIVsIQNg2j8tLnpmqkar5q0qC5teAdBXg/viewform)
  - [CTF Team Signup Form](https://docs.google.com/forms/d/e/1FAIpQLScdDf6CVkZTf5CpVYxzoRxg7cJjzAYzXBg0SxI8GOKiQ3exUQ/viewform)

`cq-ctf-parser` contains the logic that validates the google sheet data from the forms and updates the standings in real time. 
`cq-ctf-problems` contains all 4 problems, w/ 6 flags worth of content.

teams may be registered and updated in real time with the team signup form. associated emails collected from submission data are connected to the teams they are registered under and then used to update a tally for each team based on serverside data retrieval. 

## current setup:
- enter sheet id's in a `.env` file put in the root file of `/cq-ctf-parser` with the following format:
    ```
    TEAM_SHEET_ID=...
    SUBMISSION_SHEET_ID=...
    ```
- run a development version with `npm run dev` in the parser subdir.


## future changes: 
- UI is a little dookie, but it works. Will be advanced + expanded w/ md readers for future hackathons + diff question bank will be expanded.
- use md files to populate problem sets directly - create customizable format.
- use a proper db instead of google sheets to save teams + progress data for cleaner retrieval support.

- introduce cool new functionalities w/ diff modes for the ctfs! i.e. problem trades, randomly changing problems, etc. -- something fresh!
