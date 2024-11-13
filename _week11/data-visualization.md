## Introduction to Data Visualization

# Introduction to Data Visualization

In today's tutorial, we're going to go over some familiar forms of data visualization using some new and familiar datasets. As we do so, we'll also think about how different techniques in data visualization can be used iteratively as part of your exploratory analysis. (You might consider rendering the same data 3 different ways!)

### Basic data visualization

+ Example 1: [Making a line plot](#scrollTo=6fWu_GQeQJEp)
    + Dataset: At the Circulating Library, 1837-1901
+ Example 2: [Making simple bar and pie charts](#scrollTo=APZYKu1UQJEw)
    + Dataset: Modernist Journals Project

### Advanced data visualization

+ Example 3: [Make stacked bar chart](#scrollTo=gf2-bS5TQJEz)
    + Dataset: Modernist Journals Project
+ Example 4: [Make an interactive visualization](#scrollTo=UdprD16kQJE2) 
    + Dataset: Modernist Journals Project
+ Example 5: [Save an interactive visualization to an HTML file](#scrollTo=bwCBHYaWQJE2) 
    + Dataset: Modernist Journals Project
+ Example 6: [Make an interactive scatterplot visualization](#scrollTo=CLumOo-hQJE3)
    + Dataset: Seattle Public Library Circulation Data, 2010-2015
+ Example 7: [Make a Gantt chart to visualize sequential data](#scrollTo=clSgi2WqQJE4)
    + Dataset: Columbia University Literature Humanities Syllabus Texts: 1937-2020
+ Example 8: [Make a map from a list of place names](#scrollTo=nTisDrstQJE5)
    + Dataset: Place names generated from performing Named Entity Recognition on *The Adventures of Sherlock Holmes* (1892)

### Off-the-Shelf Data Visualization

+ Example 9: [Make a visualizations of distinctive and shared vocabulary between two texts using SameDiff](#scrollTo=IzWBsmVibkUP)
    + Dataset: Gertrude Stein's "Matisse" and "Picasso"; other text corpora of your choice
+ Example 10: Make a bump chart of patterns in netflix genre
    + Dataset: Netflix Original Series 2013-2017;  other tabular data of your choice


## Ex 9: Make a visualizations of distinctive and shared vocabulary between two texts using SameDiff

+ Navigate to DataBasic's SameDiff tool: https://databasic.io/en/samediff/
+ Compare some of the default text corpora (eg. Beyoncé's lyrics and Aretha Franklin's lyrics). Scroll to the bottom. 
    + What kind of output do you get? How might
    + Scroll to the bottom and click to download the full results as a CSV (scroll to the bottom of SameDiff). Open it up. What kind of information do you have? How else might you try and represent this dat?
+ Then click the "upload texts" and upload the following sets of texts:
    + Stein's "Matisse" and Stein "Picasso" (in [week 2 texts](https://github.com/sceckert/Data-and-Culture-Fall-2024/tree/main/_week2))
    + A collected edition of Christina Rossetti's poems (published 1876) with the three 19th-centuy editions of Emily Dickinson's poems, published posthumously (in [week 11 texts](https://github.com/sceckert/Data-and-Culture-Fall-2024/tree/main/_week11))
    + Two textual corpora of your choice!
+ For each, explore the visual output. 
+ Explore other DataBasic visualization tools like [WordCounter](https://databasic.io/en/wordcounter/)



## Ex 10: Make a BumpChart of Netflix genres over time using RawGraphs

+ Go to RawGraphs (https://app.rawgraphs.io/), a web-browser based tool for data visualization 
    + Click "Try our data samples"
    + Select the Sample Netflix Original Series 2013-2017 dataset
    + Select "BumpChart"
    + Add the Premiere Year to X Axis and "Genre" to "Streams"
    + Then try changing from "Genre" to "Subgenre"
    + What do you notice?
    + Try experimenting with other formats and settings
    + Download your visualization at the bottom
+ Then try with an alternate tabular dataset of your your choice that includes temporal data (maybe the Seattle Checkouts? Poe data?) 


