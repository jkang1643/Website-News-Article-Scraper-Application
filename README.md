# 🌊 Maritime News Scraper & Topic Extractor

Automate your daily marine, shipping, oil & logistics industry intelligence with this robust Python script that scrapes maritime news from top sources, summarizes content, extracts keywords, and performs Named Entity Recognition (NER) to surface trending topics — all exported cleanly to CSVs for analysis or reporting.

---

## 📌 Features

✅ Scrapes top maritime news websites  
✅ Extracts article metadata (title, summary, keywords, publish date)  
✅ Performs Named Entity Recognition (NER) using spaCy  
✅ Summarizes and logs trending named entities by frequency  
✅ Outputs two professional CSV reports daily:
- `News Update for [Date].csv`
- `Trending Topics for [Date].csv`

---

## 📰 Example Sources

This tool scrapes the most respected sources in the shipping and oil maritime ecosystem:

- [Manifold Times](https://www.manifoldtimes.com)  
- [Marine Insight](https://www.marineinsight.com)  
- [Maritime Executive](https://www.maritime-executive.com)  
- [Bunkerworld](http://www.bunkerworld.com)  
- [Ship & Bunker](https://shipandbunker.com/news)  
- [Splash247](https://splash247.com)  
- [Bunkerspot](https://www.bunkerspot.com/latest-news)  
- [GCaptain](https://gcaptain.com)  
- [TradeWinds](https://www.tradewindsnews.com/news)  
...and many more

> 💡 Easily extensible with more URLs.

---

## 📂 Output Files

### `News Update for [Month Day, Year].csv`
| Title | Summary | Keywords | Named Entities | URL | Publish Date | Extraction Date |
|-------|---------|----------|----------------|------|---------------|-----------------|

### `Trending Topics for [Month Day, Year].csv`
| Entity Name | Entity Type | Frequency | Date |
|-------------|-------------|-----------|------|

---

## 🛠️ Requirements

Install dependencies:

```bash
pip install newspaper3k spacy pandas
python -m nltk.downloader punkt
python -m spacy download en_core_web_sm
