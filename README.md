# Vanessa Littler | Growing Video Game Sales Project

An analysis on the video games industry.

## Quick links

- [Analytics dashboard](https://public.tableau.com/app/profile/vanessa.littler/viz/videogamesanalysis_17915487186250/VideoGameAnalysis#1)
- [About the project](#about-the-project)
- [Tools used](#tools-used)
- [Data](#data)
- [Project artifacts](#project-artifacts)
- [Project deliverables](#project-deliverables)

## About the project

This is a personal project which explores video game industry data to help better understand sales performance and market trands. I did this with the intention to then present research, data findings and actionable insights to a group of stakeholders from a fictional game developer business to help solidify business goals and improve sales performance.

Key questions to answer:
- Which year performed the best based on unit sales?
- What was the split between the varying game genres available?
- Overall, which game genre performed the best based on unit sales?

For this project, the video games industry was chosen as the focus as this is an area that has always fascinated me. I enjoy playing video games myself and I've always found it interesting to see the variety of games available over the years, as well as understanding how each perform and what can influence best-selling games across the market.

## Tools used

- Python
- SQL
- BigQuery
- Tableau
- Excel
- PowerPoint

## Data

The data used within this project was sourced by a data scraper ([vgchartzScraper](https://github.com/GregorUT/vgchartzScrape)) originally found linked to the Video Game Sales dataset available on [Kaggle](https://www.kaggle.com/datasets/gregorut/videogamesales).

Fields within this data set are:
- Rank - ranking of overall sales
- Name - the name of the game
- Platform - the platform the game released on (e.g. PC, Xbox, Playstation, Nintendo)
- Year - year of the game's release
- Genre - genre type of the game
- Publisher - the name of the game's publisher
- NA_Sales - unit of sales within North America (in millions)
- EU_Sales - unit of sales within Europe (in millions)
- JP_Sales - unit of sales within Japan (in millions)
- Other_Sales - unit of sales within the rest of the world (in millions)
- Global_Sales - unit of sales worldwide (in millions)

The original dataset available on Kaggle only held older records (prior to 2020) which is why I decided to run the data scraper myself. Doing this helped highlight a major challenge with the data, which was incomplete or redundant information.

The issue I'd found was that whilst the data scraper was capable of updating the dataset, the original website source that the data scraper is reliant on wasn't complete or up to date itself. This meant that after pulling the data, the majority of the games information which were listed with a release between 2021-2026 was incomplete and at times, creating incorrect information. 

To counter this, I cleaned the dataset using SQL and BigQuery to remove any NULL values as well as the incomplete and redundant information. This meant that with my data, I could only base my research and evaluations on games released prior to 2020.
