# PostGIS Database Orchestration

**Student:** Elham Alavy
**Course:** GIST 604B – Open Source GIS
**Module:** Module 4 – PostGIS Database Orchestration
**University of Arizona**

## Project Description
This repository contains SQL-based spatial analysis work completed as part of Module 4, using a PostGIS-enabled PostgreSQL database with real-world NYC datasets. I set up a PostGIS environment using Docker, imported spatial shapefiles, and wrote SQL queries to perform geometry operations, spatial relationship analysis, and spatial joins on New York City neighborhood, street, census block, and subway station data.

## Tools and Technologies
- PostgreSQL with PostGIS extension
- Docker / Docker Compose
- shp2pgsql (shapefile importer)
- SQL (spatial queries)
- GitHub Codespaces

## What I Did
- Set up a PostGIS-enabled PostgreSQL database using Docker inside GitHub Codespaces
- Downloaded and imported four NYC shapefiles (neighborhoods, census blocks, streets, subway stations) into the database using `shp2pgsql`
- Wrote basic SQL queries to explore and filter the dataset
- Performed geometry queries including area, length, and coordinate extraction
- Wrote spatial relationship queries to test containment, intersection, and proximity
- Completed spatial join queries combining multiple tables for multi-layered spatial analysis

## How to View / Run
- Open this repository in GitHub Codespaces
- Start the database: `docker compose up -d`
- Connect to the `nyc` database using the PostgreSQL Explorer (VS Code extension)
- Open any `.sql` file in the `sql/` folder, select the query lines, right-click, and choose **Run Query**

## Repository Structure

    .
    ├── README.md
    ├── .devcontainer
    │   ├── devcontainer.json
    │   └── Dockerfile
    ├── sql/
    │   ├── 01_basic_sql_queries.sql
    │   ├── 02_geometry_queries.sql
    │   ├── 03_spatial_relationships.sql
    │   └── 04_spatial_joins.sql
    ├── demos/
    │   ├── demo_aggregation_queries.sql
    │   ├── demo_basic_queries.sql
    │   ├── demo_filtering_queries.sql
    │   └── demo_postgis_queries.sql
    └── docker-compose.yml

