🚢 Titanic ETL Pipeline (Python + Supabase)

An end-to-end ETL (Extract, Transform, Load) pipeline built using Python, Pandas, and Supabase (PostgreSQL) to process and store the Titanic passenger dataset.
This project demonstrates real-world data engineering practices including modular ETL design, data cleaning, batch loading, and cloud database integration.

📌 Project Overview
Extracts raw Titanic passenger data from CSV
Cleans and transforms the dataset
Loads structured data into a Supabase PostgreSQL database
Implements batch inserts with error handling
Designed using modular ETL architecture

🛠 Tech Stack
Python 3.13
Pandas
Supabase (PostgreSQL)
python-dotenv
SQL

🔄 ETL Pipeline Flow
1️⃣ Extract
Reads raw Titanic data from CSV
Stores it in the data/raw/ directory

2️⃣ Transform
Drops unnecessary columns
Handles missing values
Creates new features:
    family_size
    is_alone
    title
Writes cleaned data to data/staged/

3️⃣ Load
Loads transformed data into Supabase
Inserts data in batches for reliability
Handles NULL values correctly
