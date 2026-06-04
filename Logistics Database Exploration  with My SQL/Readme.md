# Logistics Database Exploration with MySQL Workbench
# Overview

Hey there! Welcome to my database exploration project. This repository is a hands-on deep dive into working with complex relational database schemas. Using a simulated enterprise logistics network, I practiced navigating multi-table architectures, writing clean joins, and solving the kind of real-world debugging issues that happen when your data gets messy.

---

## Project at a Glance

If you’ve ever wondered how global shipping companies track assets, drivers, and deliveries all at once, this is a look under the hood. 

My goals for this exercise were simple:
* **Learn the Land:** Explore how 14 different tables map together to represent a complex corporate supply chain.
* **Connect the Dots:** Write queries that pull disparate data points (like a truck's mileage and a driver's name) into a single, cohesive view.
* **Fix What Breaks:** Troubleshoot common SQL execution errors and write cleaner, more defensive code.

---

This project demonstrates basic SQL querying and table relationships within a logistics management database using MySQL Workbench.

The exercise focuses on:

- Viewing table contents
- Exploring database schema structure
- Retrieving records from individual tables
- Performing JOIN operations between related tables
- Understanding foreign key relationships

---

# Database Information

**Database Name:** `logistics_project`

The database contains multiple tables used to simulate a logistics and transportation environment, including:

- customers
- delivery_events
- driver_monthly_metrics
- drivers
- facilities
- fuel_purchases
- loads
- maintenance_records
- routes
- safety_incidents
- trailers
- trips
- truck_utilization_metrics
- trucks

---

# Snapshot : Image 1 :images/Woohoo,My First SQL Practice Work.png

# Snapshot : Image 2 :images/Woohoo,My First SQL Practice Work(JOIN).png


# Step 1: View Driver Records

The `drivers` table was queried to display all available driver information.

## Query

```sql
SELECT * FROM logistics_project.drivers;
```

## Purpose

This query retrieves every column and row from the `drivers` table, allowing inspection of:

- Driver IDs
- Names
- Hire dates
- License information
- Employment status
- Home terminals

---

# Step 2: Explore Relationships Between Tables

After reviewing the driver data, a relationship between the `trips` and `drivers` tables was identified.

The common field:

```text
driver_id
```

This field acts as a link between both tables.

---

# Step 3: Join Trips and Drivers Tables

A JOIN operation was performed to combine trip information with driver records.

## Query

```sql
SELECT *
FROM trips
JOIN drivers
ON trips.driver_id = drivers.driver_id;
```

## Purpose

This query merges records from:

- `trips`
- `drivers`

based on matching `driver_id` values.

The result provides a consolidated view containing:

- Trip details
- Driver information
- Distance traveled
- Fuel consumption
- Trip duration
- Driver profile data

---

# Error Encountered

## Ambiguous Column Error

When attempting to select `driver_id` directly, MySQL returned:

```text
Error Code: 1052
Column 'driver_id' in field list is ambiguous
```

### Cause

Both tables contain a column named:

```text
driver_id
```

MySQL could not determine which table's column was being referenced.

---

# Resolution

Specify the table name before the column.

## Correct Query

```sql
SELECT
    trips.trip_id,
    trips.driver_id
FROM trips
JOIN drivers
ON trips.driver_id = drivers.driver_id;
```

Or:

```sql
SELECT
    trips.trip_id,
    drivers.first_name,
    drivers.last_name
FROM trips
JOIN drivers
ON trips.driver_id = drivers.driver_id;
```

This removes ambiguity and allows MySQL to identify the correct column source.

---

# Key SQL Concepts Practiced

## SELECT

Used to retrieve data from a table.

Example:

```sql
SELECT * FROM drivers;
```

---

## JOIN

Used to combine rows from multiple tables.

Example:

```sql
SELECT *
FROM trips
JOIN drivers
ON trips.driver_id = drivers.driver_id;
```

---

## Foreign Key Relationships

A foreign key creates a connection between tables.

Example:

```text
trips.driver_id
        ↓
drivers.driver_id
```

This relationship allows driver information to be associated with individual trips.

