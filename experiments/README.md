# Setup
Run `source setup-env.sh` to setup this experimenting environment

# Relevant Docs
Anki apkg documentation:
https://github.com/SergioFacchini/anki-cards-web-browser/blob/master/documentation/Processing%20Anki's%20.apkg%20files.md

Anki Database Structure:
https://github.com/ankidroid/Anki-Android/wiki/Database-Structure

SQLite in Javascript:
https://github.com/sql-js/sql.js/

# .apkg Figuring
When generating the SQLLite DB for this project:
- graves are empty

- Tables
  - cards
  - col
    - Single row
  - graves
    - empty
  - notes
    - where most of the work actually is
  - revlog
    - empty
  - sqllist_stat1
    - empty

`col` table columns
- id
- crt
- mod
- scm
- ver
- dty
- usn
- ls
- conf
- models
- decks
- dconf
- tags

`notes` table columns
- id
  - eopch miliseconds when this is created
- guid
- mid
- mod
- usn
- tags
- flds
- sfld
- csum
- flags
  - unused
- data
  - unused