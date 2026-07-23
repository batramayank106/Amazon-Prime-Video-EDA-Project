# Dataset Description

## Source

The dataset is sourced from the Amazon Prime Video content library, available on Kaggle.

## Files

### titles.csv

Contains core metadata for 9,871 titles on Amazon Prime Video.

| Column | Type | Description |
|--------|------|-------------|
| id | string | Unique identifier (e.g., tm19248, ts20945) |
| title | string | Movie or show name |
| type | string | MOVIE or SHOW |
| description | string | Plot synopsis |
| release_year | int | Year of release (1916-2024) |
| age_certification | string | Age rating (G, PG, PG-13, R, TV-MA, etc.) |
| runtime | int | Duration in minutes |
| genres | string | JSON-encoded list of genre tags |
| production_countries | string | JSON-encoded list of ISO country codes |
| seasons | float | Number of seasons (shows only) |
| imdb_id | string | IMDb identifier |
| imdb_score | float | IMDb rating (0-10) |
| imdb_votes | float | Number of IMDb user votes |
| tmdb_popularity | float | TMDb popularity index |
| tmdb_score | float | TMDb rating (0-10) |

### credits.csv

Contains cast and crew information for 124,235 credited individuals across 8,861 titles.

| Column | Type | Description |
|--------|------|-------------|
| person_id | int | Unique identifier for each person |
| id | string | Title ID (foreign key to titles.csv) |
| name | string | Person's full name |
| character | string | Character played (actors only) |
| role | string | ACTOR or DIRECTOR |

## Notes

- The `genres` and `production_countries` columns are stored as string-encoded JSON lists and require parsing
- Age certification is missing for a significant portion of titles
- IMDb and TMDb scores are not available for all titles
- The `seasons` column is only populated for TV shows
