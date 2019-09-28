# Invenire

### What it does
Find out the specific place you're looking for in just three steps, utilizing a corpus of user reviews.

Used for finding places with special features (a bar, clean environment, certain atmosphere) you want to specify.

Based on the idea of finding that place you are looking for only in three steps:
1. Give it an area to search
2. Give it the type of location you are looking for (bar, museum, park, etc)
3. Give it the specific features you want your place to have (clean, cheap, luxurious, etc)

### What it uses
1. Utilizes Here Geocoder API & the Google Places API
- **User interface** 
    - HTML/CSS (Bootstrap) and Javascript.
- **Natural Language Processing**
    - Get the info on certain types of places near the area selected - **Here Geocoder API**
    - Take the user reviews of the places found - **Google Places API**
    - Process the user reviews to identify which ones have the desired features - **TextBlob (NTLK Framework)**

## Requirements

- Python 3.6+

## Recommendations

Usage of [virtualenv](https://realpython.com/blog/python/python-virtual-environments-a-primer/) is recommended for package library / runtime isolation.

## Usage

To run the server, please execute the following from the root directory:

1. Setup virtual environment

```bash
python3 -m venv env
source env/bin/activate
```

2. Install dependencies

```bash
pip3 install -r requirements.txt
```

3. Install `TextBlob` dependencies

```bash
python -m textblob.download_corpora
```

4. Run Startup server
    
```bash
python3 app.py
```

or via docker-compose

```bash
docker-compose up -d
```
