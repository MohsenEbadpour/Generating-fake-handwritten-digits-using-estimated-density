# Generating fake handwritten digits using estimated density
This repository contains code for a problem related to image estimating density in pattern recognition. The problem involves compress images, estimate density, then generate fake handwritten digits.

## Course Information

This problem is related to a *Statistical Pattern Recognition* course taught by Professor Mohammad Rahmati (<rahmati@aut.ac.ir>) in the Computer Engineering department at Amirkabir University of Technology (AUT) in Tehran, Iran. The course was offered in the Fall of 2021.

## Problem Description
In this problem, the goal was to generate fake images of digits using generative models. The dataset provided contained 1700 images of size 7×7, each depicting a handwritten digit. Here are the steps taken to accomplish the task:

a. PCA was applied to the dataset to reduce its dimensionality to 15. The values of each 15 eigenvectors were specified.

b. The best value for the bandwidth parameter was found by following a procedure which involved using the KDE (kernel density estimation) algorithm on a range of bandwidth values and comparing the estimated density function to the original dataset. The bandwidth value which resulted in the best match was selected.

c. 20 random samples were generated from the estimated density of the data using the selected bandwidth value. These samples were then converted into 7×7 images and displayed.

d. The same process was repeated without the dimensionality reduction step, and the results were compared to those obtained in step c.

![Output](/output.png)


## Repository Contents

The repository contains Python code for the problem described above, as well as a Jupyter notebook that explains the problem and provides a step-by-step cells for running the code.

## Feedback

If you have any feedback or suggestions for improving this code, please feel free to open an issue in the repository as well as send an email to Mohsen Ebadpour (<m.ebadpour@aut.ac.ir> , <mohsenebadpour@outlook.com>).


