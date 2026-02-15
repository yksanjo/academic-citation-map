# Global Academic Citation Map 📚

A high-compute scraping project that builds citation graphs from arXiv, conference proceedings, and academic databases. Track influence propagation, identify emerging research clusters, and visualize the scholarly knowledge graph.

## 🎯 Project Overview

**Goal**: Create a comprehensive academic intelligence system to:
- Build citation graphs from multiple sources
- Track influence propagation across papers
- Identify emerging research clusters
- Predict breakthrough papers
- Enable VC scouting and R&D intelligence

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                  Global Academic Citation Map                   │
├─────────────────────────────────────────────────────────────┤
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────────┐   │
│  │   Source    │  │  Citation  │  │   Influence    │   │
│  │   Scrapers  │──▶│  Builder   │──▶│   Analyzer     │   │
│  └─────────────┘  └─────────────┘  └─────────────────┘   │
│                   └─────────────┘  ┌─────────────────┐   │
│  ┌─────────────┐  ┌─────────────┐  │   Cluster      │   │
│  │  arXiv API  │  │  Graph DB  │  │   Detector     │   │
│  │  CrossRef   │  │  (Neo4j)   │  └─────────────────┘   │
│  │  Semantic   │  └─────────────┘                          │
│  └─────────────┘                                             │
└─────────────────────────────────────────────────────────────┘
```

## 📊 Data Sources

- **arXiv**: Preprints and submissions
- **CrossRef**: DOI metadata and citations
- **Semantic Scholar**: Paper graphs and metrics
- **Google Scholar**: Citation counts
- **Conference Sites**: CVPR, NeurIPS, ICML, etc.

## 🔧 Tech Stack

- **Language**: Python
- **Scraping**: arXiv API, CrossRef, Scrapy
- **Graph Database**: Neo4j
- **Vector Store**: Pinecone
- **Embeddings**: SciBERT, Specter
- **API**: FastAPI
- **NLP**: spaCy, transformers

## 🚀 Getting Started

```bash
# Clone the repo
git clone https://github.com/yksanjo/academic-citation-map.git
cd academic-citation-map

# Install dependencies
pip install -r requirements.txt

# Set up environment
cp .env.example .env

# Run the scraper
python src/scrapers/arxiv_scraper.py

# Start the API
uvicorn src.api.main:app --reload
```

## 📈 Features

- [ ] Multi-source academic data collection
- [ ] Citation graph construction
- [ ] Influence scoring algorithms
- [ ] Research cluster detection
- [ ] Topic modeling and embeddings
- [ ] Trend prediction
- [ ] Interactive knowledge visualization

## 📊 Project Phases

### Phase 1: Data Collection
- arXiv API integration
- CrossRef metadata fetching
- Conference proceedings scraping

### Phase 2: Graph Building
- Citation network construction
- Entity resolution
- Influence metrics calculation

### Phase 3: Intelligence
- Embeddings generation
- Cluster detection
- Trend analysis

### Phase 4: Visualization
- Interactive graphs
- Research dashboard
- API access

## 📝 License

MIT License - See [LICENSE](LICENSE) for details.

## 👤 Author

Yoshi Kondo - [@yksanjo](https://github.com/yksanjo)

---

🔬 Map the frontier of human knowledge!
