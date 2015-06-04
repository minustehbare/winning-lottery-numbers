# Winning Lottery Numbers tool(s)

This is the start of a tool, or set of tools, that will allow users to retrieve
winning lottery numbers (draws) for a variety of games.

Lottery draws will be output into a JSON file dump and potential features may
include:
  * Command-line options parsing for things like:
    * Game name to retrieve draw information for
    * Date to capture draw information for
    * Flag to indicate whether JSON objects should be represented in a format
    that can be used by
    [MongoDB's](https://www.mongodb.com/) [mongoimport](http://docs.mongodb.org/manual/reference/program/mongoimport/)
    * Credentials to use when accessing public APIs
    (see [SODA Getting Started](http://dev.socrata.com/consumers/getting-started.html)
    and [SODA Registration](http://dev.socrata.com/register)
    * MongoDB connection info to directly write data into MongoDB without using
    an intermediate JSON file
  * Logging
  * Others that do not come to mind

## Draw information
Lottery draw information is, for some games, obtainable through an API.
These are links to interactive data sets for New York that also have API
endpoints to leverage:
  * [Mega Millions](https://data.ny.gov/Government-Finance/Lottery-Mega-Millions-Winning-Numbers-Beginning-20/5xaw-6ayf)
  * [Take 5](https://data.ny.gov/Government-Finance/Lottery-Take-5-Winning-Numbers/dg63-4siq)
  * [Powerball](https://data.ny.gov/Government-Finance/Lottery-Powerball-Winning-Numbers-Beginning-2010/d6yy-54nr)
  * [New York Lotto](https://data.ny.gov/Government-Finance/Lottery-NY-Lotto-Winning-Numbers-Beginning-2001/6nbc-h7bj)
  * [Pick 10](https://data.ny.gov/Government-Finance/Lottery-Pick-10-Winning-Numbers-Beginning-1987/bycu-cw7c)
  * [Quick Draw](https://data.ny.gov/Government-Finance/Lottery-Quick-Draw-Winning-Numbers-Beginning-2013/7sqk-ycpk)
  * [Win-4](https://data.ny.gov/Government-Finance/Lottery-Daily-Numbers-Win-4-Winning-Numbers-Beginn/hsys-3def)
  * [Cash 4 Life](https://data.ny.gov/Government-Finance/Lottery-Cash-4-Life-Winning-Numbers-Beginning-2014/kwxv-fwze)
  
Some may not (yet) be available this way.  Once again, for New York:
  * [Numbers](http://nylottery.ny.gov/wps/portal/Home/Lottery/Home/Daily+Games/NUMBERS)
  
Focus will primarily be on obtaining data through APIs with more elusive games
having a lower priority.
