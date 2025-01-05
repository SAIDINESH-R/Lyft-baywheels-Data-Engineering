# Bay Wheels Data Engineering Project

## Overview
This project implements an end-to-end data engineering solution for analyzing Lyft's Bay Wheels bike-sharing system in the San Francisco Bay Area. The solution includes data extraction, transformation, loading (ETL), and visualization of bike-sharing patterns and user behaviors.

## Architecture
The project follows a modern data engineering architecture:
- ETL Pipeline orchestrated through Mage AI
- Data Warehouse: Google BigQuery 
- Storage: Google Cloud Platform
- Visualization: Looker Studio
- Data Modeling: Star Schema

The star schema consists of:
- **Fact Table**: fact_rides
 - Tracks rides, durations, distances
 - Contains foreign keys to all dimension tables

- **Dimension Tables**:
 - Date_Dim: Temporal data 
 - Dim_Start_Station & Dim_End_Station: Geographical data
 - Dim_Bike: Bike type and category
 - Dim_Rider: User type information 
 - Dim_Distance: Distance categorization

## Technology Stack
- Python
- Mage AI for ETL orchestration
- Google Cloud Platform
- BigQuery for data warehousing
- Looker Studio for visualization
- SQL for data transformation

## Repository Structure
bay-wheels-project
├── notebooks
│   └── data_transformation.ipynb
├── data_model
│   ├── fact_table.sql
│   └── dimensional_tables.sql
├── visualizations
│   └── dashboard.pdf
├── architecture
│   └── gap_architecture.png
└── README.md

## Key Insights
Analysis of 261,311 bike rides revealed:
- Electric bikes dominate with 209,048 rides vs 52,263 classic bikes
- Average ride duration: 12.71 minutes
- Market Street emerged as prime starting location
- Distinct usage patterns between subscribers and casual riders
- Peak usage during commute hours
- Geographic concentration in San Francisco and San Jose areas

## Dashboard Features
- Time series analysis of daily rides
- Subscriber vs casual rider patterns
- Electric vs classic bike usage trends
- Station popularity heat maps
- Peak hour visualizations
- Distance and duration metrics
- Interactive filtering capabilities

## Future Enhancements
- Real-time data processing
- Machine learning integration
- Predictive analytics
- Enhanced geospatial analysis
- Advanced user segmentation

## Contact & Acknowledgments
Special thanks to @snkpgithub for project guidance and mentorship.

Contact: [LinkedIn](https://www.linkedin.com/in/sai-dinesh-rachakonda-4b9767338/)

## License
