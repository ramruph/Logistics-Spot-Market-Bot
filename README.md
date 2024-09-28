# Logistics Spot Market Bidding Bot

## Project Overview

This project involves the creation and development of an automated bot that scrapes, analyzes, and executes bids on logistics spot market shipments, optimizing for profitability based on dynamic market conditions. I built, maintained, and continuously improved this system from the ground up during my entire tenure, integrating data scraping, Monte Carlo simulation, and a machine learning Random Forest model to provide strategic, risk-adjusted bids. The bot runs 24/5 and monitors market conditions in real-time, making continuous improvements to its bidding strategy.

**Note: This is a project I created from bottom up, but no longer have access to the code**

---

## Table of Contents
1. [Project Description](#project-description)
2. [Technologies Used](#technologies-used)
3. [Setup & Installation](#setup--installation)
4. [Data Pipeline Overview](#data-pipeline-overview)
5. [Modeling & Optimization](#modeling--optimization)
6. [Results](#results)
7. [Future Improvements](#future-improvements)
8. [Acknowledgments](#acknowledgments)

---

## Project Description

This project was developed entirely from scratch and evolved over time. It involved building, maintaining, and optimizing the system for automating the bidding process for spot market shipments in the logistics industry. Key components include:

- **Data Collection**: Built web scraping modules using **Selenium** and **BeautifulSoup** to collect data from multiple logistics spot market boards and internal data sources. This captured real-time information such as shipment prices, national average price per mile, and internal custom indicators.

- **Data Storage & Processing**: Created an ETL pipeline that cleaned and processed data daily (ranging from 1 GB to 100 GB), which was then stored in a **PostgreSQL database** for analysis and model training.

- **Monte Carlo Simulation**: Designed and implemented a Monte Carlo simulation to predict optimal bids based on logistics market parameters, including fuel costs and market averages.

- **Machine Learning (Random Forest Model)**: **Built and trained the Random Forest model from scratch** using **Scikit-learn**, which continuously improved bid strategies by factoring in real-time market conditions (storms, supply chain disruptions, etc.) and historical data.

- **Bid Execution & Monitoring**: Automated the process of posting bids to spot market boards, tracked performance, and iterated improvements based on performance feedback. Continuous maintenance and optimization ensured that the bot adapted to market changes.

- **Real-Time Monitoring**: Designed **Tableau dashboards** that pulled from **Tableau Server** data sources, allowing for real-time monitoring of the bot’s performance by senior executives.

Throughout my time, I was responsible for every aspect of the system, from its initial design and coding to its ongoing maintenance and improvement, ensuring it evolved as market conditions and business needs changed.

---

## Technologies Used
- **Python**: Used for building web scraping scripts (Selenium, BeautifulSoup), running Monte Carlo simulations, and implementing the Random Forest model.
- **PostgreSQL**: Used for storing large volumes of internal and external data.
- **Selenium & BeautifulSoup**: Web scraping tools used to gather real-time shipment data.
- **Scikit-learn**: Used for building and improving the Random Forest Machine Learning model.
- **Tableau**: For building interactive dashboards to monitor the bot’s performance.
- **VMware**: Virtual machine for hosting the bot and running it continuously (24/5).

---

## Setup & Installation

### Prerequisites
- Python 3.x
- PostgreSQL
- Selenium WebDriver
- Scikit-learn
- Tableau Server
- VMware or any virtual machine for 24/5 operation

---

## Data Pipeline Overview
1. **Data Collection (Scraping)**:
   - Scrape available shipments from various logistic spot market boards using **Selenium** and **BeautifulSoup**.
   - Extract relevant information such as shipment details, price, and market indicators.
   
2. **ETL Process**:
   - Transform and clean the collected data.
   - Store the processed data in a **PostgreSQL** database.

3. **Monte Carlo Simulation**:
   - Simulate potential bids based on current market parameters (fuel costs, price per mile, etc.).
   
4. **Machine Learning Model**:
   - The **Random Forest model**, built with **Scikit-learn**, predicts the optimal price to bid, accounting for dynamic market factors like weather events and supply chain issues.

---

## Modeling & Optimization

- **Monte Carlo Simulation**: Designed from scratch, this simulation runs numerous random scenarios based on current market conditions to predict bid profitability and risk.
  
- **Random Forest Model (Scikit-learn)**: Built, maintained, and iteratively improved the Random Forest model over time, using historical shipment data to make better predictions. The model learns from past performance to make increasingly accurate bid decisions.

---

## Results

- The bot generated approximately **$300,000 in gross profit** by the time I transitioned to a new role.
- It successfully adapted to dynamic market conditions (e.g., storms, fuel price fluctuations, supply chain disruptions), ensuring profitable bids with calculated risk margins.
- **Tableau dashboards** provided real-time performance monitoring for stakeholders, offering insights into the bot’s effectiveness.

---

## Future Improvements
- **Model Enhancements**: Implement advanced machine learning techniques like **XGBoost** or **Neural Networks** to further refine bidding strategies.
- **Expand Data Sources**: Integrate additional external data sources, such as economic indicators or sentiment analysis, to account for broader market trends.
- **Additional Markets**: Automate bidding for more logistics spot market platforms to maximize profitability.

---

## Acknowledgments

Special thanks to Bluegrace Logistics for providing the support and data necessary for the development and deployment oppritunity for this project during my tenure

---
