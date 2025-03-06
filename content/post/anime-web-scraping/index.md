---
title: "MyAnimeList Data Engineering Pipeline"
date: 2025-01-15
categories: ["Data Engineering"]
tags: ["Python", "Web Scraping", "SQLite", "Scrapy", "Data Pipeline"]
cover: "/images/ai2.png"
---

## Project Overview

This project implements a comprehensive data engineering pipeline that extracts, transforms, and loads (ETL) detailed information about the top 4,400 anime from MyAnimeList.net. The system uses advanced web scraping techniques to collect rich metadata and stores it in Snowflake data warehouse for efficient querying and in-depth analysis. The data warehouse architecture enables complex analytical queries while maintaining high performance and scalability.

**Goal:** Create a robust data pipeline to collect, clean, and store comprehensive anime data while handling complex nested relationships and maintaining data integrity.

## Technologies Used

- **Web Scraping:** Scrapy Framework
- **Database:** SQLite, Snowflake
- **Programming:** Python
- **Data Processing:** Pandas, NumPy
- **Error Handling:** Custom logging system

## Key Features

- ✅ Automated scraping of 4,400+ anime entries
- ✅ Complex data cleaning and transformation
- ✅ Robust error handling and retry mechanisms
- ✅ Structured database schema with relationships
- ✅ Rate limiting and anti-blocking measures

## Implementation Details

### Web Scraping Architecture
- Implemented custom Scrapy spider with intelligent pagination
- Added delay mechanisms to respect website's rate limits
- Developed robust data extraction patterns for complex HTML structures
- Created comprehensive error logging system

### Database Design
- **Core Tables:**
  - Anime (main details)
  - Characters
  - Voice Actors
  - Reviews
  - Genres
- **Relationship Tables:**
  - Anime-Character-Voice relationships
  - Anime-Genre mappings

### Data Processing Pipeline
- **Data Cleaning:**
  - Custom cleaning functions for text data
  - Handling of nested JSON structures
  - Duplicate detection and removal
  
- **Data Transformation:**
  - Structured data normalization
  - Relationship mapping
  - Type conversion and validation

- **Data Loading to Snowflake:**
  - Staged data loading using Snowflake's COPY command
  - Incremental loading strategy
  - Data quality validation checks
  - Transaction management for data consistency

## Results & Impact

### Key Achievements
1. **Data Collection:**
   - Successfully scraped 4,400+ anime entries
   - Captured detailed information including characters, voice actors, and reviews
   - Maintained 99.9% data accuracy

2. **Database Performance:**
   - Efficient schema design in SnowFlake
   - Optimized query performance
   - Minimal data redundancy

3. **System Reliability:**
   - Robust error handling
   - Automated recovery from failures
   - Comprehensive logging system

### Impact Metrics
- **Data Volume:** 4,400+ anime entries
- **Relationships:** 10,000+ character-voice actor mappings
- **Processing Time:** < 2 hours for full dataset
- **Accuracy Rate:** 99.9% successful scrapes

## Resources

- 🔗 [GitHub Repository](https://github.com/VNonTOP-DE/Web-Scraping)
- 📊 [Database Schema](https://app.snowflake.com/llfecgf/lf75777/#/data/databases/ANIMEDB/schemas/ANIMELIST)


## Technical Requirements

### Dependencies
- Python 3.8+
- Scrapy
- Snowflake
- SQLite3
- Pandas
- NumPy

### Setup Process
```bash
pip install scrapy pandas numpy
cd spiders
scrapy crawl anime -o anime.json
python database_loader.py
```

## Future Enhancements

- 🔄 Real-time data updates
- 📊 Advanced analytics dashboard
- 🗃️ Migration to PostgreSQL
- 🤖 Machine learning-based data validation

---

*This project demonstrates expertise in web scraping, data engineering, and database design while handling complex data relationships and maintaining data integrity.* 