# Global-Crop-and-Livestock-Data
Given my interest in the Agrotech field, I  gather, process, analyze, and visually represent agricultural data spanning the past two decades, with a focus on crop and livestock production. 

## Introduction
I was introduced to Tableau during my Udacity business analytics course. I really liked it because it takes complex data and turns it into clear, visual stories. It simplifies the process of understanding trends and patterns, making data much more accessible and insightful.
Recently, I’ve become interested in a global market analysis position at a top AgroTech firm. Therefore, as part of my application process, I wanted to expand my agriculture domain knowledge and refine my Tableau skills at the same time. Thus, I find myself on this exciting journey of visualizing agricultural trends.

## Data Collection
For this project, I sourced my data from the Food and Agriculture Organization of the United Nations (FAOSTAT). My aim was to obtain comprehensive data spanning all countries, crops, and livestock items over the past two decades. To achieve this, I acquired the crops and livestock products bulk data file, encompassing information from 1961 for every country and region, detailing aspects such as production, harvested area, and yield.

## Data Processing
After downloading the bulk data, I initiated a sequence of data-wrangling steps to transform the data into a usable format. At first, I utilized Python to perform the wide-to-long data transformation of the years using the pandas library and the pd.melt function. A wide-to-long transformation involves converting a dataset from a format where each observation is represented by multiple columns (variables) into a format where those variables are stacked into a single column, typically resulting in a more organized and suitable format for analysis. Following this, I used Excel to implement additional filters for production and measurement units, to change names containing diacritics, as well as to eliminate outdated countries and regions from the dataset.

However, as the process evolved, I developed a Python script capable of automating the entire workflow. This script streamlined the process from retrieving the data directly from FAOSTAT to generating the necessary CSV file for analysis within Tableau, allowing for easier replication. I've included a link to the full code below. 

Following the data refinement process, I uploaded the Excel sheet to Tableau. Initially, country names were treated as text within the program. However, by adjusting the data type to 'location'  Tableau accurately recognized and mapped these countries geographically.

## Data Visualization
The core objective of this project was to design an exploratory dashboard that allows users to effortlessly access information about crops and livestock for any specific country of interest. The world map visually aggregates the data. Below the map, I created two bar charts. These charts dynamically update based on the selected country, crop, livestock, or year, showcasing the top-producing countries and the most prominent crops and livestock produced in a specific country. I hope users have as much fun exploring the data as I had creating this project!
