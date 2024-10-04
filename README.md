# Spotify-analysis-using-Advance-SQL
Over View
This project involves analyzing a Spotify dataset with various attributes about tracks, albums, and artists using SQL. It covers an end-to-end process of normalizing a denormalized dataset, performing SQL queries of varying complexity (easy, medium, and advanced), and optimizing query performance. The primary goals of the project are to practice advanced SQL skills and generate valuable insights from the dataset.

Project Steps
1. Data Exploration
Before diving into SQL, it’s important to understand the dataset thoroughly. The dataset contains attributes such as:
 Artist: The performer of the track.
 Track: The name of the song.
 Album: The album to which the track belongs.
 Album_type: The type of album (e.g., single or album).
 Various metrics such as danceability, energy, loudness, tempo, and more.

3. Querying the Data
After the data is inserted, various SQL queries can be written to explore and analyze the data. Queries are categorized into easy, medium, and advanced levels to help progressively develop SQL proficiency.

   Easy Queries
   Simple data retrieval, filtering, and basic aggregations.

   Medium Queries
   More complex queries involving grouping, aggregation functions, and joins.

   Advanced Queries
   Nested subqueries, window functions, CTEs, and performance optimization.

3. Query Optimization
In advanced stages, the focus shifts to improving query performance. Some optimization strategies include:

   Indexing: Adding indexes on frequently queried columns.
   Query Execution Plan: Using EXPLAIN ANALYZE to review and refine query performance.

15 Practice Questions
Easy Level
Retrieve the names of all tracks that have more than 1 billion streams.
List all albums along with their respective artists.
Get the total number of comments for tracks where licensed = TRUE.
Find all tracks that belong to the album type single.
Count the total number of tracks by each artist.

Medium Level
Calculate the average danceability of tracks in each album.
Find the top 5 tracks with the highest energy values.
List all tracks along with their views and likes where official_video = TRUE.
For each album, calculate the total views of all associated tracks.
Retrieve the track names that have been streamed on Spotify more than YouTube.

Advanced Level
Find the top 3 most-viewed tracks for each artist using window functions.
Write a query to find tracks where the liveness score is above the average.
Use a WITH clause to calculate the difference between the highest and lowest energy values for tracks in each album.
Find tracks where the energy-to-liveness ratio is greater than 1.2.
Calculate the cumulative sum of likes for tracks ordered by the number of views, using window functions.

#Query Optimization Technique
To improve query performance, we carried out the following optimization process:

Initial Query Performance Analysis Using EXPLAIN

We began by analyzing the performance of a query using the EXPLAIN function.
The query retrieved tracks based on the artist column, and the performance metrics were as follows:
Execution time (E.T.): 7 ms
Planning time (P.T.): 0.17 ms

#Index Creation on the artist Column

To optimize the query performance, we created an index on the artist column. This ensures faster retrieval of rows where the artist is queried.

#Performance Analysis After Index Creation

After creating the index, we ran the same query again and observed significant improvements in performance:
Execution time (E.T.): 0.153 ms
Planning time (P.T.): 0.152 ms

#Graphical Performance Comparison

A graph illustrating the comparison between the initial query execution time and the optimized query execution time after index creation.

#Technology Stack
Database: PostgreSQL
SQL Queries: DDL, DML, Aggregations, Joins, Subqueries, Window Functions
Tools: pgAdmin 4 (or any SQL editor), PostgreSQL (via Homebrew, Docker, or direct installation)

