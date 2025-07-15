# Applications of Machine learning

(Course created around 2020)

- AGI is Overhiped
- AI is going to create 13 trillion dollars annually by 2030

## What is machine learning?

“Field of study that gives computers the ability to learn without being explicitly programmed.” - Arthur Samuel (1959)

In the course We will see:

Machine learning algorithms

- Supervised learning (course 1,2)
    - Used the most in real word applications and had most rapid advancements 
- Unsupervised learning (course 3)
- Recommender systems (course 3)
Reinforcement learning (course 3)

Practical advice for applying learning algorithms

## Supervised Learning

SPL refers to algorithms that learn (x => y) or input to output mappings.

Learn by getting pairs of input and output and eventually learn to get the output with just the input.

![](/images/supervised-learning-regression.png)

### Regression

Regression is a type of supervised learning 

![](/images/regression-1.png)

What is regression?
The term "regression" in AI and statistics comes from its historical roots in the work of Sir Francis Galton in the late 19th century. He studied the relationship between parents' and children's heights, observing that children's heights tended to "regress" toward the average height of the population, rather than being as extreme as their parents' heights. This phenomenon, where extreme values tend to move closer to the mean in subsequent measurements, was called "regression toward the mean."

In 1886, Galton formalized this concept in his paper "Regression Towards Mediocrity in Hereditary Stature." The term "regression" stuck and was later applied to statistical methods developed to model relationships between variables, particularly by predicting a dependent variable based on one or more independent variables. These methods, like linear regression, became foundational in machine learning and AI for predicting numerical outcomes.

So, the name "regression" reflects this idea of values moving back toward a typical or average state, even though modern regression techniques are used for much broader purposes, like fitting models to data for prediction or inference. It’s less about "going backward" and more about the historical context of describing how data points relate to a central tendency.

### Classification Algorithm

Breast cancer detection

We are trying to predict only two possible different output numbers, that is why we are classifying.

In the next graph we see a classification system that classifies between benign or malignant.

![](/images/classification-1.png)

In classification the output “class” and “category” are used interchangeably.


In classification problems we can have more than two output categories.

Eg. Benign and Two types of malignant cancers.

Classification algorithms predict categories. Categories can be numbers, if a pic is cat or dog. Benign or malignant. A small number of possible outputs.


![](/images/classification-2.png)


Classification algorithms can have more than two inputs, here the classification algorithm finds a boundary to divide between malignant or benign.

![](/images/classification-3.png)

### To summarize

Supervised learning maps input(x) to output(y), where the learning algorithm learns from the right answers.

The two major types of supervised learning are regression and classification.

In a regression application, like predicting prices of houses, the learning algorithm has to predict numbers from infinitely many possible output numbers.

In classification, the learning algorithm has to make a prediction of a small set of possible outputs.

## Unsupervised Learning

In unsupervised learning we are given data which isn't asociated with any output labels (y). Say you are given data on patients age and tumor size but not whether the tumor was bening or malignant.

![](/images/unsupervised-1.png)

We are not asked to find if the tumor is bening or malignant because we are not given any labels (y) in the dataset. Instead our job is to find some structure or some pattern or just find something interesting in unlabeled data.

We call it unsupervised learning because we are not trying to supervise the algorithm to give some "right" answer to every input, instead we ask the algorithm to figure out all by itself what's interesting or what patterns or structures there might be in this data.

In this particular dataset an unsupervised learning algorithm might decide that the data can be assigned to two different groups or two different clusters. This is a type of UL called clustering, because it places the unlabel data into different clusters and turns out to be used in many applications.

![](/images/unsupervised-2.png)

For example, in Google news, from the millions of different news every day a clustering algorithm figures our which are the different clusters that day by itself.

We can have an idea of what its doing by noticing that the words panda, twin and zoo appear in all articles on that cluster. So the algorithm could be finding the articles that have similar words and grouping them into clusters.

The algorithm needs to figure out by itself which are the clusters of news articles today, that's why this cluster algorithm is a type of unsupervised learning.

### Other types of UL

Anomaly detection: Find unusual data points.

Dimensionality reduction: Compress data using fewer numbers.

We are going to see these algos later in the course.

### To summarize

A clustering algorithm which is a type of unsupervised learning algorithm takes data without labels and tries to automatically group them into clusters

- Data only comes with inputs x, but not output labels (y).
- Algorithm has to find structure in the data.