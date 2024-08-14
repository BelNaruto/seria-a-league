# Serie A API Documentation

This documentation provides details on the various endpoints available in the Serie A API. The API provides data related to games, teams, players, and other relevant information about Serie A.
This API can be found on RapidAPI [https://rapidapi.com/belchiorarkad-FqvHs2EDOtP/api/serie-a-league](https://rapidapi.com/belchiorarkad-FqvHs2EDOtP/api/serie-a-league)

## Base URL

**Note:** If the endpoint response link/url does not include the base URL, assume the base URL is `https://espn.com`.


## Table of Contents
1. [Play by Play](#play-by-play)
2. [Box Score](#box-score)
3. [Game Summary](#game-summary)
4. [Schedule](#schedule)
5. [Scoreboard](#scoreboard)
6. [Standings](#standings)
7. [Team List](#team-list)
8. [Team Info](#team-info)
9. [Team Roster](#team-roster)
10. [News](#news)
11. [Player Seasons](#player-seasons)
12. [Player Leagues](#player-leagues)
13. [Player Statistics](#player-statistics)
14. [Team Statistics - Discipline](#team-statistics---discipline)
15. [Team Statistics - Scoring](#team-statistics---scoring)
16. [Team Performance](#team-performance)
17. [Team Transfers](#team-transfers)
18. [Tables](#tables)
19. [Injuries](#injuries)
20. [Team Results](#team-results)
21. [Player Overview](#player-overview)
22. [Player Statistics](#player-statistics-1)
23. [Player Bio](#player-bio)

---


## Box Score

**Endpoint:** `/boxscore`

**Method:** GET

**Query Parameters:**
- `gameId` (required): The ID of the game

**Response:** JSON object containing the box score for the specified game

---

## Game Summary

**Endpoint:** `/summary`

**Method:** GET

**Query Parameters:**
- `gameId` (required): The ID of the game

**Response:** JSON object containing the summary for the specified game


---

## Schedule

**Endpoint:** `/schedule`

**Method:** GET

**Query Parameters:**
- `year` (required): The year for the schedule
- `month` (optional): The month for the schedule
- `day` (optional): The day for the schedule

**Response:** JSON object containing the schedule for the specified date

**Note:** If the link doesn't contain the base URL, remember that the base URL is https://espn.com

---

## Scoreboard

**Endpoint:** `/scoreboard`

**Method:** GET

**Query Parameters:**
- `year` (required): The year for the scoreboard
- `month` (optional): The month for the scoreboard
- `day` (optional): The day for the scoreboard
- `limit` (optional): The maximum number of results to return (default: 100)

**Response:** JSON object containing the scoreboard for the specified date

---

## Standings

**Endpoint:** `/standings`

**Method:** GET

**Query Parameters:**
- `year` (required): The year for the standings
- `group` (optional): The group for the standings (default: 'league', accepted values: 'league', 'conference', 'division')

**Response:** JSON object containing the standings for the specified year and group

---

## Team List

**Endpoint:** `/team/list`

**Method:** GET

**Query Parameters:**
- `limit` (optional): The maximum number of teams to return (default: 400)

**Response:** JSON object containing the list of teams


---

## Team Info

**Endpoint:** `/team/info`

**Method:** GET

**Query Parameters:**
- `teamId` (required): The ID of the team

**Response:** JSON object containing information about the specified team


---

## Team Roster

**Endpoint:** `/team/roster`

**Method:** GET

**Query Parameters:**
- `teamId` (required): The ID of the team

**Response:** JSON object containing the roster of the specified team

---

## News

**Endpoint:** `/news`

**Method:** GET

**Query Parameters:**
- `limit` (optional): The maximum number of news items to return (default: 23)

**Response:** JSON object containing news items

---

## Player Seasons

**Endpoint:** `/player/season`

**Method:** GET

**Query Parameters:**
- `playerId` (required): The ID of the player
- `page` (optional): The page number for pagination (default: 1)

**Response:** JSON object containing the seasons data for the specified player


---

## Player Leagues

**Endpoint:** `/player/leagues`

**Method:** GET

**Query Parameters:**
- `playerId` (required): The ID of the player
- `page` (optional): The page number for pagination (default: 1)

**Response:** JSON object containing the leagues data for the specified player


---

## Player Statistics

**Endpoint:** `/player/statistic`

**Method:** GET

**Query Parameters:**
- `playerId` (required): The ID of the player

**Response:** JSON object containing statistics for the specified player

---

## Team Statistics - Discipline

**Endpoint:** `/team/statistic/discipline`

**Method:** GET

**Query Parameters:**
- `teamId` (required): The ID of the team
- `season` (optional): The season for the statistics (default: 2023)

**Response:** JSON object containing discipline statistics for the specified team

---

## Team Statistics - Scoring

**Endpoint:** `/team/statistic/scoring`

**Method:** GET

**Query Parameters:**
- `teamId` (required): The ID of the team
- `season` (required): The season for the statistics

**Response:** JSON object containing scoring statistics for the specified team

---

## Team Performance

**Endpoint:** `/team/perfomance`

**Method:** GET

**Query Parameters:**
- `teamId` (required): The ID of the team

**Response:** JSON object containing performance data for the specified team


---

## Team Transfers

**Endpoint:** `/team/transfers`

**Method:** GET

**Query Parameters:**
- `teamId` (required): The ID of the team
- `season` (required): The season for the transfers
- `limit` (optional): The maximum number of transfers to return (default: 100)
- `page` (optional): The page number for pagination (default: 1)

**Response:** JSON object containing transfer data for the specified team


---

## Tables

**Endpoint:** `/tables`

**Method:** GET

**Query Parameters:**
- `season` (optional): The season for the tables (default: 2023)

**Response:** JSON object containing tables data for the specified season

---

## Injuries

**Endpoint:** `/injuries`

**Method:** GET

**Response:** JSON object containing injuries data for the current season

---

## Team Results

**Endpoint:** `/team/results`

**Method:** GET

**Query Parameters:**
- `teamId` (required): The ID of the team
- `season` (required): The season for the results

**Response:** JSON object containing results for the specified team and season

---

## Player Overview

**Endpoint:** `/player/overview`

**Method:** GET

**Query Parameters:**
- `playerId` (required): The ID of the player

**Response:** JSON object containing an overview of the specified player

---

## Player Statistics

**Endpoint:** `/player/statistic`

**Method:** GET

**Query Parameters:**
- `playerId` (required): The ID of the player

**Response:** JSON object containing statistics for the specified player

---

## Player Bio

**Endpoint:** `/player/bio`

**Method:** GET

**Query Parameters:**
- `playerId` (required): The ID of the player

**Response:** JSON object containing biographical information for the specified player

