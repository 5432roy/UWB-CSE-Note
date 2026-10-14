# CSS 581 - Machine Learning: Assignment 1

Machine Learning Foundations

Total points: 50

Student: Shang-Yu Chan

## Problem 1: Data Objects and Attributes [5 points]

Give a concrete example of a data object in the real world. Think about its attributes or features and list all the attributes you can identify. A clear drawing of a simple table is encouraged.

Stock price.
- daily high/low
- trading volume
- RSI

## Problem 2: Recognizing Machine Learning Problems [5 points]

Briefly justify each answer in one or two sentences.

(a) You have developed an algorithm to automatically and efficiently retrieve addresses and phone numbers from a very large database using a person’s name as the search key. Is this machine learning? Why or why not?

I don't think this algorithm is considered machine learning, but more like a dictionary lookup algorithm. The behavior to retrieve data with a given key is fully specified by handwritten rules instead of learned from data.

(b) You have developed an algorithm to automatically and efficiently retrieve all images similar to a query image from a very large image database. The results could be ranked by similarity scores or probabilities. Is this machine learning? Why or why not?

It depends how the algorithm determine the similarity scores. If different traning data set or different training process can affect how the algorithm calculate the similarity scores, it is machine learning. On the other hand, a algorithm like calculating and sum the Euclidean pixel distance to rank the similarity will not be machine learning. 

## Problem 3: Selecting an Appropriate Learning Task [10 points]

For each scenario, state which type of machine learning is most appropriate: *classification*, *regression*, *clustering*, or *association rule analysis*. Briefly justify each answer in one or two sentences. Each part is worth 2.5 points.

(a) You are the manager of a local Safeway store. Sales data indicate that customers who buy onions and potatoes together are also likely to buy hamburger meat. You want to benefit from this pattern through promotional pricing or product placement.

Association rule analysis, because we are trying to find out co-occurrence relationships among items. Not regress because we are not trying to predict a continuous value, such as how many ponds of hamburger meat will be bought.

(b) A dietician is trying to understand how people’s dietary choices affect the amount of weight they gain or lose, but no obvious patterns are apparent. For a recent six-month period, the dietician has records for 150 clients describing their consumption of 12 different foods and the change in their weight over that period.

Regression, becuase we want to find out the continous value between relationship.

(c) You and a friend disagree about how many social groups exist at your school. You believe there are approximately half a dozen natural groups based on preferences for music, clothing, athletics, and politics, while your friend believes everyone’s preferences are random. You can access publicly available records from a poll in which 1,000 students scored their preferences for 20 forms of art and entertainment.

Clustering

(d) You work at an oil company that wants to predict whether wells drilled in several new formations will produce oil. You are given a large collection of data from past drilling efforts, including geographic location, well depth, rock type, formation age, and the success or failure of each drilled well.

Classification. With a job to output discrete decisions (yes/no), it is classification.

## Problem 4: A Machine Learning Opportunity [4 points]

Describe a situation in your life where machine learning might be beneficial. For example, this could be something you encounter at work, at school, or on the internet, such as a social networking site. Explain the problem to be solved, the data or information you might collect, and the type of machine learning you think is applicable. There is not necessarily a single correct answer; the purpose is to begin recognizing opportunities to apply machine learning.

## Problem 5: Term Project Proposal [6 points]

Answer each of the following questions. Each part is worth 2 points.

(a) Which dataset and problem are you planning to study for the term project? Why are you interested in this problem?

(b) What useful information, knowledge, or patterns do you expect to discover from that dataset?

(c) Why do you think your work will be valuable? Describe a potential future application of your work or identify its potential customers.

## Problem 6: Linear Algebra Warm-up [12 points]

Determine by hand the eigenvalues and eigenvectors associated with the matrix below. Show every step of your derivation from first principles.

$$
A = \begin{bmatrix}
3 & 1 & 6 \\
2 & 1 & 0 \\
-1 & 0 & -3
\end{bmatrix}.
$$

## Problem 7: Programming Warm-up [8 points]

Calculate from scratch, using the Python programming language, the eigenvalues and eigenvectors associated with the covariance matrix below. Show your source code and include a screenshot of the results.

$$
\mathrm{cov} = \begin{bmatrix}
0.61655556 & 0.61544444 \\
0.61544444 & 0.71655556
\end{bmatrix}.
$$
