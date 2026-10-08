Behavioural Model – Netflix Customer Churn Analysis
📌 Overview

This project focuses on analyzing Netflix customer churn using a Netflix Customer Churn dataset.

The project follows a simple data analytics workflow:

Netflix Customer Churn Dataset (CSV)
              │
              ▼
     CSV to SQLite Converter
              │
              ▼
        SQLite Database
              │
              ▼
           Metabase
              │
              ▼
    Data Analysis & Dashboards
              │
              ▼
       Customer Churn Insights


The CSV dataset is first converted into a SQLite database using a CSV to SQLite Converter application. The SQLite database is then connected to Metabase, where the data can be explored through queries, charts, visualizations, and dashboards.

The main objective is to understand customer behavior and identify patterns and factors associated with customer churn.

🎯 Objectives
Analyze the Netflix Customer Churn dataset.
Convert the CSV dataset into a SQLite database.
Store and manage the dataset using SQLite.
Connect the SQLite database with Metabase.
Explore customer demographics and subscription information.
Identify patterns associated with customer churn.
Create meaningful visualizations and dashboards using Metabase.
Generate insights that can help understand customer retention and churn.
🛠️ Technologies and Tools
CSV – Source dataset format
CSV to SQLite Converter – Used to convert the CSV dataset into SQLite
SQLite – Database for storing the converted dataset
Metabase – Data analysis and visualization platform
Java – Required to run the Metabase JAR
Git & GitHub – Version control and project hosting
📊 Dataset

This project uses a Netflix Customer Churn Dataset.

The dataset contains customer-related information that can be used to analyze churn behavior.

Depending on the version of the dataset, the available fields may include information such as:

Customer demographics
Subscription details
Account information
Usage information
Payment information
Customer status
Churn status

The dataset is used for educational and analytical purposes.

🔄 Project Workflow
Step 1 – Obtain the Dataset

Download or obtain the Netflix Customer Churn dataset in CSV format.

Example:

netflix_customer_churn.csv

Step 2 – Convert CSV to SQLite

Open the CSV to SQLite Converter application.

Import the Netflix Customer Churn CSV file and convert it into a SQLite database.

Example output:

netflix_customer_churn.db

Step 3 – Start Metabase

Download the Metabase JAR file from the official Metabase website if you don't already have it.

Place the downloaded file somewhere convenient, for example:

C:\Metabase\metabase.jar

Step 4 – Check Java

Open Command Prompt and check whether Java is installed:

java -version


If Java is installed correctly, CMD will display the installed Java version.

Step 5 – Navigate to the Metabase Folder

Open CMD and navigate to the folder containing metabase.jar:

cd C:\Metabase


You can verify that the JAR exists by running:

dir


You should see:

metabase.jar

Step 6 – Run Metabase

Start Metabase using:

java -jar metabase.jar


Keep this CMD window open while using Metabase.

You should see Metabase startup messages in the CMD window.

Wait until Metabase has finished starting.

Step 7 – Open Metabase in Your Browser

Once Metabase has started, open your web browser and go to:

http://localhost:3000


Metabase normally runs on port 3000 by default.

You should now see the Metabase setup/login page.

🗄️ Connecting SQLite to Metabase

After opening Metabase at:

http://localhost:3000


follow these steps:

Complete the initial Metabase setup if this is your first time.
Go to Admin / Settings.
Open Databases.
Select Add database.
Select the appropriate SQLite database option if available in your Metabase setup.
Provide the path to your SQLite database.
Save the connection.
Verify that the Netflix Customer Churn data is available.

Note: SQLite support/configuration can vary by Metabase version and deployment. Follow the database options shown by your installed Metabase version.

📈 Data Analysis Using Metabase

After connecting the database, the Netflix Customer Churn data can be analyzed using Metabase.

Example questions that can be explored:

What percentage of customers have churned?
Which customer groups have the highest churn rate?
Does subscription type affect churn?
Which demographics have higher churn?
What factors are associated with customer churn?
How does customer behavior differ between churned and active customers?
Which customer segments have the highest retention?
What patterns can be identified among customers who leave Netflix?

Charts and dashboards can then be created to present these findings.

📊 Suggested Metabase Dashboard

A possible dashboard can contain:

Customer Overview
Total Customers
Active Customers
Churned Customers
Overall Churn Rate
Customer Demographics
Customers by Age Group
Customers by Gender
Customers by Location
Subscription Analysis
Customers by Subscription Type
Churn Rate by Subscription Type
Subscription Distribution
Churn Analysis
Churn Rate by Customer Segment
Churned vs. Active Customers
Factors Associated with Churn
📂 Project Structure

A possible project structure is:

Behavioural-Model/
│
├── dataset/
│   └── netflix_customer_churn.csv
│
├── database/
│   └── netflix_customer_churn.db
│
├── README.md
├── .gitignore
└── ...


The actual structure may vary depending on the files included in the project.

⚠️ Metabase JAR and GitHub

The metabase.jar file is not included in this GitHub repository.

The reason is that the Metabase JAR is very large and GitHub's normal Git file-size limit is 100 MB.

Therefore, the project uses .gitignore to prevent metabase.jar from being uploaded.

The .gitignore file should contain:

metabase.jar


Download Metabase separately from the official Metabase website:

https://www.metabase.com/start/oss/jar

💻 Complete CMD Commands

If Metabase is located at:

C:\Metabase\metabase.jar


open CMD and run the following commands sequentially:

cd C:\Metabase


Check the file:

dir


Check Java:

java -version


Run Metabase:

java -jar metabase.jar


After Metabase finishes starting, open your browser and visit:

http://localhost:3000

Quick version
cd C:\Metabase
java -version
java -jar metabase.jar


Then open:

http://localhost:3000


Important: Do not close the CMD window running Metabase. Closing it will stop the Metabase server.

🛑 Stopping Metabase

To stop Metabase, go back to the CMD window where it is running and press:

Ctrl + C


Metabase will stop running.

To start it again later:

cd C:\Metabase
java -jar metabase.jar


Then open:

http://localhost:3000

🔐 Security

Do not commit sensitive information to GitHub, such as:

Database passwords
API keys
Access tokens
Personal credentials
Private configuration files

Use environment variables or secure configuration methods for sensitive information.

🚀 Clone the Project

To download this project from GitHub:

git clone https://github.com/Varsha-998921/Behavioural-Model.git


Then:

cd Behavioural-Model

🤝 Contributing

Contributions and suggestions are welcome.

Fork the repository.
Create a new branch.
Make your changes.
Commit your changes.
Push the branch.
Create a Pull Request.

Example:

git checkout -b feature/new-analysis
git add .
git commit -m "Add new churn analysis"
git push origin feature/new-analysis

👤 Author

Varsha

GitHub: https://github.com/Varsha-998921

📄 License

Add the appropriate license for this project if required.