---
# Logistics Database Exploration with MySQL Workbench

## Overview

This project demonstrates basic SQL querying and table relationships within a logistics management database using MySQL Workbench.

The exercise focuses on:

- Viewing table contents
- Exploring database schema structure
- Retrieving records from individual tables
- Performing JOIN operations between related tables
- Understanding foreign key relationships

---

# Database Information

**Database Name:** `logistics_project`

The database contains multiple tables used to simulate a logistics and transportation environment, including:

- customers
- delivery_events
- driver_monthly_metrics
- drivers
- facilities
- fuel_purchases
- loads
- maintenance_records
- routes
- safety_incidents
- trailers
- trips
- truck_utilization_metrics
- trucks

---

# Step 1: View Driver Records

The `drivers` table was queried to display all available driver information.

## Query

```sql
SELECT * FROM logistics_project.drivers;
```

## Purpose

This query retrieves every column and row from the `drivers` table, allowing inspection of:

- Driver IDs
- Names
- Hire dates
- License information
- Employment status
- Home terminals

---

# Step 2: Explore Relationships Between Tables

After reviewing the driver data, a relationship between the `trips` and `drivers` tables was identified.

The common field:

```text
driver_id
```

This field acts as a link between both tables.

---

# Step 3: Join Trips and Drivers Tables

A JOIN operation was performed to combine trip information with driver records.

## Query

```sql
SELECT *
FROM trips
JOIN drivers
ON trips.driver_id = drivers.driver_id;
```

## Purpose

This query merges records from:

- `trips`
- `drivers`

based on matching `driver_id` values.

The result provides a consolidated view containing:

- Trip details
- Driver information
- Distance traveled
- Fuel consumption
- Trip duration
- Driver profile data

---

# Error Encountered

## Ambiguous Column Error

When attempting to select `driver_id` directly, MySQL returned:

```text
Error Code: 1052
Column 'driver_id' in field list is ambiguous
```

### Cause

Both tables contain a column named:

```text
driver_id
```

MySQL could not determine which table's column was being referenced.

---

# Resolution

Specify the table name before the column.

## Correct Query

```sql
SELECT
    trips.trip_id,
    trips.driver_id
FROM trips
JOIN drivers
ON trips.driver_id = drivers.driver_id;
```

Or:

```sql
SELECT
    trips.trip_id,
    drivers.first_name,
    drivers.last_name
FROM trips
JOIN drivers
ON trips.driver_id = drivers.driver_id;
```

This removes ambiguity and allows MySQL to identify the correct column source.

---

# Key SQL Concepts Practiced

## SELECT

Used to retrieve data from a table.

Example:

```sql
SELECT * FROM drivers;
```

---

## JOIN

Used to combine rows from multiple tables.

Example:

```sql
SELECT *
FROM trips
JOIN drivers
ON trips.driver_id = drivers.driver_id;
```

---

## Foreign Key Relationships

A foreign key creates a connection between tables.

Example:

```text
trips.driver_id
        ↓
drivers.driver_id
```

This relationship allows driver information to be associated with individual trips.

---

# Skills Demonstrated

- Database navigation in MySQL Workbench
- SQL querying
- Data exploration
- Relational database concepts
- Table joins
- Troubleshooting SQL errors
- Understanding primary and foreign keys

---

# Tools Used

- MySQL Server 8.0
- MySQL Workbench
- SQL

---

# Learning Outcome

This exercise reinforced how relational databases store related information across multiple tables and how JOIN operations can be used to retrieve meaningful combined datasets. It also highlighted the importance of qualifying column names when working with tables containing duplicate field names.
# Skills Demonstrated

- Database navigation in MySQL Workbench
- SQL querying
- Data exploration
- Relational database concepts
- Table joins
- Troubleshooting SQL errors
- Understanding primary and foreign keys

---

# Tools Used

- MySQL Server 8.0
- MySQL Workbench
- SQL

---

# Learning Outcome

This exercise reinforced how relational databases store related information across multiple tables and how JOIN operations can be used to retrieve meaningful combined datasets. It also highlighted the importance of qualifying column names when working with tables containing duplicate field names.
