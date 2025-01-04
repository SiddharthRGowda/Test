# Youtube User Survey Analysis-Dashboard

### Dashboard Link : https://app.powerbi.com/groups/me/reports/7bae0a53-9d06-4a2d-8b3b-f35d9f6172d3/32753c99ca47be2e704b?experience=power-bi

## Problem Statement

This project seeks to analyze YouTube user data to segment customers into distinct groups based on their viewing behaviors, preferences, and psychological traits. The key factors considered include user engagement metrics such as minutes watched, the number of channels subscribed to, and channels watched, along with subjective opinions on content quality, entertainment value, and usefulness. Additionally, personality traits like openness, conscientiousness, extraversion, agreeableness, and neuroticism will be examined to understand how psychological characteristics influence viewing habits and content preferences. By identifying these segments, the study aims to provide actionable insights for content creators and marketers to better target diverse audience groups. This segmentation will enable more personalized content recommendations, improve user satisfaction, and optimize marketing strategies tailored to different viewer profiles. The ultimate goal is to enhance YouTube's ability to deliver relevant content to various user types, thereby increasing platform engagement and customer retention. 



### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : Check the relationships between tables in the Model View.
- Step 5 :Create necessary measures and calculated columns using DAX (e.g., SUM, AVERAGE, COUNT).
- Step 6 : Rename tables and fields for clarity.
- Step 7 : In the report view, under the view tab, theme was selected.
- Step 8 : Since the data contains various ratings, thus in order to represent ratings, a new visual was added using the three ellipses in the visualizations pane in report view. 
- Step 9 : Visual filters (Slicers) were added for four fields named "Clusters", "Age", "Gender" & "Behaviours".
- Step 10 : Three card visuals were added to the canvas, one representing average total time in minutes, total time spent &  sum of videos watched.
           Using visual level filter from the filters pane, basic filtering was used & null values were unselected for consideration into average calculation.
           
           Although, by default, while calculating average, blank values are ignored.
- Step 11 : A line chart was added to the report design area representing the total time spent by minute watch.
- Step 12 : A gauge to represent sum of duration in seconds.
- Step 13 : A Funnel to represent RFM score and number of participants.
- Step 14 :A pie chart to represent device storage.
- Step 15 : The following steps were used to perform customer segmentation: 
  
1.Feature Selection: Key features used in the clustering analysis include: 
 Duration of YouTube usage. Number of channels subscribed to. Number of videos watched in the last 7 days. Opinion ratings (Terrible, Poor, etc.).Device preference (most frequent modality).

2.Clustering Algorithm: K-means clustering was selected for its efficiency in segmenting large datasets. The optimal number of clusters (K) was determined using the elbow method, which plots the sum of squared distances against different values of K and identifies the point of diminishing returns. Clustering via-Agglomerative clustering where items are grouped into clusters based on similarities, starting with each item as a singleton cluster and then merging pairs of clusters until all items are in one large cluster. Examining the cluster formed via line graph and dendrogram with the output obtained from SPSS statistical analysis.

In this two types of clustering is done to obtain the best analysis: Hierarchical clustering: To determine the number of clusters. K-means clustering: For classification and Interpretation 

        
Snap of clustering ,

![Screenshot 2025-01-04 123745](https://github.com/user-attachments/assets/0c5c51ed-34c3-430a-b8f4-afedd9d3a71b)

![Screenshot 2025-01-04 123736](https://github.com/user-attachments/assets/dee87199-22de-415b-8fe0-c6b7776143db)

![Screenshot 2025-01-04 125000](https://github.com/user-attachments/assets/8bbada68-fbc5-4360-a81e-57f7f4c1c1c3)

![Screenshot 2025-01-04 124913](https://github.com/user-attachments/assets/252f6f7e-a500-4f62-b9ce-918cff7faa97)

![Screenshot 2025-01-04 124936](https://github.com/user-attachments/assets/fbe9ab73-0b78-4081-9fae-066cf6f6943b)



# Snapshot of Dashboard (Power BI Service)

![Youtube user Survey analysis](https://github.com/user-attachments/assets/a2f8f996-9a6a-4b82-8e8a-bf6a95a80af1)




# Insights

A single page report was created on Power BI Desktop 

Following inferences can be drawn from the dashboard;

### [1] Total Device Usage = 6K Between Age 18-24

   Computer = 1835 (32.77 %)

   Smartphone = 2391 (52.36 %)

   TV  = 559 (9.98 %)

   Tablet = 275 (4.91 %)

   Others = 0


           thus, Smartphone users are Higher.
           
### [2] Average Time spent = 120.97 minutes Between Age 18-24
  
  while calculating average rating, null values have been ignored as they were not relevant for some customers. 
  
  These ratings will change if different visual filters will be applied.  
  
  ### [3] Sum of videos watched = 5K
  
      a) Duration in Seconds = 19K

 ### [4] Some other insights
 
 ### RFM analysis
 
 The x-axis represents Frequency: 
 how many number of videos watched.The y-axis represents Recency: how recently the video has been watched, with higher values indicating more recent activity. 
 
 Color Gradient: The different shades of blue represent the Mean Monetary Value per RF Category, where darker shades correspond to higher monetary values (as seen in the legend on the right). Values range from 280 (lightest blue) to 400 (darkest blue). 

 
 ### High Recency and Frequency:
  Customers who have a high recency score (4 or 5) and a high frequency score (4 or 5) tend to spend more. This is evident from the darker blue squares in the upper right corner, indicating higher monetary values (close to 400). 

         
### RFM Scores and Participants: 
The bar chart shows that 335K RFM scores are distributed among 494K participants. The percentage difference implies that not all users are engaged at the highest levels. 

### Total Time Spent by Minute Watch: 
The line graph indicates fluctuations in total time spent across different segments of users (possibly time buckets). It peaks at 22K, then drops before a slight rise again at 9K. This could point to varying user engagement at different times or with different content. 

### Sum of Duration in Seconds: 
The gauge chart shows a total of 315K seconds of content watched, providing a quick snapshot of total engagement duration. 
