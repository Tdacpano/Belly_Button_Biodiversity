# Belly_Button_Biodiversity
Using Plotly.js, a JavaScript data visualization library, to create an interactive data visualization for the web, based on bacterial species that may reside within individuals belly buttons. We completed a panel for demographic information and then needed to create a visualization on the bacterial data for each volunteer.

# Deliverable 1: Create a Horizontal Bar Chart
We first created a horizontal bar chart to display the top 10 bacterial species (OTUs) when an individual’s ID is selected from the dropdown menu on the webpage. The horizontal bar chart will display the sample_values as the values, the otu_ids as the labels, and the otu_labels as the hover text for the bars on the chart. We accomplished this by creating a variable that has the array for all the samples. Next, we created a variable that will hold an array that contains all the data from the new sample that is chosen from the dropdown menu. We retrieved the data from the new sample, by filtering the variable we just created for the sample id that matches the new sample id chosen from the dropdown menu. Next we created a variable that holds the first sample in the array, and another variable that have arrays for the other data: otu_ids, otu_labels, and sample_values. We finished the first deliverable by creating the trace object, the layout, and Plotly.newPlot() function for the horizontal bar chart. The final outcome was 

<img width="559" alt="Screen Shot 2023-02-22 at 2 26 48 PM" src="https://user-images.githubusercontent.com/117120227/220774148-bbd3bda1-18b4-4c70-bde0-526cc8b7251d.png">

# Deliverable 2: Create a Bubble Chart
The next step was to create a bubble chart that will display the following when an individual’s ID is selected from the dropdown menu webpage. We used the same variables that were created in Deliverable 1 to populate the bubble chart. Therefore the only necessary steps were to create the trace for our bubble chart and assigning out variables to the correct axes. Once we finished the trace, lastly we had to create the layout for the bubble chart, add a title, a label for the x-axis, margins, and the hovermode property. Once executed we used Plotly.newPlot() to plot our bubble chart.

<img width="859" alt="Screen Shot 2023-02-22 at 2 30 19 PM" src="https://user-images.githubusercontent.com/117120227/220774801-26c1f910-9268-49ab-967c-1a959b2b08e2.png">

# Deliverable 3: Create a Gauge Chart
Our last task was to create a gauge chart that displays the weekly washing frequency's value, and display the value as a measure from 0-10 on the progress bar in the gauge chart when an individual ID is selected from the dropdown menu. This was accomplished by creating a a new variable that filters the metadata array within our dataset for an object in the array whose id property matches the ID number from the dropdown menu. We additionally created another variable to hold the first sample in the array along with another variable that converted the washing frequency into a floating point number. Once this was completed we followed the same steps from the first two deliverables and created our trace and layout to correspond with a gauge chart and plotted both. The final outcome came out to this:

<img width="594" alt="Screen Shot 2023-02-22 at 2 35 25 PM" src="https://user-images.githubusercontent.com/117120227/220775680-4a6abde5-1c15-4c49-95da-67f72ff0a945.png">

