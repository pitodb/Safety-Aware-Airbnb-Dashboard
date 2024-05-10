# README: Safety-Aware Airbnb Dashboard for Travelers

## Team Members:
- Jasmit Gill
- Pietro Del Bianco
- Pranay Reddy

## Course:
BUDT737: Enterprise Cloud Computing and Big Data

## Project Date:
March 10th, 2024

## Dataset Description:
### Airbnb Dataset:
The dataset comprises over 77,000 Airbnb listings from six major US cities, with a focus on Washington DC. Utilizing Spark streaming, we processed the data to include only Washington DC listings, ensuring efficiency and relevance.

### Crime Dataset:
Containing over 26,000 instances of reported crime across the covered cities, this dataset provides detailed crime information essential for analyzing neighborhood safety.

## Methodology:
### Neighborhood Definition (Unsupervised ML):
K-Means Clustering was employed to define 30 distinct neighborhoods based on Airbnb listing locations, simplifying analysis and enhancing user-friendliness.

### Cluster Definition on Crime Data:
Utilizing the same K-Means Clustering process, 30 crime clusters were defined based on geographical crime data, facilitating accurate association with neighborhoods.

### Cluster Distance from Neighborhood Center:
Custom User-Defined Functions (UDFs) in PySpark were used to calculate the Euclidean distance between neighborhood and crime cluster centers, enabling precise crime association.

### Data Cleaning:
Unnecessary columns were removed from the datasets to streamline analysis and enhance efficiency, focusing on relevant information.

### Final Dataset Preparation (SQL):
Using SQL functions, a comprehensive dataset was created, grouping data by neighborhood, aggregating key statistics, and joining Airbnb and crime datasets, forming the foundation for the interactive dashboard.

## Development of Indicators:
To provide travelers with a clear understanding of neighborhood safety, five crime indicators were developed: Danger Score, Police Surveillance, Theft Score, Property Crime Score, and Crime Rate. These indicators were scaled between 0 and 1 for fair comparison.

## Interactive Map Creation:
A crucial component of the dashboard, the interactive map, was developed using the Folium Python library. Integration of HTML and CSS enhanced user experience, providing detailed neighborhood information via pop-up windows.

## Results:
### Dashboard Overview:
The interactive map displays each Washington DC neighborhood with markers. Pop-up windows offer detailed information, including Airbnb listings, average price, and safety indicators. A circle marker indicates danger score.



https://github.com/pitodb/Safety-Aware-Airbnb-Dashboard/assets/112696408/ef469c71-ca58-49fe-95f5-5b99b1187edf




### Key Findings:
- Neighborhood Clustering: Identified 30 distinct neighborhoods, enabling granular analysis.
- Safety Indicators: Developed indicators offer users quick insights into neighborhood safety.
- Price and Safety Correlation: Revealed correlations between Airbnb prices and safety indicators.
- User-Friendly Interface: The interactive map and pop-up windows ensure ease of use for travelers.

## Conclusion:
The Safety-Aware Airbnb Dashboard for Travelers provides a comprehensive solution for travelers, empowering them to make informed decisions about their accommodations based on safety considerations. By integrating Airbnb listings with neighborhood safety data, the dashboard enhances user experience and ensures worry-free travel experiences in Washington DC.
