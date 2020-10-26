## 7_R

> In probability theory and statistics, the marginal distribution of a subset of a collection of random variables is the probability distribution of the variables contained in the subset.  

So, the distribution of an individual random variable is call the *marginal distribution*


> Given random variables X,Y that are defined on a probability space, the *joint* probability distribution for X,Y is a probability distribution that gives the probability
that each of X,Y falls in any particular range or discrete set of values specified for that variable.  

So, *joint distributions* allow us to reason about the relationship between multiple events.  


Example: 

![Joint_Marginal](/Images/Homework3_JointMarginal.PNG)


The values of the joint distribution are in the 2×2 square;  
The values of the marginal distributions are along the right and bottom margins.  

Given two random variables X and Y, the *conditional distribution* of Y given X is the probability of Y when the value assumed by X is known.  

![Conditional](/Images/Homework3_Conditional.PNG)  

Example: 

![ExampleBelt](/Images/Homework3_ExampleBelt.PNG)  

If a randomly selected person wears no restraint, what is the probability of death?  

![ExampleBelt](/Images/Homework3_ConditionalBeltFormula.PNG)  

That is, there is a 6.25% chance of death of a randomly selected person in an automobile accident, if the person wears no restraint.  

## 8_R

Two random variables are independent if the realization of one does not affect the probability distribution of the other.  

More precisely, fixed two variables (X,Y), they are independent if and only if their joint probability can be factorized into their marginal probabilities   
=> **P(X ∩ Y) = P(X)P(Y)**

In fact their conditional distribution have all the same shape of their marginals.  



## 9_R  

There are several charts and graph that you can use, these are useful for statistics and data presentation, let's see some of these:  

**Flowchart**  

Flowcharts help organize the steps, decisions or actions in a process from beginning to end. People often use flowcharts to depict complex situations.  

**Pie Chart**

A pie chart presents the different parts of a whole. The pieces are different sizes based on how much of the whole they represent.  
People use pie charts in business presentations to demonstrate population segments, market research responses and budget allocations.  

**Histogram**

A histogram is another type of bar graph that illustrates the distribution of numeric data across categories. The height or length of each bar in the histogram shows how many entities are in each category.  

**Scatter plot**

Scatter plots use dots to depict the relationship between two different variables. The process involves plotting one variable along the horizontal axis and the other variable along the vertical axis. The resulting scatter plot demonstrates how much one variable affects the other.  

**Differences**

Charts are tables, diagrams or pictures that organize large amounts of data in a clear and concise way. People use charts to interpret current data and make predictions. Graphs, however, focus on raw data and show trends over time.  
Plot is a synonym of graph: we use graph to showing the relationship between two or more quantities, measurements or indicative numbers, in the other hand, you need to use plot
to determine significant patterns of events.




For me the heat map is the best method for representing data, as thanks to the colors it is possible to focus attention on key data.  

> A heat map (or heatmap) is a data visualization technique that shows magnitude of a phenomenon as color in two dimensions. The variation in color may be by hue or intensity, giving obvious visual cues to the reader about how the phenomenon is clustered or varies over space.  

Heatmaps provide a *visual* approach to understanding numeric values: "If a picture is worth a thousand words, a single heatmap can be worth a thousand numbers."  

As you can see in this heat map, attention is focused on high temperatures in the summer months compared to the lower ones in the other months (Sweden 1901-1917)

![HeatMap](/Images/heat-map-with-numbers.png)








Sources:

https://en.wikipedia.org/wiki/Joint_probability_distribution  
https://en.wikipedia.org/wiki/Marginal_distribution  
http://ciep.itam.mx/~rtorres/microapl/usa-elections.pdf  
https://it.wikipedia.org/wiki/Distribuzione_condizionata  
https://online.stat.psu.edu/stat414/book/export/html/717  
https://en.wikipedia.org/wiki/Heat_map  
https://mouseflow.com/blog/2018/11/the-7-advantages-of-website-heat-mapping-as-a-diagnostic-tool/#:~:text=Heatmaps%20provide%20a%20visual%20approach%20to%20understanding%20numeric%20values&text=Although%20heatmaps%20are%20just%20as,rows%20and%20columns%20of%20numbers.   
https://www.indeed.com/career-advice/career-development/types-of-graphs-and-charts#3  
https://wikidiff.com/graph/plot  
https://www.displayr.com/how-to-make-a-heatmap-in-excel/  


