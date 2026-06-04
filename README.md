# Harry Potter — Network Analysis, Information Spread & Influence Maximisation

A report submitted to SVKM's Narsee Monjee Institute of Management Studies (NMIMS) as part of Semester III of Bachelor of Science Applied Mathematical Computing.

**By:** Tanushri Shetty (A011)

---

## Project Overview

The full pipeline covers:
- **Character Scraping** — extracting character lists from fan study websites using BeautifulSoup
- **Network Construction** — using spaCy Named Entity Recognition (NER) and a sliding window approach to detect character co-occurrences and build weighted graphs
- **Network Visualisation** — static plots with matplotlib and interactive networks with pyvis
- **Centrality Analysis** — identifying the most important characters using degree, closeness, and betweenness centrality
- **Community Detection** — uncovering character groupings using the Louvain algorithm
- **Information Spread** — simulating how news/rumours spread through the network using the Independent Cascade (IC) model
- **Influence Maximisation** — comparing seeding strategies (degree, PageRank, betweenness) and brute-forcing optimal seed sets to maximise network reach

---

### Book Text Files
The Harry Potter books are copyrighted and cannot be included in this repository. To run the notebook, source the plain text versions of the books yourself and place them in the project directory as:

1. Book1.txt   # Harry Potter and the Philosopher's Stone
2. Book7.txt   # Harry Potter and the Deathly Hallows

---

### Running the Notebook
The notebook is designed to run on **Google Colab**. Upload `Book1.txt` and `Book7.txt` to your Colab session (`/content/`) and run all cells in order.

---

## Key Findings
- **Harry** is the most central character in both books by all centrality measures
- Community detection reveals groupings that closely mirror the book's factions (e.g. Hogwarts students, Death Eaters, the Order of the Phoenix)
- Higher-degree seeding strategies consistently outperform random seeding in the IC simulations
- The optimal 2-node seed set for maximum influence is identified via brute-force search

---

## Tools & Libraries
| Library | Purpose |
|---|---|
| spaCy | Named Entity Recognition |
| NetworkX | Graph construction and analysis |
| pyvis | Interactive network visualisation |
| python-louvain | Louvain community detection |
| BeautifulSoup | Web scraping |
| matplotlib | Static visualisation |
