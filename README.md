# Predicting a document/article topic using the LDA_model

The "articles" directory contains links to all used articles for the experiment and a .txt files with the articles for each topic, split by a new line.

After text preprocessing, the most common words for each document were kept, as a strategy to get more "overlaps" or common words between the documents which share the same topic. 

I trained an LDA model for 5000 iterations and traced the predicted topics.

Here are some visualizations of variable convergence during the training process:

- **theta = topic distribution per-document**

![image](/images/theta.jpg)

- **phi = word distribution per-topic**

![image](/images/phi.jpg)

- **z = topic value**

![image](/images/z.jpg)


I was able to calculate the topic similarity between 2 documents. Some documents might contain elements of different topics other than their own. I calculated the number of most common word overlaps, this time increasing the number of most common words, and then divided by the number of most common words to get the similarity. I also tried the Blei Lafferty method (see Notebook).
