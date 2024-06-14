# Netflix Dashboard Project

### Dashboard Link : https://app.powerbi.com/groups/me/reports/34fa1007-68df-4982-af0d-5481e0e802c0/6f4686408591447b0768?experience=power-bi

## Overview

This project involves creating a Power BI dashboard to analyze and visualize data from a Netflix dataset. The dashboard provides insights into Netflix's content library, including trends in show additions, ratings, genres, and more.

## Dataset

The dataset is sourced from a CSV file containing the following columns:
- `show_id`: Unique identifier for each show.
- `type`: Indicates whether it is a movie or TV show.
- `title`: Title of the show.
- `date_added`: Date when the show was added to Netflix.
- `release_year`: Year when the show was released.
- `rating`: Rating of the show.
- `duration`: Duration of the show.
- `duration_type`: Indicates minutes for a movie and seasons for a TV show.
- `cast`: List of cast members.
- `countries`: List of countries where the show was produced.
- `description`: Brief description of the show.
- `directors`: List of directors.
- `listed_in`: Genres of the show.

## Data Preparation

1. **Data Cleaning and Transformation**:
   - Used Excel's text-to-column functionality to split entries in `cast`, `countries`, `directors`, and `listed_in` columns.
   - Saved transformed columns as separate CSV files.
   - Replaced empty cells with `NULL` values.

2. **Database Setup**:
   - Created a MySQL schema.
   - Converted CSV file encoding from UTF-8 to ANSI.
   - Imported CSV data into MySQL tables.

## Power BI Dashboard

1. **Connecting to Data**:
   - Connected Power BI to MySQL database.
   - Imported relevant tables for analysis.

2. **Dashboard Pages**:
   - **Overview Page**:
     - Area Chart: Trend of shows added to Netflix over the years (post-2012).
     - Stacked Column Chart: Distribution of shows by rating and type.
     - Clustered Bar Chart: Count of shows by genre.
     - Map: Geographic distribution of shows.
   - **Single Title View Page**:
     - Slicer: Select specific movie/show by title.
     - Cards: Display details (release year, rating, description).
     - Map: Show country of origin.
     - Multirow Cards: Display genres, cast, directors.
# Snapshot of Dashboard (Power BI Service)

![Overview](https://github.com/pradeeshculer/Netflix-Dashboard/assets/115096109/93709009-3b2c-4415-b2ce-9378568ee394)

![Single Title View Page](https://github.com/pradeeshculer/Netflix-Dashboard/assets/115096109/30d00bb4-362f-4a8e-a91f-b0dd1323ba92)

## Insights

- Peak year for adding shows was 2019; declined post-2019 likely due to COVID-19.
- Majority of shows rated TV-MA, followed by TV-14, TV-PG, R, and PG-13.
- "International Movies" genre had the highest count, followed by dramas, comedies, international TV shows, and documentaries.

## Conclusion

This Power BI dashboard offers comprehensive insights into Netflix's content library, viewer preferences, and trends. It helps understand the distribution of shows across genres, ratings, and geographical locations.
