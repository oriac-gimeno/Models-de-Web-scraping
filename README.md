# Models-de-Web-scraping

End-to-end web scraping & text analysis pipeline with an interactive Streamlit demo.

## Quick summary
- Scrapes visible text (p, headings, article) from public web pages.
- Cleans & tokenizes text (stopwords, punctuation, simple normalization).
- Produces word frequency tables and a downloadable CSV.
- Interactive Streamlit app with WordCloud visual.

## How to run (local)
1. Clone:
   git clone https://github.com/oriac-gimeno/Models-de-Web-scraping.git
   cd Models-de-Web-scraping

2. Create env:
   python -m venv venv
   source venv/bin/activate   # mac/linux
   venv\Scripts\activate      # windows

3. Install dependencies:
   pip install -r requirements.txt

4. Download NLTK resources (one time):
   python -c "import nltk; nltk.download('punkt'); nltk.download('stopwords')"

5. Run app:
   streamlit run app/app.py

## Sample usage
- Posa una llista d'URLs (una per línia)
- Tria nombre de paraules per al WordCloud
- Fes clic a Run i baixa CSV amb mots i comptes

## Data / Legal
Respecteu robots.txt i les condicions d'ús del lloc. No utilitzar per a scraping massiu sense autorització.

## Next steps / roadmap
- Async requests, rotació d'user-agent i proxys
- Paginació i scraping de llarga cua
- NER i sentiment analysis

## License
MIT
