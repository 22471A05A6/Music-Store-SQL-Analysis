# 🎵 Music Store SQL Analysis

## 📌 Project Overview

The **Music Store SQL Analysis** project is a SQL-based data analysis project designed to analyze customer purchasing behavior, music preferences, sales performance, and revenue trends.

The project uses a relational Music Store database and SQL queries to transform raw transactional data into meaningful business insights.

---

## 🎯 Business Problem

A music store generates a large amount of customer, invoice, track, artist, and sales data.

The business needs to understand:

- Who are the most valuable customers?
- Which countries generate the most transactions?
- Which cities generate the highest revenue?
- Which music genres are most popular?
- Which artists have the highest number of tracks?
- How do customers spend money on different artists?
- Which genres are preferred in different countries?

Using SQL analysis, these questions can be answered and converted into actionable business insights.

---

## 🎯 Project Objectives

The main objectives of this project are:

- Analyze the Music Store database using SQL.
- Understand customer purchasing behavior.
- Analyze sales and revenue performance.
- Identify popular music genres and artists.
- Identify high-revenue countries and cities.
- Find the highest-spending customers.
- Use SQL concepts to generate meaningful business insights.

---

## 🗄️ Database Schema

The project contains the following tables:

1. `Employee`
2. `Customer`
3. `Invoice`
4. `InvoiceLine`
5. `Artist`
6. `Album`
7. `Track`
8. `Genre`
9. `MediaType`
10. `Playlist`
11. `PlaylistTrack`

### Table Relationships

```text
Artist
   │
   └── Album
          │
          └── Track
                 │
                 ├── Genre
                 └── MediaType

Customer
   │
   └── Invoice
          │
          └── InvoiceLine
                 │
                 └── Track

Playlist
   │
   └── PlaylistTrack
          │
          └── Track

Employee
   │
   └── Customer
