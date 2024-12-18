## In-class practicum: topic modeling collections of texts

As part of preparation for today, you read through a [tutorial on how to use Python (and Pandas) to topic model in a Jupyter notebook.](https://colab.research.google.com/drive/1i5W4X8qqXrRcXD55cYAoj_YDQaGxiBeY?usp=sharing) 

But there are also browser-based methods for using topic modeling to model a collection of texts. We're going to try two different methods using an off-the-shelf tool that allows us to run topic models on different collections of texts.  

## Part 1: Topic modeling State of the Union Addresses (1914-2009)

David Mimno, a professor of information sciences at Cornell and one of the authors of the first topic modeling algorithm, made a browser-based tool for topic modeling small corpora of texts. Read a little about [how the tool works here](https://mimno.infosci.cornell.edu/jsLDA/index.html). It has a default corpus of US State of the Union speeches (1914-2009), broken up by paragraph.

With a partner:

1. Navigate to the topic model web-browser: https://mimno.infosci.cornell.edu/jsLDA/jslda.html
2. Click "Run 50 iterations" several times, (until you've run around 200 iterations).
3. What do you notice? Try running another 50 iterations. How did it affect the composition of topics?
6. Try clicking on "topic" (listed to the left), the center column will populate with paragraphs from U.S. State of the Union Speeches.
7. Try running more iterations. 
5. Try changing the number of topics ––in the upper right-hand corner and then running more iterations).
8. Try exploring the "Topic Correlations" and "Time Series" buttons. Also try clicking on the "Download" button to see what format you can download the modeling data.


## Part 2: Topic modeling detective fiction (1890-1920)

You can also upload your own corpus and stoplist (that's a plain text file with a list of very frequently used words that you want the model to ignore). (Read Mimno's [description in "Upload your own documents"](https://mimno.infosci.cornell.edu/jsLDA/) about how documents need to be formatted in order to upload)

1. Navigate to week 10 of our course files:  
2. Download the `detective-fiction.tsv` or `doyle-fiction.tsv`and `stopwords.txt` filesby right-clicking on each file and "Saving link as.." to somewhere on your desktop. 
    - Note: `detective-fiction.tsv` is a tab-separated values file with the Story ID, date, and full text of each of the detective stories in the [Birth of the Modern Detective Story Dataset](https://github.com/ahmmnd/BMDS/tree/main?tab=readme-ov-file#the-birth-of-the-modern-detective-story-bmds-dataset); `doyle-fiction.tsv` is a subset of that corpus for just Arthur Conan Doyle Fiction. The file `stopwords.txt` is a standard list of stopwords. 
4. Navigate back to the topic model web-browser: https://mimno.infosci.cornell.edu/jsLDA/jslda.html  and in the "Use a different colleciton" box upload either `detective-fiction.tsv` or `doyle-fiction.tsv` for "Documents" and "stopwords.txt" for "Stoplist"
5. Then, try steps 2-8 from part 1 on this corpus. What do you notice?
6. Right now in our corpus, each "document" is the full text of a story in the BMDS corpus. How our model might be different if we broke up each story by paragraph?
7. What are the possible uses of LDA? What are its limits? When could you see yourself using it? 


