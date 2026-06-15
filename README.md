# 🕸️ Org Network Analytics & Leadership Intelligence

> **Graph-based people analytics** — map organizational communication networks to identify leadership gaps, high performers, and collaboration bottlenecks.

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://python.org)
[![NetworkX](https://img.shields.io/badge/NetworkX-3.x-orange.svg)](https://networkx.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> 💡 **Extends attrition analytics** — while attrition tells you *who left*, network analysis tells you *who matters* and *what breaks* when they do.

---

## 📌 Business Problem

Org charts show reporting lines — they don't show how work actually gets done. Communication network analysis reveals:
- **Who are the true connectors and knowledge brokers?**
- **Which teams are siloed or over-dependent on single individuals?**
- **Where are the leadership voids that attrition would create?**
- **Who has informal influence beyond their title?**

---

## 🏗️ Project Architecture

```
org-network-analytics-leadership/
├── data/
│   ├── org_hierarchy.csv        # Reporting structure data
│   ├── communication_logs.csv   # Email/Slack interaction data (anonymized)
│   └── performance_data.csv     # Performance ratings and outcomes
├── notebooks/
│   ├── 01_network_construction.ipynb    # Build org graph from data
│   ├── 02_centrality_analysis.ipynb     # Identify key nodes/influencers
│   ├── 03_community_detection.ipynb     # Team cluster analysis
│   ├── 04_leadership_gap_analysis.ipynb # Succession risk scoring
│   └── 05_high_performer_network.ipynb  # High performer collaboration patterns
├── src/
│   ├── graph_builder.py         # Org graph construction
│   ├── centrality.py            # Centrality metrics
│   ├── community.py             # Community detection algorithms
│   └── leadership_scoring.py    # Leadership gap scoring model
├── dashboard/
│   └── app.py                   # Interactive org network dashboard
├── requirements.txt
└── README.md
```

---

## 🔬 Analytics Methods

### Network Centrality Metrics
| Metric | What It Reveals |
|---|---|
| Degree Centrality | Volume of direct connections |
| Betweenness Centrality | Bridge nodes / information brokers |
| Eigenvector Centrality | Influence via well-connected peers |
| PageRank | Overall importance in the org network |
| Clustering Coefficient | Team cohesion level |

### Community Detection
- **Louvain Algorithm** — detect organic team clusters
- **Girvan-Newman** — hierarchical community structure
- **Label Propagation** — fast community assignment at scale

### Leadership Gap Analysis
- Succession risk score: single points of failure in the network
- Knowledge concentration index: over-reliance on key individuals
- Cross-functional bridge score: who connects disparate teams
- High performer cluster analysis: collaboration patterns of top quartile

---

## 📊 Key Outputs

- **Org Network Graph** — interactive visualization (Pyvis / Plotly)
- **Influence Leaderboard** — top-ranked employees by network centrality
- **Succession Risk Report** — nodes whose removal fragments the network
- **Team Silo Detection** — clusters with low cross-team connectivity
- **Leadership Pipeline Score** — readiness assessment per team

---

## 🧠 Use Cases by Stakeholder

| Stakeholder | Use Case |
|---|---|
| CHRO / People Analytics | Succession planning, retention prioritization |
| CEO / Board | Org design decisions, M&A integration |
| VP Engineering | Team topology optimization |
| Data Science Leader | Quantifying informal influence structures |

---

## 🚀 Quick Start

```bash
git clone https://github.com/shobharanip/org-network-analytics-leadership.git
cd org-network-analytics-leadership
pip install -r requirements.txt
jupyter notebook notebooks/01_network_construction.ipynb
```

**Key Libraries:**
```
networkx, community, pyvis, plotly, pandas, scikit-learn, matplotlib
```

---

## 🔗 Related Projects

- [employee-attrition-analytics](https://github.com/shobharanip/employee-attrition-analytics)
- [customer-churn-ltv-strategy](https://github.com/shobharanip/customer-churn-ltv-strategy)

---

## 👩‍💻 Author

**Shobharani Polasa** — AI & Data Leader | [LinkedIn](https://linkedin.com/in/shobharanip) | [GitHub](https://github.com/shobharanip)
