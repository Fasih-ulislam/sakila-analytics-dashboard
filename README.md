🎬 Sakila Film Analytics Dashboard
A real-time interactive data visualization dashboard built with Streamlit, SQLAlchemy, and Plotly. This application connects to the classic Sakila MySQL database to provide actionable insights into film inventory, rental trends, and rating distributions.

📌 About the Project
This project serves as a bridge between SQL database management and front-end data storytelling. Instead of running manual queries to understand film inventory, this dashboard automates the data extraction process and presents it through an intuitive, user-friendly interface.

Key Analytical Features:

KPI Metrics: Instant visibility into total film counts, average rental rates, and average durations.

Rating Distribution: A breakdown of the inventory by MPAA rating (G, PG, R, etc.).

Rental Rate Trends: Visualizing how pricing is distributed across different categories.

Dynamic Filtering: Sidebar controls to slice data by release year and rating in real-time.

Correlation Analysis: A scatter plot exploring the relationship between film length and rental costs.

🛠️ Tech Stack
Frontend: Streamlit (Data Web Framework)

Visualizations: Plotly Express (Interactive Charts)

Data Manipulation: Pandas

Database ORM: SQLAlchemy

Environment Management: python-dotenv

🚀 Getting Started
1. Prerequisites
Python 3.8+

A running MySQL/PostgreSQL instance with the Sakila database installed.

2. Installation
Clone the repository:

Bash
git clone https://github.com/Fasih-ulislam/sakila-analytics-dashboard.git
cd sakila-analytics-dashboard
Install dependencies:

Bash
pip install -r requirements.txt
3. Environment Variables
Create a .env file in the root directory and add your database connection string:

Code snippet
DATABASE_URL=mysql+pymysql://user:password@localhost:3306/sakila
4. Running the App
Bash
streamlit run app.py
📊 Database Connection & Performance
The app utilizes SQLAlchemy Connection Pooling to ensure efficient database communication:

pool_size: 5

pool_recycle: 1800 seconds (prevents stale connections)

@st.cache_data: Implemented to reduce database load by caching heavy queries.

👤 Author
Your Name

LinkedIn: [muhammad-fasih-cs](https://www.linkedin.com/in/muhammad-fasih-cs/)

GitHub: [Fasih-ulsilam](https://github.com/Fasih-ulislam)
