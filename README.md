# Celestial-Bodies-Database-FREECODECAMP
SQL script to create and populate a database for a fictional universe, including tables for galaxies, stars, planets, moons, and black holes.

# Universe Database SQL Script

This repository contains a SQL script (`universe.sql`) for creating and populating a database for a fictional universe. The database includes several tables representing entities in the universe, such as galaxies, stars, planets, moons, and black holes.

## Purpose
The purpose of this script is to:
- Create a relational database that models a fictional universe with galaxies, stars, planets, moons, and black holes.
- Populate the tables with sample data.
- Illustrate how these entities relate to one another through foreign key constraints.

## Tables Created

The following tables are created in the database:
- **galaxy**: Represents different galaxies in the universe.
- **star**: Represents stars, each of which is part of a galaxy.
- **planet**: Represents planets that orbit stars.
- **moon**: Represents moons that orbit planets.
- **blackhole**: Represents black holes within galaxies.

## Data Types Used
- **INT**: For numerical values such as mass, diameter, and radius.
- **NUMERIC**: For representing mass and other large or precise values.
- **VARCHAR**: For textual data like names of galaxies, stars, planets, etc.
- **BOOLEAN**: For attributes such as `is_habitable` or `has_atmosphere`.

## Relationships
- A **star** is linked to a **galaxy** (foreign key relationship).
- A **planet** is linked to a **star** (foreign key relationship).
- A **moon** is linked to a **planet** (foreign key relationship).
- A **black hole** is linked to a **galaxy** (foreign key relationship).

## Sample Data
The script also includes sample data for:
- 6 galaxies
- 6 stars
- 12 planets
- 20 moons
- 5 black holes

## Running the Script

1. **Create the database**:
   Run the following command in PostgreSQL to create the database:
   ```sql
   CREATE DATABASE universe;
