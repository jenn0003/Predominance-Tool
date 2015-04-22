# <b>Predominance Toolset</b></center>

The <b>Predominance Tool</b> prompts you to input the fields you are interested in and reports the predominant value. To run the full tool, you will need to first utilize the <b>“Calculate Gap”</b> tool which calculates the first and second highest numbers in a list of fields and outputs the gap between these two numbers. Then, the <b>“Calculate Predominance”</b> tool incorporates the gap value calculated in the first tool. The gap represents the difference between the largest value and the second largest value. The collection of these gap numbers are compared throughout the dataset in order to measure if the predominance is significant or not. The user can specify 1 of 3 options to determine significance: (1) Should the gap be larger than the mean of all gaps to be considered significant?, (2) Should the gap be greater than a specified standard deviation over the mean to be significant?, or (3) Should the percentage of the gap be greater than a user-specified value to be considered significant?

The rest of this document will address the specifics of each tool.

#### 1. The Calculate Gap Tool

This tool finds the first and second highest numbers in a list of inputted fields and outputs the gap (or difference) between these two numbers. 


