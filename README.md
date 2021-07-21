# ALL-ABOUT-HEATMAPS 

## 1. What is a HeatMap
Heatmaps visualize the data in a 2-dimensional format in the form of colored maps. The color maps use hue, saturation, or luminance to achieve color variation to display various details. This color variation gives visual cues to the readers about the magnitude of numeric values. HeatMaps is about replacing numbers with colors because the human brain understands visuals better than numbers, text, or any written data. Human beings are visual learners; therefore, visualizing the data in any form makes more sense. Heatmaps represent data in an easy-to-understand manner. Thus visualizing methods like HeatMaps have become popular.
Heatmaps can describe the density or intensity of variables, visualize patterns, variance, and even anomalies. Heatmaps show relationships between variables. These variables are plotted on both axes. We look for patterns in the cell by noticing the color change. It only accepts numeric data and plots it on the grid, displaying different data values by varying color intensity.

## 2. Uses of HeatMap
### Business Analytics: 
A heat map is used as a visual business analytics tool. A heat map gives quick visual cues about the current results, performance, and scope for improvements. Heat maps can be continued to be updated to reflect the growth and efforts. These maps can be integrated into a business’s workflow and become a part of ongoing analytics. Heat maps present the data in a visual and easy to understand manner to communicate to team members or clients.
### Website:
Heatmaps are used in websites to visualize data of user’s behaviour. This visualization helps business owners and marketers to identify the best & worst-performing sections of a webpage. 
### Exploratory Data Analysis:
EDA is a task performed by data scientists to get familiar with the data. All the initial studies are done to understand the data are known as EDA. Heatmaps are a compelling way to visualize relationships between variables in high dimensional space. 
### Molecular Biology: 
Heat maps are used to study disparity and similarity patterns in DNA, RNA, etc.
### Geovisualization: 
Geospatial heatmap charts are useful for displaying how geographical areas of a map are compared to one another based on specific criteria. Heatmaps help in cluster analysis or hotspot analysis to detect clusters of high concentrations of activity; For example, Airbnb rental price analysis.
## 3. Types of HeatMaps
Typically, there are two types of Heatmaps:
### Grid Heatmap: 
The magnitudes of values shown through colors are laid out into a matrix of rows and columns, mostly by a density-based function. Below are the types of Grid Heatmaps.
#### Clustered Heatmap: 
The goal of Clustered Heatmap is to build associations between both the data points and their features. This type of heatmap implements clustering as part of the process of grouping similar features. Clustered Heatmaps are widely used in biological sciences for studying gene similarities across individuals.
The order of the rows in Clustered Heatmap is determined by performing hierarchical cluster analysis of the rows. Clustering positions similar rows together on the map. Similarly, the order of the columns is determined.
![image](https://user-images.githubusercontent.com/46440771/126457422-577ce7cd-c9d4-4238-bead-d0401a3d02ed.png)

 

#### Correlogram: 
A correlogram replaces each of the variables on the two axes with numeric variables in the dataset. Each square depicts the relationship between the two intersecting variables, which helps to build descriptive or predictive statistical models.
 ![image](https://user-images.githubusercontent.com/46440771/126457495-302b2702-a5df-4dae-9d43-3c82466b9c76.png)


### Spatial Heatmap: 
Each square in a Heatmap is assigned a color representation according to the nearby cells’ value. The location of color is according to the magnitude of the value in that particular space. These Heatmaps are data-driven “paint by numbers” canvas overlaid on top of an image. The cells with higher values than other cells are given a hot color, while cells with lower values are assigned a cold color.

## Color schemes
Many different color schemes can illustrate the heat map, with perceptual advantages and disadvantages for each. The color palette choices are more than just aesthetics because the colors in the HeatMap reveal patterns in the data. Good color schemes can enhance pattern discovery, and poor color choices can hide it.
General principles for using colors in Heatmaps are:
#### Vary hue to distinguish categories: 
Vary the elements’ color to represent multiple plot categories. Most people can differentiate between a moderate number of shades. It is best to represent categories using hues.
#### 
Vary luminance to represent numbers: Varying brightness helps you see structure in numeric data. In Bivariate distribution, luminance variation enhances discrete or continuous pattern visualization. The luminance color scheme also makes apparent that there are two prominent peaks.


## Hands-on Using Seaborn Heatmap
#### Purpose of Seaborn HeatMap
The seaborn Heatmaps are the grid Heatmaps that can take various types of data and generate heatmaps. The primary purpose of the seaborn heatmap is to show the correlation matrix by data visualization. It helps find the relationship between multiple features and which features are best for Machine Learning model building.
#### Correlation Matrix
A correlation matrix denotes the correlation coefficients between variables at the same time. A heat map grid can represent these coefficients to build a visual representation of the variables’ dependence. This visualization makes it easy to spot the strong dependencies. A positive correlation indicates a strong dependency, while a negative correlation indicates a strong inverse dependency; a correlation coefficient closer to zero indicates weak dependence.
##  How to Read a Seaborn Heat map
The heatmap transforms the correlation matrix into color codings. The correlation matrix shows how the variables are correlated to each other on a scale of -1 to 1. 1 being positively correlated and -1 being inversely correlated. As only numerical features can show the correlation, the heatmap cannot visualize categorical features. Strings need to be encoded to be pictured on the Heatmaps.


## Heatmap Function
seaborn.heatmap(data, *, vmin=None, vmax=None, cmap=None, center=None, robust=False, annot=None, fmt='.2g', annot_kws=None, linewidths=0, linecolor='white', cbar=True, cbar_kws=None, cbar_ax=None, square=False, xticklabels='auto', yticklabels='auto', mask=None, ax=None, **kwargs)

## Create a default Heatmap using Seaborn
#### Heat map representing Data

sns.heatmap(data)
![image](https://user-images.githubusercontent.com/46440771/126457844-af1339c9-2ce5-4db6-9b49-b51fad50f910.png)

#### Heatmap representing Data Correlation matrix
sns.heatmap(data.corr())

![image](https://user-images.githubusercontent.com/46440771/126457993-f1216aef-dd45-4de3-a7ed-2422cabcf482.png)

