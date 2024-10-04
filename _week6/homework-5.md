# Homework 5:  From Humanities Datasets to Research Questions

So far we've learned how to think about datasets in all of their rich contexts, how turn sources into datasets, and how to collect data by hand. We've also learned the basics of Python commands, Jupyter notebooks (a file format for sharing Python code), and Pandas (a specific Python library for analyzing tabular data).

In this week's homework, we're going to put some of this together and practice turning specific research questions into hunches that we can test out using what we've learned so far in pandas. 

In Part I, working with a single dataset, we're going to translate some research questions into the concrete analytical tasks (measure, count, analyze) that we would want to perform with the assistance of simple Python commands. 

In Part II, we'll look at some existing, off-the shelf browser-based tools designed by humanities scholars for exploring textual data.


## Part 1: From exploratory data analysis in Python to a research hypothesis

For Part 1, we're going to be working with the film dialogue dataset behind *The Pudding'*s 2017 article, ["Film Dialogue from 2,000 screenplays, Broken Down by Gender and Age"](https://pudding.cool/2017/03/film-dialogue/)

Read up on background behind the choices in the "Film Dialogue, By Gender" project here: [https://medium.com/@matthew_daniels/faq-for-the-film-dialogue-by-gender-project-40078209f751](https://medium.com/@matthew_daniels/faq-for-the-film-dialogue-by-gender-project-40078209f751)



### 1.1 Getting set up

Take a few minutes to refresh yourself with the following questions (**no need to record your answers, this is just for you**)

- Jupyter notebooks
	- How do we make a Jupyter notebook? open it? rename it? save it? how do we import Pandas?
- Pandas
	- How do we read in a csv? what is a dataframe? what is a column (or "series")"? how do we select columns and rows? create new ones? How do we select only rows which contain a certain value in a given column?
	- How do we sort data? how do we filter data?  how can we aggregate data?

If it helps, look back at the sequence of our lessons on these topics on the [resources page](https://sceckert.github.io/Data-and-Culture-Fall-2024/resources)

1. Download the three datasets from [this zip file](https://github.com/sceckert/Data-and-Culture-Fall-2024/blob/main/_datasets/pudding-film-dialogue-data.zip?raw=true). These scripts are from Matt Daniels's [Github repo](https://github.com/matthewfdaniels/scripts/). Take a look inside the documentation files to see what each contain
2. Launch Anaconda Navigator, Launch JupyterLabs and create a new Jupyter notebook  OR open this Google Colab notebooks and click "File" -- > "Save a copy in Drive""
3. Read in each of the CSV files as a dataframe. This particular *Pudding* data has a slightly different encoding, so make sure to specify `encoding = "ISO-8859-1")` when you load them in, like so: `df = pd.read_csv('path/to/the/file/', encoding='ISO-8859-1`).  In Colab, the files are already uploaded, and the file path will start"" Data-and-Culture-Fall-2024//_datasets/pudding-film-dialogue-data/[name-of-each-file]"
	- You should create THREE separate pandas DataFrames, one for the character_list data, one for the character_mapping data, and one for the public_scripts data.
4. Once you've loaded in each CSV, and created each DataFrame take a look at what you find in each of them. See if there is any missing data, what kinds of data is present in each, what kind of values appear, what are their ranges and distributions, etc. 

NOTE: THIS IS THE END OF WHAT YOU WRITE in PYTHON.

### 1.2 Planning how to translate research questions into specific computational tasks (eg specific things to measure, count, explore, visualize, and model)

These datasets were originally created for a specific set of research questions about gender and dialogue in films, but there's enough data here that we could think about other research questions we could ask.

***Write down some thoughts in plain English (no need for actual Python commands)** describing in lay terms what you might do answer the following questions (If you want, you can try to take a stab at outlining what kinds of Python commands you might use, but the goal here is to describe what each step is doing): 

1. How could we tell if the total amount of dialogue (by gender breakdown and total) in a given movie, was increasing over time in our movies dataset? How might this influence the assessment about the breakdown of gender dialogue?
2. How could you test if there was any relationship between the film's gross value and the amount of dialogue in the film?
3. How would you visualize one of the research questions above? What variables would we plot and how? (Again, in plain English, not Python)
4. What do you *hypothesize* your visualization would look like? 

Then, think about:

1. What other research questions would *you* want to explore in this dataset?
2. How could you turn one research questions into concrete computational tasks––what might be some steps you would need to take in order to pursue your question?

**Again, remember that all of the questions above should be prose descriptions**: We will *complete* the Python portion together on 10/16.


## Part II: Developing research questions with off-the-shelf humanities tools

So far, we've been spending most of our time in Python and Jupyter notebooks. It's a handy language that's able to handle any of the formats for your data: the benefits of Python is that you have a lot of flexibility and control over what dataset you use. But there are other tools that allow you to analyze a collection of texts or a collection of metadata.

Choose one of the following 4 tools–– Corpus Linguistics in Context (CLiC), EarlyPrint Lab, Voyant Tools, Bookworm/ Bookworm Playground –– to explore. You'll be able to use them in your web-browser, no downloading required. Try exploring the existing data, or uploading your own. Think about what kinds of questions the tool might enable and the limitations. **Then write up a set of short responses to the following questions**:

1. What is a specific research question that you would want to explore with your chosen tool? 
2. What steps might you take to begin exploring that question?

Tools to choose from (choose ONE):

+ [**Corpus Linguistics in Context (CLiC)**](https://clic.bham.ac.uk/): a project originally created for analyzing patterns in direct speech, narration, and speech tags, which now features full text for several small sample collections of 19th-century British novels, 19th-century African American novels, and 19th-century children's literature.
	+ [Quick Start Guide](https://blog.bham.ac.uk/clic-dickens/2022/06/15/clic-quick-start-guide/)
	+ [Additional Background](https://clic.readthedocs.io/en/2.1/clicanalysis.html)
	+ Texts [currently available to work with in CLiC](https://github.com/mahlberg-lab/corpora/blob/master/INDEX.pdf)
+ [**EarlyPrint Lab**](https://earlyprint.org/lab/): a toolkit for interacting with the EarlyPrint project's existing collection of early English print from 1473 to the early 1700s. The lab contains 4 tools for searching and 4 for visualizing patterns within the database.
	+ [EarlyPrint Lab](https://earlyprint.org/lab/)
	+ [Tutorials and How-To](https://earlyprint.org/how-to/)
	+ There's also a Python set of tools in a nifty [set of Jupyter notebooks](https://earlyprint.org/jupyterbook/intro.html)
+ [**Voyant Tools**](https://voyant-tools.org/): a dashboard for uploading your own collection of either plain text or XML files. The dashboard includes two demo collections: Project Gutenberg versions of Jane Austen's novels and Williams Shakespeare's plays, but the tool can be used with any plain text collection (or even on single texts).
	+ My [quick tutorial](https://github.com/sceckert/Data-and-Culture-Fall-2024/tree/main/_week6/Eckert-Text-Analysis-Introduction-to-Voyant.pdf) using the demo Austen novels corpus (1790-1818) and our corpus of U.S. Inaugural Addresses (1789-2021)
	+ [User Guide](https://voyant-tools.org/docs/#!/guide/start)
	+ List of [tools to customize in Voyant dashboard](https://voyant-tools.org/docs/#!/guide/tools)
+ [**HathiTrust's Bookworm**](https://bookworm.htrc.illinois.edu/develop/) and the [**Bookworm Playground**](https://bookworm.htrc.illinois.edu/app/): are two related toolkits for interacting with HathiTrust's collection of 18+ million digitized copies of texts held in member libraries. (For work published before 1929, these texts are fully available, for texts after 1929, only the metadata is publicly accessible) . For an overview of what's actually in HathiTrust, scroll through this [interactive visualization](https://creatingdata.us/datasets/hathi-features/) by Ben Schmidt to get a sense of what's in HathiTrust. HathiTrust Bookworm is little like GoogleBooks Ngram Viewer, with many more ways of moving from the distant overview of the visualization to particular titles. The Bookworm Playground offers other
	+ [Bookworm Line Chart](https://bookworm.htrc.illinois.edu/develop/)
	+ [Bookworm Playground](https://bookworm.htrc.illinois.edu/app/)
	+ Short [overview of how to use "BookWorm"](https://htrc.atlassian.net/wiki/spaces/COM/pages/43295225/HathiTrust+Bookworm+step-by-step+tutorial) 
