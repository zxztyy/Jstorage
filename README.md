# Jstorage
# Recruitment Data Analytics & Visualization Platform

A full-stack recruitment data analytics platform built with **Django**, **Apache Spark**, and **MySQL**, providing end-to-end solutions for job data collection, processing, visualization, salary prediction, and personalized job recommendation.

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Django](https://img.shields.io/badge/Django-5.x-green)
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-3.x-orange)
![MySQL](https://img.shields.io/badge/MySQL-8.0-blue)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## Overview

This project aims to build a comprehensive recruitment analytics platform that automatically collects job postings from online recruitment websites, performs large-scale data cleaning and statistical analysis using Apache Spark, and presents insights through interactive visual dashboards.

Besides traditional recruitment analysis, the platform also provides:

- AI-powered salary prediction
- Personalized job recommendation
- Interactive recruitment dashboards
- Administrative management system
- User authentication and favorites management

The project was developed as a graduation project.

---

## Features

### User Module

- User Registration & Login
- Personal Profile Management
- Multi-condition Job Search
- Job Detail Page
- Favorite Jobs
- Personalized Job Recommendation
- Salary Prediction
- Interactive Data Visualization Dashboard

### Administrator Module

- User Management
- Recruitment Data Management
- CRUD Operations
- Batch Delete
- Role-Based Access Control

### Data Analysis Module

- Top 20 Hiring Cities
- Salary Distribution Analysis
- Education vs Salary Analysis
- Experience vs Salary Analysis
- Company Scale Analysis
- Skills Demand Analysis
- High Salary Cities Ranking
- Interactive Visualization Dashboard

---

## Tech Stack

### Backend

- Python
- Django
- Django ORM

### Big Data

- Apache Spark
- PySpark
- Pandas

### Database

- MySQL

### Frontend

- HTML
- CSS
- JavaScript
- Bootstrap
- ECharts

### Data Collection

- Requests
- BeautifulSoup
- Web Crawling

### Recommendation Algorithm

- Content-Based Recommendation
- Cosine Similarity

### AI Integration

- AI Salary Prediction API

---

## System Architecture

```
                Recruitment Website
                        │
                  Web Crawler
                        │
               Raw Recruitment Data
                        │
                Data Cleaning
              (Pandas + PySpark)
                        │
                  MySQL Database
                        │
      ┌─────────────────┴────────────────┐
      │                                  │
 Django Backend                  Spark Analysis
      │                                  │
      └──────────────┬───────────────────┘
                     │
             ECharts Dashboard
                     │
                 End Users
```

---

## Project Structure

```
Recruitment-Analytics-Platform
│
├── backend/
│   ├── apps/
│   ├── templates/
│   ├── static/
│   └── manage.py
│
├── crawler/
│
├── spark/
│
├── sql/
│
├── screenshots/
│
├── requirements.txt
│
├── README.md
│
└── LICENSE
```

---

## Key Functionalities

### Recruitment Data Collection

- Automated web crawling
- Anti-crawling strategy
- Structured data extraction

### Data Cleaning

- Duplicate removal
- Salary normalization
- Missing value processing
- Data standardization

### Data Analysis

The platform performs statistical analysis on:

- Salary
- Education
- Experience
- Company Scale
- Skills
- Cities

using Apache Spark.

---

## Personalized Recommendation

The recommendation engine adopts a **Content-Based Recommendation Algorithm**.

Feature vectors include:

- City
- Job Type
- Education
- Experience
- Salary

The cosine similarity between user preference vectors and candidate jobs is calculated to generate personalized recommendations.

---

## Salary Prediction

The platform provides two salary prediction methods:

### Database-based Prediction

Average salary estimation using historical recruitment data.

### AI-based Prediction

External AI services generate salary estimation and analysis based on:

- Position
- City
- Education
- Experience

---

## Database

Main tables:

- users
- user_profiles
- cleaned_jobs
- userfavorite
- hot_cities_top20
- education_salary
- experience_salary
- skill_salary
- high_salary_cities_top10
- scale_welfare_detail

---

## Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/Recruitment-Analytics-Platform.git
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Configure Database

Create a MySQL database.

Update:

```
settings.py
```

with your database configuration.

### Run Server

```bash
python manage.py runserver
```

---

## Future Improvements

- Docker Deployment
- REST API
- Elasticsearch Integration
- Redis Cache
- JWT Authentication
- Machine Learning Recommendation Models
- Cloud Deployment (AWS / Azure)

---

## License

This project is released under the MIT License.

---

## Author

**J**

Bachelor

GitHub: *(your GitHub profile)*
---

⭐ If you like this project, please consider giving it a star.
