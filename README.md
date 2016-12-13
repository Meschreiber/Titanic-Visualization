# DataVisualization
Udacity Unit on d3.js &amp; dimple.js

## Summary 
This visualization shows the demographics of 891 of the 1317 passengers aboard the Titanic. Specifically, gender, class, port of embarkment, age, and number of family members aboard were explored. There were more men than women, more third class passengers than first class, and the most common age range was between 21 - 30.  Next, survivorhsip within each of these categories was explored.  Unsurprisingly, women, children, and first class passengers were more likely to survive.

## Design 

### Dataset information
This dataset is taken from [Kaggle]( https://www.kaggle.com/c/titanic/data?train.csv#) website.  I cleaned the data by removing categories I was uninterested in (passenger name, cabin number, fare) and creating a new one which combined the number of spouses/siblings and parents/children abroad and a new one which put passengers into age "bins".

### Version 1
My inital idea is to move progressively through the data from simple to more complex. The first set of visualizations will simply show the breakdown of theses passengers in terms of gender, age, ticket class (first, second, or third class), port of embarkment, and number of family members abroad.  Second, will focus on survivorship, first by showing the total number of survivors and non survivors and then breaking down the original visualization into these categories.  Finally, the visualization will show each of these categories as percentages rather than raw numbers.  In the future, I would like users to be able to select certain demographics (First class, single, female, in her 20s, embarked in Southampton) and see what the survival rate for that particular demographic is.

### Version 2 (based on feedback #1 and #2)
I added a written explanation of "unknown" categorie" and also labeled the unknown category in the age graph. Additionally, I will make graphical changes such as increase the axes label font size and changing the positioning of the hover tool tip.  I also added additional visualizations to the conclusion that explore how class plays a role in family size and port of embarkment.

## Feedback 
### Feedback #1:
> What do you notice in the visualization?

Graphs are presented in a simple and straightforward manner that affords easy and quick interpretation. The two-color scheme of bar graphs offers simplicity and dissuades potential distraction in understanding and interpreting data.

The titles of each graph, e.g., Gender Breakdown, Class Breakdown, etc.  are clearly presented (large size font).  It would help in visualizing data if font size of Y and X axis labels are also enlarged. 

> What questions do you have about the data?

1.	In the Age/Survivor Breakdown graph, the last graph is not labeled. Is this for another age category – 81 -?
2.	Why is there a category “Unknown” in the graph on “Port Survivor %”?  If there’s a reason for including this category, it’s not clear to me .  
3.	The placement of the label “Port of Embarkment” is not on the same line as the titles of other categories, i.e., Gender and Ticket Class.
4.	 Due to large numbers of third class passengers and those who embarked from Southampton, could these categories potentially skew the relationships on survivorship drawn from the data? 
5.	There are no survivors among those with number of family members 7 and 10. Is there a possible explanation on why this is so?  
6.	Is there historic evidence that first class passengers were given priority? If so, would it explain this category’s high rate of survivorship?

> What relationships do you notice?

Percent of survivorship is greater among women (than men) and children (than older passengers). Writer noted that these trends are supported by historic evidence that women and children were given priority in being allowed to go to life boats.

> What do you think is the main takeaway from this visualization?

The main takeaway is that graphs are an excellent tool in presentation of data. When graphs are presented in a simple and straightforward design, data are more easily understood. 

> Is there something you don’t understand in the graphic?

No. Graphic is excellent and allowed easier understanding of data.

### Feedback #3:
> What do you notice in the visualization?
The visualization displays information about the Titanic passengers in a very clear format.  The progression from frequency, to survivorship and then to relative frequency helps illustrate arguments regarding likelihood of survival more clearly.  For example, looking at survivorship of children younger than 11 years old it is hard to tell that the majority of them survived.  I also have noticed that it is hard to pinpoint the exact value the bars represent, but there is a convenient tool that allows me to see which y-value it corresponds with.  I also noticed a few mistakes / inconsistencies in the graphs for Gender/Survivor breakdown and Age survivor breakdown and %.
 
> What questions do you have about the data?
I would be interested in knowing the greatest determinant of survival on the Titanic and why Southhampton had a much larger relative frequency of deaths (did they have the most 3rd class passengers maybe?).

> What relationships do you notice?
I notice that a greater percentage of women and children survived as compared to men.  I noticed that a greater percentage of first and second class passengers survived as compared to third class passengers.  I noticed that there were a lot more men on the ship than women (why is this true?).  I also noticed that, outside of being younger than 11, there was no distinct advantage for any particular age group in terms of survival.  I agree with the author's claim that the data shows that women and children were given priority for fleeing the ship.

> What do you think is the main takeaway from this visualization?
The main take away for me is that third class passengers were much less likely to have survived the accident than first class passengers.  
 
> Is there something you don’t understand in the graphic?
The graphics are very clear and easy to read.  There are just some small errors:  
1. the Gender/Survivor breakdown graph, why are the colors switched for perished and survived as compared to the others? 
2. the Age survivor breakdown and % there is a category missing, is this the category for unknown age?

## Resources 
(Listed in order of usage)

- Titanic Wikipedia Entry https://en.wikipedia.org/wiki/RMS_Titanic
- Titanic Facts http://www.titanicfacts.net/titanic-passengers.html
- Dimple.js documentation http://dimplejs.org/examples_index.html
- Udacity Forum Discussion https://discussions.udacity.com/t/beginner-help-with-dimple-js-and-javascript-in-general/203196
- Udacity Forum Discussion https://discussions.udacity.com/t/project-6-feedback-and-help-request-titanic-data/198669
- Vverde's repository https://github.com/vverde/Udacity-Data-Analyst-Nanodegree-P6
- Stack Overflow Exchange http://stackoverflow.com/questions/17791926/how-to-rotate-x-axis-text-in-dimple-js
- Stack Overflow Exchange http://stackoverflow.com/questions/33179439/d3-js-dimple-getting-a-title-on-a-graph
- Dimple Wiki on Github https://github.com/PMSI-AlignAlytics/dimple/wiki/dimple.series#addOrderRule
