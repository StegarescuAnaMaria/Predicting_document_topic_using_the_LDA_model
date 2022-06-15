# Predicting a document/article topic using the LDA_model

The "articles" directory contains links to all used articles for the experiment and a .txt files with the articles for each topic, split by a new line.

After text preprocessing, the most common words for each document were kept, as a strategy to get more "overlaps" or common words between the documents which share the same topic. 

I trained an LDA model for 5000 iterations and traced the predicted topics.

here are some visualizations of variable convergence during the training process:

![image](/images/theta.png)

<img src="/images/theta.png" align="left" height="48" width="48" >

theta = topic distribution per-document

![image](https://user-images.githubusercontent.com/48885998/173806569-34b31fa0-e8d5-43d7-8b72-9ca3faa61f2c.png)

phi = word distribution per-topic

![image](https://user-images.githubusercontent.com/48885998/173806666-5f095d3e-48c7-4cc1-8644-d5be5d29c655.png)

z = topic value
