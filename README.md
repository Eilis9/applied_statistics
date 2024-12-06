# Applied Statistics Module 

## Repository Description

This repository contains the tasks and project for the Applied Statistics module of the Higher Diploma in Computing in Data Analytics at GMIT. <br>

Lecturer: Ian McLoughlin <br>
Student: Eilis Donohue (G00006088)

### Software and Packages Used

 - Python v3.12.7 
 - Jupyter Notebook 7.2.2 
 - Numpy v1.21.2
 - Scipy v1.7.3
 - Matplotlib v3.4.3
 - Pandas v1.3.3

 - Full list of all packages are given in the [requirements.txt](requirements.txt) file.
 </p>


The tasks for the module are in the workbook [tasks.ipynb](tasks.ipynb) and the project is in [project.ipynb](project.ipynb). <br> 
All commentary and references are given in the respective Jupyter Notebooks. 

### How to get started with this repository

Local download:
1. Download the repository from GitHub by clicking on the green "Code" button and selecting "Download ZIP".
2. Extract the files to a location on your computer.
3. Open the Jupyter Notebook by typing `jupyter notebook` in the command line.

Codespace:
1. Click on the green "Code" button and select "Open with Codespaces".
2. The repository will open in a Codespace in your browser.
3. Open the Jupyter Notebook by clicking on the file name in the file list.

### How to run the Jupyter Notebooks

The Jupyter Notebooks should be downloaded along with the /img and /data  folders and run locally in Jupyter notebook version 7.2.2. 
The [requirements.txt](requirements.txt) file lists the required packages to run the Jupyter Notebooks.
 - - -

## Task Descriptions

### Task 1: Permutations and Combinations

Suppose we alter the Lady Tasting Tea experiment to involve twelve cups of tea.
Six have the milk in first and the other six having tea in first.
A person claims they have the special power of being able to tell whether the tea or the milk went into a cup first upon tasting it.
You agree to accept their claim if they can tell which of the six cups in your experiment had the milk in first.

Calculate, using Python, the probability that they select the correct six cups.
Here you should assume that they have no special powers in figuring it out, that they are just guessing.
Remember to show and justify your workings in code and MarkDown cells.

Suppose, now, you are willing to accept one error.
Once they select the six cups they think had the milk in first, you will give them the benefit of the doubt should they have selected at least five of the correct cups.
Calculate the probability, assuming they have no special powers, that the person makes at most one error.

Would you accept two errors? Explain.

### Task 2: numpy's Normal Distribution

In this task you will assess whether `numpy.random.normal()` properly generates normal values.
To begin, generate a sample of one hundred thousand values using the function with mean `10.0` and standard deviation `3.0`.

Use the `scipy.stats.shapiro()` function to test whether your sample came from a normal distribution.
Explain the results and output.

Plot a histogram of your values and plot the corresponding normal distribution probability density function on top of it.

### Task 3: t-Test Calculation

Consider the following dataset containing resting heart rates for patients before and after embarking on a two-week exercise program.

| Patient ID |  0 |  1 |  2 |  3 |  4 |  5 |  6 |  7 |  8 |  9 |
|:-----------|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|
| Before     | 63 | 68 | 70 | 64 | 74 | 67 | 70 | 57 | 66 | 65 |
| After      | 64 | 64 | 68 | 64 | 73 | 70 | 72 | 54 | 61 | 63 |

Calculate the t-statistic based on this data set, using Python.
Compare it to the value given by `scipy.stats`.
Explain your work and list any sources used.

### Task 4: ANOVA

In this test we will estimate the probability of committing a type II error in specific circumstances.
To begin, create a variable called `no_type_ii` and set it to `0`.

Now use a loop to perform the following test 10,000 times.

1. Use `numpy.random.normal` to generate three samples with 100 values each. Give each a standard deviation of `0.1`. Give the first sample a mean of `4.9`, the second a mean of `5.0`, and the third a mean of `5.1`. 

2. Perform one-way anova on the three samples and add `1` to `no_type_ii` whenever a type II error occurs.

Summarize and explain your results.


## Project

In this project, you will analyze the [PlantGrowth R dataset](https://vincentarelbundock.github.io/Rdatasets/csv/datasets/PlantGrowth.csv).
You will find [a short description](https://vincentarelbundock.github.io/Rdatasets/doc/datasets/PlantGrowth.html) of it on [Vicent Arel-Bundock's Rdatasets page](https://vincentarelbundock.github.io/Rdatasets/).
The dataset contains two main variables, a treatment group and the weight of plants within those groups.

Your task is to perform t-tests and ANOVA on this dataset while describing the dataset and explaining your work.
In doing this you should:

1. Download and save the dataset to your repository.

2. Describe the data set in your notebook.

3. Describe what a t-test is, how it works, and what the assumptions are.

3. Perform a t-test to determine whether there is a significant difference between the two treatment groups `trt1` and `trt2`.

4. Perform ANOVA to determine whether there is a significant difference between the three treatment groups `ctrl`, `trt1`, and `trt2`.

5. Explain why it is more appropriate to apply ANOVA rather than several t-tests when analyzing more than two groups.



