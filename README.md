# Data Modeling for POSTGRES database (Fact and Dimension Tables)

## Description

The primary objective of this project is help Sparkify, a fictional music streaming service to analyze songs that users mostly listen to.
However, the data is not stored in a relational database. Meta data about the songs and user activity are stored in **__JSON logs__**. The `etl.py` script extracts data from these JSON logs and stores them in a PostGRES relational database.

## Database Schema and Design

The database schema consists of a fact table and 4 dimension tables.
### Fact Tables

> songplays

* songplay_id
* start_time
* user_id
* level
* song_id
* artist_id
* session_id
* location
* user_agent

### Dimension tables

> users

* user_id
* first_name
* last_name
* gender
* level

> songs

* song_id
* title
* artist_id
* year
* duration

> artists

* artist_id
* name
* location
* lattitude
* longitude

> time

* start_time
* hour
* dat
* week
* month
* year
* weekday

## Example Queries