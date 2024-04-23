# Bing-News-Analysis

🚀 Azure Data Engineering project: Binge News Analysis 📈


In this project, I have created an end to end solution for analyzing the binge latest news data. I have used the microsoft fabric for all the tools. Here's a breakdown of the journey:


1️⃣ Data Ingestion: Created pipeline in data Factory which connects to Bing API and ingest all the latest news articles as a raw json structure to the lakehouse.

2️⃣ Synapse Data Engineering: Used synapse data engineering component to read the ingested raw json file and process it to a clean and structured Delta table and load that into the same Lakehouse database.

3️⃣ Synapse Data Science: used this to read this clean Delta table and sentiment analysis is performed further by using a description column which contains information about the news articles so basically we use this information and predicted the sentiment of the news using a pre-trained synapse machine learning model and the data is stored as a Delta table in the Lakehouse.

4️⃣ PowerBI Dashboard - Created two page report one page was autocreated by powerbi and then I created a new page which is our main news dashboard based on requirements in this dashboard I have configuration in a way that every time when I open this report only the latest news that are published in the last 24 hours will be displayed.

5️⃣ Final ADF Pipeline - Created a pipeline in data Factory to connect all the task end to end and scheduled the pipeline to run every single day exactly at 6:00 a.m.

6️⃣ Alerts Integration: Integrated alerts into Microsoft Teams, ensuring real-time notifications for updates.
