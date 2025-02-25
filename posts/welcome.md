---
title: "Introduction to SciPy"
description: "Introduction Post"
author: "Shreya Anbu"
date: "2/25/2025"
---


# **Introduction to SciPy**

# scipy.stats Module

It is a very helpful module used for statistical analysis and modeling.

> This module contains a large number of probability distributions, summary and frequency statistics, correlation functions and statistical tests, masked statistics, kernel density estimation, quasi-Monte Carlo functionality, and more.

You can find more information on the [official documentation page](https://docs.scipy.org/doc/scipy/reference/stats.html).

# Installation

If you already have Python installed, you can install SciPy with pip by executing the following in a terminal/shell:

```python
python -m pip install scipy
```

While using Jupyter Notebook or Google Colab, just use the following line before writing the main code:

```python
import scipy
```

# Comparison with PyTorch Distributions

Can't both of these modules used for modeling distributions? Why do they exist as two separate models then? <br>
PyTorch module provides more functionality for deep learning applications, whereas SciPy is more suitable for statistical modeling, having a more user-friendly interface for statisticians.

| Feature | PyTorch Version| ScipPy Version |
|-------|-----|-----|
| Creating a Distribution | torch.distributions.Poisson(rate_param)  |scipy.stats.poisson(rate_param)|
| Creating a Sample | dist.sample((n, ))  |dist.rvs(size = n)|
| Calculating PMF | dist.log_prob(x).exp()  |dist.pmf(x)|

We can see with the last comparison how SciPy has more direct, easy to read functions for obtaining basic values out of a distribution.

# Different Kinds of Distributions Available

There are a lot of things contained by the scipy.stats module, but we will be looking into the different kinds of distributions available for us to use. There are three kinds: **continuous**, **discrete** and **multivariate**. <br>


*   **Continuous Distribution:** Random variable can take on any value within a specified range, meaning there are infinitely many possible values between any two points;

*   **Discrete Distribution:** Random variable can only take on a finite number of distinct values, usually whole numbers;

*  **Multivariate Distribution:** Describes the probability of multiple random variables occurring simultaneously, considering their potential relationships and correlations with each other.

There are tons of distributions available under each kind that we can use, which can be explored again in the [official documentation](https://docs.scipy.org/doc/scipy/reference/stats.html).

![Screenshot from official documentation](https://gist.github.com/user-attachments/assets/b3db29a9-bc79-4164-9f4b-969c0c3fa23b)

The above image shows the start of the list of functionalities, which barely scratches the surface.
