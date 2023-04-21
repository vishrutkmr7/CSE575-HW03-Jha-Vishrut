CSE575 HW03, Thursday, 11/10/2022, Due: Wednesday, 11/30/2022
Please note that you have to typeset your assignment using either LATEX or Microsoft
Word, and produce a PDF file for submission. Hand-written assignment (or photo of
it) will not be graded. You need to submit a zip file for this assignment which
contains: 1) a PDF file containing the solution/report of this assignment; 2) all of
your implementation code. You should name your zip file CSE575-HW03-
LastName-FirstName.zip. The zip file should be able to unzip into a folder named
CSE575-HW03-LastName-FirstName.

1 Handwritten Digits Recognition with k-NN [30 pts]
In this problem, you need to implement the 𝒌-NN algorithm for MNIST handwritten digits recognition.
The data set is included in the “MNIST” folder of this assignment, which contains training set images,
training set labels, test set images, and test set labels. Please find an introduction to the MNIST data in
“MNIST.html” in the same folder.
You need to implement the algorithm from scratch using either MATLAB or Python, and to predict
the digits in the test set. You will use the Euclidean distance to measure the distance between each
pair of data points.
• For each value of 𝑘 = 1, 3, 5, 10, 20, 30, 40, 50, 60, compute the prediction accuracy. Plot the
accuracy vs the value of 𝑘.
• Write out your observations from the obtained results.
Write the observations and explanations of the result from the figure into your report (PDF) file,
and include your implementation in the zip file.
2 K-Means Clustering [30 pts]
In this problem, you will implement the K-means algorithm for clustering. You should implement from
scratch, using either MATLAB or Python. Download the data set from Canvas. The data set contains 128
data points, each has 13 features. If you encounter missing values in the dataset, replace the missing
entry with the mean of that feature. You should run your implementation with 𝑲 = 𝟐, 𝟑, . . . , 𝟗. For
each run, initialize the cluster centers randomly among the given data, and terminate the iteration if
the cluster assignment of all data points remains unchanged (in other words, each data point will be
assigned to the same cluster if running more iterations). You could use slide 14 of Lecture17 as the
reference for implementation.
• Plot the objective function as a function of 𝐾.
• For 𝐾 = 2, plot the points using its first two features. Use two different colors or symbols to
distinguish the two clusters.
• Write out your observations from the obtained results.
Write the observations and explanations of the result from the figure into your report (PDF) file, and
include your implementation in the zip file.
3 Gaussian Mixture Model (GMM) [40 pts]
In this problem, you will implement the Gaussian Mixture Model (or Mixture of Gaussians). You should
implement from scratch, using either MATLAB or Python. Use the same dataset as in the previous
problem. You should run your implementation with 𝑲 = 𝟐, and run until convergence. You can choose
to terminate the iteration when the change of the log-likelihood, computed by equation (9.28) on page
439 of the textbook, is smaller than a small threshold (such as 1e-5). Please use the EM algorithm on
page 438 and page 439 of the textbook as the reference for implementation, and you could use the
code in “init_gmm.m” on Canvas for initializing parameters of GMM.
• For 𝐾 = 2, plot the points using its first two features. Use two different colors or symbols to
distinguish the two clusters. The cluster assignment is determined by the posterior 𝛾(𝑧𝑛𝑘)
computed by equation (9.23) of the textbook. A data point 𝑥𝑛 is assigned to cluster 1 if 𝛾(𝑧𝑛1) >
𝛾(𝑧𝑛2), and it is assigned to cluster 2 otherwise.
• Write out your observations from the obtained results.
Write the observations and explanations of the result from the figure into your report (PDF) file, and
include your implementation in the zip file.
