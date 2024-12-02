# BBC News Scraper and Entity Extractor

A Python program that scrapes articles from BBC News and performs named entity recognition on text. Built as part of the JHUB Module 5 Natural Language Processing coursework.

## Features

### BBC News Scraper
- Scrapes articles from any BBC News URL
- Extracts title, date, and full article content 
- Returns data in JSON format
- Handles multiple URLs through iteration
- Removes unwanted content like navigation links and related stories

### Entity Extractor  
- Uses spaCy's natural language processing
- Identifies three types of entities:
 - People
 - Places 
 - Organisations
- Returns entities in JSON format

## Requirements
- Python 3.x
- requests
- beautifulsoup4 
- spacy
- pytest


## Code Structure

The program is split into the following code blocks:

### Block 1: Dependencies
```python
import pytest
import requests 
from bs4 import BeautifulSoup
import json
import spacy
import datetime

