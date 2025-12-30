Analysis of Crime Patterns in Toronto: A Data Mining Approach to Public Safety 🚓📊

📌 Project Overview
This project utilizes historical Major Crime Indicators (MCI) data from the Toronto Police Service (2014-2025) to uncover hidden spatial and temporal patterns in criminal activity. By adopting the CRISP-DM framework, the analysis aims to transition policing and urban planning from a reactive stance to a proactive, evidence-based model.

Our research applies advanced data mining techniques to distinguish systematic clustering from background noise, discover "crime recipes," and predict high-risk environments to optimize resource allocation.

👥 Team Members
Navdisha Bhakri - Seneca Polytechnic

Dhruv Chotalia - Seneca Polytechnic

Vinh Minh Dang - Seneca Polytechnic

🚀 Key Features & Methodology
We employed three distinct data mining algorithms to analyze the dataset:

DBSCAN (Density-Based Spatial Clustering):

Goal: To distinguish systematic spatial clustering of crimes from stochastic background noise.

Finding: Successfully separated the city into core high-density clusters and low-density areas. Assaults were found to align strongly with high-population dense areas (e.g., Downtown, transit hubs).

Apriori (Association Rule Mining):

Goal: To discover conditional "crime recipes" and associations between variables (e.g., location, time, and type of crime).

Finding: Uncovered distinct environmental trends driven by the city's physical infrastructure.

Decision Tree Classification:

Goal: To train an interpretable model for crime prediction based on premises type and other features.

Finding: The model achieved a Recall of 0.88 for Assaults, demonstrating high efficacy in predicting violent crime based on environmental context.

📊 Data Source
The dataset used in this project is the Major Crime Indicators (MCI) 2014-2025, sourced from the Toronto Police Service Public Safety Data Portal.

Total Records Analyzed: ~450,000+ incidents

Key Features: OCC_DATE, REPORT_DATE, OFFENCE, MCI_CATEGORY, PREMISES_TYPE, LAT_WGS84, LONG_WGS84, NEIGHBOURHOOD_158.

🛠️ Technologies Used
Language: Python 3.x

Environment: Jupyter Notebook / Google Colab

Libraries:

pandas & numpy (Data Manipulation & Cleaning)

matplotlib & seaborn (Data Visualization)

scikit-learn (Machine Learning models)

📂 Project Structure
Bash

.
├── data/                   # Dataset files (not included in repo, see Data Source)
├── notebooks/
│   └── Final_Project_SEA500.ipynb  # Main analysis code
├── reports/
│   ├── group_10_ms_4_report.pdf    # Full technical report
│   └── SEA500_Presentation.pptx    # Project presentation slides
└── README.md
⚙️ Installation & Usage
Clone the repository:

Bash

git clone https://github.com/yourusername/toronto-crime-analysis.git
cd toronto-crime-analysis
Install dependencies:

Bash

pip install pandas numpy matplotlib seaborn scikit-learn
Run the Notebook:

Open Final_Project_SEA500.ipynb in Jupyter or Google Colab.

Note: The notebook is currently set up to mount Google Drive. If running locally, comment out the Drive mounting code and ensure the crime.csv file path matches your local directory.

Python

# Update this line in the notebook if running locally
# df_crime = pd.read_csv('path/to/your/crime.csv')
📈 Key Findings
Spatial Trends: Identification of stable "micro-hotspots" for auto theft in suburban commuter belts versus assault clusters in the downtown core.

Temporal Patterns: Crime follows distinct hourly and seasonal trends (e.g., Assaults peak during specific hours and seasons).

Predictive Power: High recall in predicting assaults suggests that violent crimes are often tied to specific premises types rather than being purely random events.

📝 Future Work
Integration of weather data to analyze its correlation with specific crime types.

Real-time dashboard deployment for police resource allocation.

Expansion of the dataset to include demographic data for fairer risk assessment.

📜 License
This project is for educational purposes as part of the SEA500 course at Seneca Polytechnic.

Disclaimer: This analysis relies on reported crime data, which may not reflect total criminal activity due to underreporting or recording biases.
