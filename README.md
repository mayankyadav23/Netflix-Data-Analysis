# 🎬 Netflix Data Analysis & Database Design 🎥

Welcome to the **Netflix Data Analysis & Database Normalization** project! This project explores the process of cleaning, normalizing, and analyzing Netflix data using SQL and database best practices. It also dives into database design principles to ensure optimized data storage and retrieval.
![Screenshot 2024-10-14 095726](https://github.com/user-attachments/assets/deb851a0-6c0c-4eb9-942c-9bb7541276ff)


## 📑 Project Overview

The original dataset contained two key tables:
- **`titles`**: Information on unique shows and movies.
- **`credits`**: Details on the cast and crew involved in each show or movie.

### Problem
We discovered discrepancies between the two tables:
- The **`credits`** table contained more unique show IDs than the **`titles`** table, leading to inconsistencies.
  
### Solution
We created a unified view by selecting only the common records from both tables, ensuring data consistency throughout the analysis. Afterward, we applied **database normalization** techniques to split the data into smaller, well-organized tables.
![Screenshot 2024-10-14 095838](https://github.com/user-attachments/assets/c350b447-2fd4-455c-87ef-bd22eea825c5)


## 🗂️ Database Design & Normalization

### Key Benefits:
1. **Less Data Duplication**: Improved storage efficiency by reducing redundancy.
2. **Increased Data Integrity**: Accurate and consistent data across all tables.
3. **Improved Query Performance**: Faster and more efficient queries through proper indexing and structure.
4. **Enhanced Security**: More controlled access to sensitive information.

### Database Design
Database design is the organization of data according to a database model. The designer determines what data must be stored and how the data elements interrelate.

After cleaning the Netflix data in Part 1, we obtained two tables - 'titles' containing information about unique shows/movies and 'credits' containing information about the castings in different shows/movies. The data is now distributed in these two tables.
![Screenshot 2024-10-14 101220](https://github.com/user-attachments/assets/cafcb93f-e482-47dd-ab89-1e29f694afcf)

When we counted the unique shows in each of the tables (since both have id column which corresponds to unique shows), we found out that the number of unique shows in credits table is higher than the titles table.
![Screenshot 2024-10-14 101235](https://github.com/user-attachments/assets/ab8a7f75-9845-44ff-8b11-f8c62439ba47)


### Process Overview:
1. **Conceptual Data Model**: High-level view of key entities and relationships.
![image](https://github.com/user-attachments/assets/c98e5287-9ca7-423d-9c3d-57906969fec9)

2. **Logical Data Model**: Detailed relationships and entity specifications.
![image](https://github.com/user-attachments/assets/b67d8b0c-7d88-4aa2-a3e5-6560e78e6519)

3. **Physical Data Model**: Actual implementation of the tables, ensuring optimal performance.
![image](https://github.com/user-attachments/assets/61d4ac6c-55c7-4fee-94cd-25bea4b773c8)

## 🔍 Data Analysis Highlights

### Insights:
- We performed **Exploratory Data Analysis (EDA)** to uncover trends in popular genres, actor appearances, and the distribution of shows across different ratings.
- The normalized tables made it easy to run complex queries on specific data points, providing deeper insights into Netflix's vast content library.

### Queries:
Some of the SQL queries we explored:
- **Most Frequent Actors**: Identify which actors appear most often in Netflix shows.
- **Genre Popularity**: Analyze which genres dominate Netflix’s catalog.
- **Rating Distributions**: Understand how shows and movies are rated across various regions.

### Visualization:
We used tools like **Tableau** and **Power BI** to visualize the findings. Here's an example of how the data looks post-normalization:

![Data Distribution](https://github.com/mayankyadav23/Netflix-Data-Analysis/blob/main/Netflix%20Data%20Analysis%20Dashboard.png)

## 💡 Why Normalize Your Database?

Normalization is crucial for:
- Ensuring **data consistency** across related tables.
- **Eliminating redundancy**, so each piece of data is stored only once.
- Making your database **scalable**, easier to manage, and more flexible for future changes.

## 🚀 Getting Started

### Prerequisites:
- **SQL** (PostgreSQL, MySQL)
- **Python** (for additional data analysis)
- **Tableau/Power BI** (for visualizations)

### Steps:
1. **Clone the repository** to your local environment:
   ```bash
   git clone https://github.com/mayankyadav23/Netflix-Data-Analysis.git
