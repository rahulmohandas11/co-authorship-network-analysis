# Co-authorship Network Analysis

##  Project Overview
The objective of this project was to create a co-authorship network for reserach papers published in 2024 in the field of 'business analytics' with at least one of the authors affiliated to IIM-A and analyze collaboration patterns among the authors. Network analysis techniques have been used to uncover key insights about reserch collaboration patterns and identify key influential researchers in this academic network.

##  Key Findings
- **Network Structure**: There are 263 researchers (nodes) connected through 423 collaborations (edges)
- **Network Type**: Observed small-world properties similar to Barabasi-Albert model and not a random graph
- **Key Influencer**: Prof. Debjit Roy was identified as the most central researcher across all centrality measures
- **Collaboration Pattern**: Highly fragmented network with 59 separate connected components
- **Research Clusters**: Largest observed component contained 26 researchers, indicating tight-knit research groups

##  Technologies Used
- **Python** - Core programming language
- **NetworkX** - Network analysis and graph theory operations
- **Pandas** - Data manipulation and pre-processing
- **Matplotlib and Seaborn** - Data visualizations

## Analysis Components

### 1. Centrality Measures
- **Degree Centrality** - Direct collaboration count
- **Betweenness Centrality** - Bridging role between researchers
- **Closeness Centrality** - Ease of reaching other researchers
- **Eigen-vector Centrality** - Influence based on well-connected collaborators

### 2. Network Comparison
- Random graph model simulation (100 iterations)
- Barabasi-Albert preferential attachment model
- Comparative degree distribution analysis

### 3. Network Structure Analysis
- Connected components identification
- Community detection and clustering patterns
- Small-world vs. scale-free network properties

## Repository Structure
```
co-authorship-network-analysis/
├── README.md                                # Project documentation
├── notebooks
│   └── network_analysis.ipynb               # Jupyter notebook for analysis
├── data/                              
│   └── research_papers_2024.csv             # Raw dataset from OpenAlex
├── visualizations/                     
│   ├── Co-authorship Network.png            # Main network visualization
│   ├── betweenness.png                      # Betweenness Centrality visualization
│   ├── degree.png                           # Degree Centrality visualization
│   ├── degree_distribution_comparison.png   # Network model comparison
│   ├── degree_histogram.png                 # Top 10 researchers by degree
│   ├── eigenvector.png                      # Eigenvector Centrality visualization
└── requirements.txt                         # Python dependencies
```

##  How to Run

### Pre-requisites
```cmd
pip install networkx pandas matplotlib seaborn numpy
```

### Execution
```cmd
# Clone the repository
git clone https://github.com/rahulmohandas11/co-authorship-network-analysis.git

# Navigate to project directory
cd co-authorship-network-analysis

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook

# Open network_analysis.ipynb and run all cells
```

## Business Impact and Apllications

### Academic Strategy Insights
-**Research Collaboration Mapping**: Identify key researchers and potential collaboration opportunities
-**Strategic Partnerships**: Understand cross-institutional research patterns
-**Resource Allocation**: Focus support on high-impact research clusters

### Broader Applications
-**R&D Networks**: Apply similar analysis to R&D and innovation teams
-**Consulting Projects**: Network analysis for organizational restructuring
-**Market Research**: Customer collaboration and influence mapping

## Methodology
1. **Data Collection**: openalex.org for 2024 business analytics research papers with IIM A affiliation
2. **Data Preprocessing**: Author name standardization and co-authorship pair extraction
3. **Network Construction**: NetworkX grapgh object with 263 nodes and 442 edges
4. **Centrality Analysis**: Calculation, interpretation and visualization of four key centrality measures - degree, betweenness, closeness and eigenvector
5. **Model Comparison**: Statistical comparison with theoretical network models

## Technical Skills Demonstrated

-**Network Theory**: Graph analysis, centrality measures, community detection
-**Statistical Analysis**: Model comparison, distribution analysis, correlation studies
-**Data Preparation**: Data cleaning and pre-processing pipelines
-**Python Programming**: Library integration, code optimization
-**Data Visualization & Business Intelligence**: network graphing, visualizations through seaborn and matplotlib, insight generation

## Future Enhancements
-**Temporal Analysis**: Multi-year collaboration trend analysis
-**Topic Modelling**: Research theme clustering using NLP techniques
-**Institutional and geographic mapping**: Institutional (other IIMs or international) collaboration pattern visualization
-**Predictive Modelling**: Future collaboration likelihood prediction
-**Interactive Dashboards**: Interactive dashboards in PowerBI, Tableau or Streamlit for insights presentation

## Contact
**Rahul Mohan**
Senior Consultant | EY-Parthenon
PGD-ABA Candidate 2025-26 | IIM Ahmedabad
rahulmohandas11@gmail.com

---

*This project was completed as part of the Network Analysis by Prof.Pritha Dev Ph.D. in the Post Graduate Diploma in Advanced Business Analytics program at IIM Ahmedabad.*
