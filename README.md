<h1 align="center">📘 A Unified Big Data & NLP Platform for Enhancing Rural Education in India</h1>

This project provides a unified Big Data + NLP analytics platform that analyzes five major educational challenges:

Scholarship Awareness

Career Guidance

Dropout Analysis

Language Barriers

Learning Outcome Gaps

The system uses web scraping, NLP models, machine learning, SQLite storage, and visualizations to generate insights for improving rural education outcomes.

<h2 align="center" style="color:#e67e22;">📂 PROJECT STRUCTURE</h2>
Scholarship/
Career/
Dropouts/
Language_Barriers/
Learning_Outcome_Gaps/
database/
visualizations/
notebooks/

<h2 align="center" style="color:#2ecc71;">📌 PAGE 1 — INTRODUCTION & PROBLEM CONTEXT</h2>
Rural Education Challenges

Lack of scholarship awareness

Limited or no career guidance

High dropout rates due to financial & social constraints

Language mismatch between home & school

Learning gaps in Maths, Science, and Languages

Problems are interlinked → need an integrated analytics solution

Project Objective

Build a unified Big Data + NLP platform that analyzes all five modules

Use scraping, NLP, ML, and visualizations

Generate actionable insights for government, NGOs, teachers & students

Tools Used

Python

BeautifulSoup4, Requests

Pandas, NumPy

NLTK, spaCy, TextBlob, VADER, Gensim

Scikit-learn

SQLite

Matplotlib, Seaborn, WordCloud

<h2 align="center" style="color:#9b59b6;">📌 PAGE 2 — SYSTEM ARCHITECTURE & ETL PIPELINE</h2> <h3 style="color:#2F80ED;">EXTRACT</h3>

HTML scraping using BeautifulSoup4 + Requests

No Selenium, Chromium, or APIs

Reads data from portals, blogs, job sites, PDFs, CSVs

<h3 style="color:#2F80ED;">TRANSFORM</h3>

Lowercasing

Removing punctuation, numbers, URLs

Tokenization

Stopword removal

Lemmatization (spaCy)

Regex cleaning

Convert unstructured text → structured clean dataset

<h3 style="color:#2F80ED;">LOAD</h3>

Store all module outputs in SQLite database

Tables created:

scholarships

careers

dropouts

language_issues

learning_gaps

<h3 style="color:#2F80ED;">NLP + ML ANALYTICS</h3>

TF-IDF

Bigram/Trigram extraction

Keyword extraction (RAKE, YAKE)

Sentiment analysis

KMeans clustering

LDA topic modeling

<h3 style="color:#2F80ED;">VISUALIZATION</h3>

Wordclouds

Bar charts

Heatmaps

TF-IDF bar graphs

Cluster scatterplots

<h2 align="center" style="color:#3498db;">📌 PAGE 3 — DATA SOURCES & TEXT ANALYTICS METHODS</h2>
Scholarship Data Sources

National Scholarship Portal (NSP)

Karnataka SSP / Telangana / Maharashtra / UP portals

Ministry of Social & Tribal Welfare portals

NGO scholarship aggregators

Educational blogs & circulars

Career Data Sources

Indeed

Naukri

Glassdoor

NSDC Skill India

Dropout Data Sources

UNICEF

Rural education survey reports

NGO publications

News articles

Language Barrier Data Sources

Research papers

Teacher feedback

Medium-of-instruction studies

Learning Gap Data Sources

ASER reports

Public learning datasets

Academic literature

Text Analytics Methods

Tokenization

Lowercasing

Stopword Removal

Lemmatization

Regex Cleaning

Word Frequency

TF-IDF Vectorization

Bigram/Trigram Extraction

Keyword Extraction (RAKE/YAKE)

Cosine Similarity

Document Clustering

Rule-based Classification

<h2 align="center" style="color:#e74c3c;">📌 PAGE 4 — EXPANDED NLP MODELS & NLP TECHNIQUES</h2> <h3 style="color:#e67e22;">NLP MODELS</h3>
spaCy (en_core_web_sm)

Does: Tokenization, Lemmatization, POS tagging, NER

Why: Standardizes text for ML/NLP

Used in: All modules

VADER Sentiment Analyzer

Does: Polarity scoring (positive/negative/neutral)

Why: Dropout/difficulty text contains emotions

Used in: Dropouts, Language Barriers, Careers

TextBlob

Does: Polarity + subjectivity

Why: Secondary sentiment validation

Used in: Careers, Learning Gaps

Gensim LDA Topic Modeling

Does: Extracts hidden themes

Why: Identify patterns in skills, language, gap data

Used in: Careers, Language Barriers, Learning Gaps

KMeans Clustering

Does: Automatically groups similar text

Why: Cluster scholarships, careers, learning gaps

Used in: Scholarships, Careers, Learning Gaps

<h3 style="color:#27ae60;">NLP TECHNIQUES (Expanded)</h3>
Text Cleaning

Tokenization

Stopword removal

Lemmatization

Regex cleaning

Feature Extraction

TF-IDF

Word Frequency

Keyword extraction

Bigrams/Trigrams

Advanced NLP

Sentiment analysis

Topic modeling

Clustering

Similarity scoring

Rule-based text classification

<h2 align="center" style="color:#16a085;">📌 PAGE 5 — VISUALIZATIONS (MODULE-WISE)</h2>
Scholarship Module Visuals

State-wise bar charts

Category distribution

Eligibility wordcloud

TF-IDF requirement charts

Scholarship clusters

Career Module Visuals

Skill frequency charts

TF-IDF heatmaps

Role clusters

LDA topic outputs

Wordclouds

Dropout Module Visuals

Dropout reason bar charts

Wordclouds

Bigram frequency charts

Sentiment distribution

Region-wise dropout comparison

Language Barriers Visuals

Difficulty heatmaps

Topic clusters

Keyword frequency charts

Region-wise comparison

Learning Gaps Visuals

Subject-wise gaps

Region-based performance

Impact charts

Wordclouds

Scatterplot (text length vs impact)

<h2 align="center" style="color:#8e44ad;">📌 PAGE 6 — MODULE OUTPUTS</h2>
Scholarship Module

Clean SQLite database

Eligibility clusters

Common requirements extracted

Awareness gap insights

Career Module

Skill dictionary

Role clusters

Topic themes

Job description sentiment

Qualification → Career mapping

Dropout Module

Categorized dropout reasons

Sentiment trends

Frequent bigram patterns

Region-wise dropout levels

Language Barriers Module

Vocabulary/grammar difficulty patterns

Topic clusters

Region-language mismatch

Learning Outcome Gaps

Gap severity labeling

Subject & region-wise mapping

TF-IDF conceptual weaknesses

High-impact learning gaps

<h2 align="center" style="color:#c0392b;">📌 PAGE 7 — CHALLENGES, IMPACT, FUTURE SCOPE & ACKNOWLEDGMENT</h2>
Challenges

Highly unstructured, multilingual text

No APIs → complete scraping

Spelling variations & noise

Ambiguous descriptions

Different formats across modules

Impact

Supports scholarship outreach

Helps NGOs target intervention zones

Teachers identify conceptual weaknesses

Students understand career options

Forms a foundation for education analytics

Future Scope

Add BERT-based multilingual NLP

Deploy on AWS, Azure, or Databricks

Add Kafka for real-time pipelines

Build predictive dropout model

AI-based scholarship/career recommender

Student assistance chatbot

Acknowledgment

Special thanks to Sri Lakshmi Ma’am for guidance, feedback, and supervision throughout the project.
