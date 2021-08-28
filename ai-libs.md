# AI Libraries

Reference:

- [1] [Top Programming Languages for AI Engineers in 2021](https://towardsdatascience.com/top-programming-languages-for-ai-engineers-in-2020-33a9f16a80b0) by Towards Data Science
- [2] [Top AI Programming Languages in 2021](https://pixelplex.io/blog/top-ai-programming-languages/) by Pixelplex

Each AI programming language has its own perks that make it better for some applications and less appropriate for others. Python, Java, R, Julia, and C++ are currently leading the list of the top used tools for development.[2]

## Python

AI libraries for Python from [1]:

- *TensorFlow*, for machine learning workloads and working with datasets
- *scikit-learn*, for training machine learning models
- *PyTorch*, for computer vision and natural language processing
- *Keras*, as the code interface for highly complex mathematical calculations and operations
- *SparkMLlib*, like Apache Spark’s Machine Learning library, making machine learning easy for everyone with tools like algorithms and utilities
- *MXNet*, as another one of Apache’s library for easing deep learning workflows
- *Theano*, as the library for defining, optimizing and evaluating mathematical expressions
- *Pybrain*, for powerful machine learning algorithms

AI libraries for Python from [2]:

- TensorFlow
- Scikit-Learn
- Keras
- Pandas
- matplotlib
- PyTorch

## Java

AI libraries for Java from [1]:

- *TensorFlow*: TensorFlow’s list of supported programming languages also includes Java with an API. The support isn’t as feature-rich as other fully supported languages, but it’s there and is being improved at a rapid pace.
- *Deep Java Library*: Built by Amazon to create and deploy deep learning abilities using Java.
- *Kubeflow*: Kubeflow facilitates easy deployment and management of Machine Learning stacks on Kubernetes, providing ready to use ML solutions.
- *OpenNLP*: Apache’s OpenNLP is a machine learning tool for natural language processing.
- *Java Machine Learning Library*: Java-ML provides developers with several machine learning algorithms.
- *Neuroph*: Neuroph makes designing neural networks using the open-source framework of Java possible with the help of Neuroph GUI.

AI libraries for Java from [2]:

- Weka
- Java-ML
- H2O
- DeepLearning4j
- MOA

## R

AI libraries for R from [1]:

- *Gmodels*: provides a collection of several tools for model fitting
- *Tm*: as a framework for text mining applications
- *RODBC*: as an ODBC interface for R
- *OneR*: for implementing One Rule Machine Learning classification algorithm, useful for machine learning models

AI libraries for R from [2]

- *Gmodels*: a collection of tools for fitting models
- *Tm*: a framework for text mining applications
- *RODBC*: an open database connectivity interface for R
- *OneR*: a framework for implementing one rule classification algorithms

*Cons*: R is not easy to learn. It is slow and suffers from security issues.[2]

## C++

- TensorFlow
- Convolutional Architecture for Fast Feature Embedding (Caffe)
- CNTK
- mlpack
- DyNet
- Shogun
- FANN

## Lisp

AI libraries for Lisp from [2]:

- CLML
- mgl
- Antik
- mgl-mat
- LLA

*Cons*: highly complex and not very easy to read.[2]

The most famous Lisp dialects include Racket, Common Lisp, *Scheme*, and *Clojure*.[2]

## Prolog

*Cons*: Prolog’s complex logic often leads to errors due to developer mistakes. This imposes a challenge since the language does not offer great tools for debugging. Therefore, quality assurance for Prolog programs is challenging and requires procedural interpretation.[2]

- Zamia-AI
- mlu
- cplint
- cplint_datasets

## Scala

*Pros*: Programs written in Scala have much less boilerplate code compared to those written in Java and this adds to its usability and simplicity. Scala also features a toolset for writing concurrent applications that can easily scale and process real-time streams of data. Due to these features, Scala has become an integral component of data analysis applications including Apache Flink, Apache Spark, Apache Kafka, and Akka Stream.[2]

*Cons*: lack of community support, low adoption, limitations on backward compatibility, and a steep learning curve.[2]

- Breeze

## Rust

*Cons*: Rust can be difficult to learn and requires knowledge of object-oriented programming concepts. It has a slow compiler and the resulting binary files are quite large. There is a limited number of machine learning libraries written explicitly in Rust.[2]

However, developers can find many bindings to standard machine learning libraries such as [2]

- PyTorch
- TensorFlow

## Haskell

*Cons*: Haskell’s learning curve, however,  is fairly steep when compared to other languages commonly used for AI development. Haskell is a lazy language, which means that values are evaluated only when needed. This often leads to difficulties in memory allocation.[2]

## Julia

Refer tp [2]:

Since the language was designed primarily for numerical and scientific computing, Julia has become very popular in research and scientific communities. It offers an abundance of libraries such as

- differential equations ecosystem *DifferentialEquations*
- optimization tools *JuMP* and *Optim*
- iterative linear solvers *IterativeSolvers*
- Fast Fourier transforms *AbstractFFTs*

For statistical analysis and data science, Julia provides *DataFrames* to work with datasets and perform common data manipulations. *JuliaGraphs* packages offer the opportunity to work with combinatorial data.

For machine learning, Julia offers

- MLJ package - common machine learning algorithms
- Flux and Knet for deep learning purposes.

Top use cases:

- Numerical analysis
- Computational scientific analysis
- Time-series analysis
- Machine learning

## MATLAB

MATLAB (MATrix LABoratory) is a closed source programming language and numeric computing environment.[2]

*Cons*: Expensive license cost [2]

The [Statistics and Machine Learning Toolbox](https://www.mathworks.com/products/statistics.html) allows:

- Exploratory Data Analysis
  - Visualization such as scatter plot and box plot
  - Descriptive statistics
  - Cluster alanysis
- Feature Extraction and Dimensionality Reduction
  - Extract features from data using unsupervised learning techniques such as sparse filtering and reconstruction ICA
  - Feature selection methods include stepwise regression, sequential feature selection, regularization, and ensemble methods
  - Feature transformation methods include PCA, factor analysis, and nonnegative matrix factorization
- Machine Learning
  - Train, Validate, and Tune Predictive Models
  - Automated Machine Learning (AutoML)
- Regression and ANOVA
  - Linear and Nonlinear Regression
  - Nonparametric Regression
  - Analysis of Variance (ANOVA)
- Probability Distributions and Hypothesis Tests
  - Probability Distributions
  - Random Number Generation
  - Hypothesis Testing such as t-tests, distribution tests (Chi-square, Jarque-Bera, Lilliefors, and Kolmogorov-Smirnov), and nonparametric tests
  

You can deploy statistical and machine learning models

- as standalone, MapReduce, or Spark™ applications;
- as web apps; or
- as Microsoft® Excel® add-ins

You cna build

- C/C++ shared libraries,
- Microsoft .NET assemblies,
- Java classes, and
- Python packages
