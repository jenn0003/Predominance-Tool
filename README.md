# <b>Predominance Toolset</b></center>

The <b>Predominance Tool</b> prompts you to input the fields you are interested in and reports the predominant value. To run the full tool, you will need to first utilize the <b>“Calculate Gap”</b> tool which calculates the first and second highest numbers in a list of fields and outputs the gap between these two numbers. Then, the <b>“Calculate Predominance”</b> tool incorporates the gap value calculated in the first tool. The gap represents the difference between the largest value and the second largest value. The collection of these gap numbers are compared throughout the dataset in order to measure if the predominance is significant or not. The user can specify 1 of 3 options to determine significance: (1) Should the gap be larger than the mean of all gaps to be considered significant?, (2) Should the gap be greater than a specified standard deviation over the mean to be significant?, or (3) Should the percentage of the gap be greater than a user-specified value to be considered significant?

The rest of this document will address the specifics of each tool.

#### 1. The Calculate Gap Tool

This tool finds the first and second highest numbers in a list of inputted fields and outputs the gap (or difference) between these two numbers. 

![alt tag](https://cloud.githubusercontent.com/assets/10080810/7265717/33775b14-e853-11e4-87d8-a8d306b667f8.png)

The first step is to click on the manila folder to select a feature class. A list of fields should pop up in the box below. Select the fields you are interested in comparing. After, click “OK” to run the tool.

The tool adds 7 fields to your feature class. To view these fields, right click on the feature class in the Table of Contents and click “Open Attribute Table”. The following is an explanation of each of the <b>added fields</b>:

1.	<b>Dominant Component</b> (DomFName): The name of the field with the highest value.
2.	<b>Dominant Component Alias</b> (DomFAlias): The alias of the field with the highest value.
3.	<b>Dominant Value</b> (DomValue): The value of the dominant field. 
4.	<b>Margin of Dominance</b> (DomMarg): The difference between the first and second highest values.
5.	<b>% Dominance</b> (DomPerc): The percent of the total values the dominant value represents. Calculated by dividing the maximum value by the total value of all selected fields.
6.	<b>Transparency</b> (DomPerXP): The transparency of the dominant field. Calculated by subtracting the dominant percent from 100 (e.g., if the dominant field is 80% of the total values, the transparency will be 20%. If the highest value is only 30% of the total value, it will have a higher transparency of 70%.)
7.	<b># of Ties</b> (DomFCnt): The number of fields with the same value.

