Description of the Data
This project aims to analyze the major factors affecting economic and GDP growth in Indian cities. We also seek to understand how these factors can guide regional decision-making to drive economic growth. The dataset collected contains data related to economic productivity and performance across 30 Indian cities from 2019 to 2024. The dataset includes key business sectors, such as Information Technology (ICT), Tourism, and Small and Medium-Sized Enterprises (SMEs), along with several economic indicators, including:
•	R&D Expenditure (% of GDP)
•	Patents per 100,000 Inhabitants
•	Unemployment Rate (%)
•	Youth Unemployment Rate (%)
•	SME Employment (%)
•	Tourism Sector Employment (%)
•	ICT Sector Employment (%)
The dataset provided sufficient data to perform analyses on GDP growth and economic factors. Using RapidMiner, several preprocessing steps were completed to prepare the data for analysis:
•	Missing Values: RapidMiner’s "Replace Missing Values" operator was used to handle any missing data points in the dataset.
•	Normalization/Standardization: Since the data involves different scales (e.g., GDP, sector income, unemployment rates), the "Normalize" or "Z-Transformation" operators were applied to ensure that all variables are on a comparable scale. This was important for the accuracy of machine learning algorithms used in the analysis.
Analysis One: Sector Contributions to GDP Growth
The first research question seeks to determine which business sector contributes most significantly to GDP growth across Indian cities. Using sectoral data, we aimed to identify the strongest contributors to GDP growth. RapidMiner’s "Linear Regression" operator was employed to model the relationship between the independent variables (SME Employment, Tourism Sector Employment, ICT Sector Employment) and the dependent variable (GDP growth).

Sector	Impact on GDP Growth
SME Employment (%)	Every 1% increase in SME employment is associated with a 0.3% decrease in GDP growth (negative coefficient: -0.003)
Tourism Sector Employment (%)	Every 1% increase in Tourism sector employment is associated with a 0.2% increase in GDP growth (positive coefficient: 0.002)
ICT Sector Employment (%)	Every 1% increase in ICT sector employment is associated with a 0.1% decrease in GDP growth (negative coefficient: -0.001)
Interpretation: The results indicate that the Tourism sector has a positive impact on GDP growth, with a 0.2% increase in GDP for every 1% increase in Tourism employment. However, both SME Employment and ICT Sector Employment have negative effects on GDP, though relatively small. For example, a 1% increase in SME Employment leads to a 0.3% decrease in GDP.
Analysis Two: Factors Influencing GDP Growth
The second research question explores which factors most influence GDP growth in Indian cities. Using RapidMiner's "Decision Tree" operator, we identified which factors, such as R&D spending, employment rates, and sector-specific income, have the greatest importance in determining GDP growth.

•	Top Predictor: R&D Expenditure (% of GDP) was identified as the most important factor influencing GDP growth. Cities with R&D expenditures greater than 2.5% of GDP consistently showed GDP growth rates above 3%.
•	Unemployment Rate: Cities with unemployment rates lower than 5% tended to have GDP growth rates above 2.8%, while cities with higher unemployment rates experienced slower growth.
•	Tourism Sector Employment: Cities with tourism sector employment above 7% showed an average GDP growth rate of 2.9%.
Interpretation: The decision tree analysis confirms the importance of R&D investment and low unemployment in driving economic growth. Cities investing more than 2.5% of GDP in R&D and maintaining low unemployment rates see stronger GDP growth.
Analysis Three: Clustering Cities by Economic Characteristics
The third research question seeks to uncover patterns among cities based on their economic characteristics. Using the "K-Means Clustering" operator, we grouped cities based on attributes such as GDP growth, employment rates, and sector-specific incomes.
 
Figure 4: Clustering  
•	Cluster 1: Cities with high R&D expenditure (greater than 3% of GDP) and low unemployment (below 4%) fell into this cluster. These cities had an average GDP growth rate of 3.5%.
•	Cluster 2: Cities with moderate ICT and SME Employment (ICT sector employment between 10-15%) showed an average GDP growth rate of 2.2%. These cities also had a moderate unemployment rate (around 6%).
•	Cluster 3: Cities with low R&D expenditure (less than 2% of GDP) and high unemployment rates (above 7%) fell into this cluster. These cities had the lowest GDP growth, averaging 1.8%.
Interpretation:
•	Cluster 1 represents the high-growth cities where R&D investment and low unemployment are driving significant GDP growth. These cities offer a blueprint for economic success.
•	Cluster 2 includes cities with moderate performance, where sectors like ICT contribute to stable but lower growth.
•	Cluster 3 includes cities struggling with high unemployment and low investment in innovation, resulting in the lowest GDP growth.
Analysis Four: Trend Analysis of R&D Expenditure and Unemployment Rate Over Time
The fourth research question aims to analyze the trends of R&D expenditure and unemployment rates over time (2019–2024) and understand how these indicators relate to economic growth in Indian cities.
Results:
 
Interpretation: The data shows fluctuating trends in R&D expenditure over the period analyzed, with a negative value in earlier years (-0.181 and -0.176) and slightly increasing in the later years (0.059). Unemployment rates also show varying trends, peaking in earlier years (0.206) and gradually decreasing over time (-0.267 in later years).
Conclusion
Through the analyses performed, we gained valuable insights into the factors driving GDP growth in Indian cities. The Tourism sector emerged as a positive contributor to GDP growth, with a 0.2% increase for every 1% rise in employment in this sector. However, both the SME and ICT sectors showed negative contributions, though these effects were small. The decision tree analysis confirmed that R&D expenditure and low unemployment rates are critical drivers of GDP growth. Cities with higher investments in R&D and lower unemployment experienced stronger economic growth.
These insights suggest that Indian cities can enhance GDP growth by focusing on innovation, reducing unemployment, and fostering growth in sectors like Tourism. Regional policymakers can use these results to shape economic strategies tailored to their cities' characteristics.
