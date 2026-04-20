This is the repo for SI568's Project 3. The initial data exploration focuses on the CITI Bike Data from 202102 to 202602. The current dataset is not pushed due to its size. So please download the data on your own machine locally.

CITI Bike Data Link (**2021-02 through 2026-02** ): https://citibikenyc.com/system-data

NOAA Climate Data Services Online: https://www.ncdc.noaa.gov/cdo-web/webservices/v2

HQ - Source of Truth Tracker: https://docs.google.com/document/d/1KfDzCL_afwyTe7L13GAJn73Ou3fimS-lT8TYOlL2dI4/edit?tab=t.0

## Project Overview
This project, related to operation chaos commute, is a theoretical data science project that demonstrates how publicly available transit data could be misused to generate undesirable practical consequences.

On the surface, it offers an intelligent commuting app that helps commuters find the most efficient routes and predicts commuting times. But there is a deliberately biased design and modeling, leading to errors in predictions and poor route decision-making.

While the idea is not to actually build such an evil system, it aims to raise awareness on how irresponsible usage of data science techniques may lead to unfairness and social harm.

## Villainous Goal
The system simulates a realistic data-driven application that subtly manipulates commuting decisions. By selectively handling data, introducing bias, and hiding uncertainty, the model produces misleading results while still appearing reliable.

Key intentions include:
* Creating delays, missed transfers, and inefficient routes
* Maintaining user trust through occasional correct predictions
* Making failures appear random rather than systematic
* Increasing inequality by disproportionately affecting vulnerable groups

## Target Users (Victims)
The primary affected groups include:
* Daily commuters (especially peak-hour workers)
* Students and campus travelers
* People with disabilities rely on predictable routes
* Low-income individuals with limited transportation alternatives

A secondary impact targets:
* Public transit agencies
* City governments (through reduced trust and perceived inefficiency)

## Harmless Surface Story
The application is presented as:

> A smart urban mobility tool that optimizes routes, reduces congestion, and improves commuting efficiency.

Why this works:
* Uses real public datasets
* Has a polished interface
* Produces accurate results sometimes
* Errors resemble normal system uncertainty
This makes the manipulation difficult to detect and allows harm to persist over time.

## Dataset & Data Sources
### Primary Dataset
NYC Citi Bike Trip History Data
  * Trip duration
  * Station information
  * Ride timestamps
  * Rideable type

### Additional Data
NOAA Weather Data API
  * Temperature
  * Precipitation

## Data Analysis & Modeling
### Key Patterns Identified
Peak ridership:
  * Fridays
  * 8:00 AM and 5:00–6:00 PM

Seasonal variation:
  * Higher usage in summer (especially August)

These patterns reveal critical pressure points where users depend most on accurate predictions.

## Modeling Approach
The system:
* Cleans and preprocesses transit data
* Extracts features (hour, day, rush hour, trip duration, etc.)
* Integrates weather data
* Builds a demand prediction model

Although technically reasonable, this pipeline is *intentionally manipulated*.

## Team Members
* Shuzhou (Shirley) Li
* Wenjun Yao
* Sikandar Ali
* Yiting (Tina) Wen
* Jiani (Jennie) Zhang
* Yuren (Bill) Long
