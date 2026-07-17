# International-maritime-piracy-risk-dashboard
Interactive Power BI dashboard analyzing international maritime piracy incidents from 2013 to 2014. Built a relational data model with 8 tables, 6 relationships, and 10 DAX measures to identify high-risk countries, vessel types, and attack conditions. Includes data cleaning, modeling, and a documented reference glossary
# International Nautical Intelligence: Maritime Piracy Risk Dashboard

## Overview
An interactive Power BI dashboard analyzing international maritime piracy 
incidents to identify high-risk vessels, locations, and operating conditions.

## Problem
Which vessels, locations, and conditions carry the highest risk of piracy 
attack, and when are vessels most vulnerable? This dashboard turns 
incident-level piracy reports into a risk profile that flags high-risk 
countries, vessel types, and operating conditions.

## Dataset
Incident-level maritime piracy attack records covering 2013 to 2014, 
including attack date and time, vessel name, type, and flag, vessel status 
at time of attack (anchored, steaming, berthed), attack type (boarded, 
hijacked, fired upon, attempted), geographic coordinates, and country or 
area of incident. The raw data included three related tables: incident-level 
attacks, vessel flag summaries, and location summaries.

## What I Did
- Cleaned and structured raw incident text data, including standardizing 
  vessel type categories and splitting combined fields (vessel name, type, 
  flag, tonnage, and IMO number were originally packed into single 
  delimited fields)
- Built a relational data model linking the attacks table to flag-of-vessel 
  and location reference tables (8 tables, 6 relationships)
- Created 10 DAX measures to calculate metrics such as percentage of 
  successful attacks, total attacks by country, and vulnerability 
  breakdowns by vessel status
- Built a documented reference glossary (vessel type definitions, vessel 
  status definitions) alongside the dashboard for interpretability

## Tools Used
Power BI (data modeling, DAX measures, relationships), Power Query 
(data cleaning and transformation)

## Key Findings
- 73.35% of recorded attacks were successful, indicating most attempted 
  piracy incidents were not repelled
- Indonesia was the highest-risk country by attack volume, and Panama the 
  most vulnerable by vessel flag exposure
- Anchored vessels accounted for 59.68% of attacks, far more than steaming 
  or berthed vessels, confirming that stationary ships in open water are 
  the primary target
- Cargo and tanker vessels were the most frequently targeted vessel types, 
  consistent with their high cargo value and limited maneuverability
- Early morning hours saw the highest concentration of attacks (252 
  incidents), suggesting a clear time-of-day risk pattern

## Dashboard Preview
![Dashboard screenshot](https://github.com/jennquaicoe-netizen/International-maritime-piracy-risk-dashboard/blob/main/International%20Nautical%20Intelligence.png?raw=true)


