<br>

**\[[🇧🇷 Português](README.pt_BR.md)\] \[**[🇺🇸 English](README.md)**\]**

<br><br>



#  <p align="center"> 11- [Data Mining]() /  [Affinity Propagation Algorithm]()



<!-- ======================================= Start DEFAULT HEADER ===========================================  -->

<br><br>


[**Institution:**]() Pontifical Catholic University of São Paulo (PUC-SP)  
[**School:**]() Faculty of Interdisciplinary Studies  
[**Program:**]() Humanistic AI and Data Science
[**Semester:**]() 2nd Semester 2025  
Professor:  [***Professor Doctor in Mathematics Daniel Rodrigues da Silva***](https://www.linkedin.com/in/daniel-rodrigues-048654a5/)

<br><br>

#### <p align="center"> [![Sponsor Quantum Software Development](https://img.shields.io/badge/Sponsor-Quantum%20Software%20Development-brightgreen?logo=GitHub)](https://github.com/sponsors/Quantum-Software-Development)


<br><br>

<!--Confidentiality statement -->

#

<br><br><br>

> [!IMPORTANT]
> 
> ⚠️ Heads Up
>
> * Projects and deliverables may be made [publicly available]() whenever possible.
> * The course emphasizes [**practical, hands-on experience**]() with real datasets to simulate professional consulting scenarios in the fields of **Data Analysis and Data Mining** for partner organizations and institutions affiliated with the university.
> * All activities comply with the [**academic and ethical guidelines of PUC-SP**]().
> * Any content not authorized for public disclosure will remain [**confidential**]() and securely stored in [private repositories]().  
>


<br><br>

#

<!--END-->




<br><br><br><br>



<!-- PUC HEADER GIF
<p align="center">
  <img src="https://github.com/user-attachments/assets/0d6324da-9468-455e-b8d1-2cce8bb63b06" />
-->


<!-- video presentation -->


##### 🎶 Prelude Suite no.1 (J. S. Bach) - [Sound Design Remix]()

https://github.com/user-attachments/assets/4ccd316b-74a1-4bae-9bc7-1c705be80498

####  📺 For better resolution, watch the video on [YouTube.](https://youtu.be/_ytC6S4oDbM)


<br><br>


> [!TIP]
> 
>  This repository is a review of the Statistics course from the undergraduate program Humanities, AI and Data Science at PUC-SP.
>
> ### ☞ **Access Data Mining [Main Repository](https://github.com/Quantum-Software-Development/1-Main_DataMining_Repository)**
> 
>  If you’d like to explore the full materials from the 1st year (not only the review), you can visit the complete repository [here](https://github.com/FabianaCampanari/PracticalStats-PUCSP-2024).
>
>



<!-- =======================================END DEFAULT HEADER ===========================================  -->


<br><br>><br>



## Table of Contents

- [Introduction](#introduction)
- [What is the Affinity Propagation Algorithm?](#what-is-the-affinity-propagation-algorithm)
- [Unsupervised vs. Supervised Learning](#unsupervised-vs-supervised-learning)
- [Silhouette Score: Evaluating Clustering](#silhouette-score-evaluating-clustering)
- [Correlation Matrix](#correlation-matrix)
    - [Positive Correlation](#positive-correlation)
    - [Negative Correlation](#negative-correlation)
- [Affinity Propagation vs. KMeans: Use Case Table](#affinity-propagation-vs-kmeans-use-case-table)
- [Code Examples: Correlation Matrix with 5 Variables](#code-examples-correlation-matrix-with-5-variables)
- [References](#references)


<br><br>



This repository provides an in-depth review of the [Affinity Propagation Algorithm](https://github.com/Quantum-Software-Development/11-DataMining_Affinity_Propagation_Algorithm/blob/main) as applied in data mining tasks, emphasizing both theory and practical implementation. It is designed as a companion to professional and academic courses focusing on [**unsupervised learning**]() and practical [**clustering**]() methods.



<br><br>


## [What is the Affinity Propagation Algorithm]() ?

**Affinity Propagation** is a clustering algorithm that identifies exemplars among data points and forms clusters of data points around these exemplars. Unlike algorithms like KMeans, it does not require the number of clusters to be specified beforehand. Instead, it uses the concept of "message passing" between data points to find a number of clusters that best reflects the data structure.


<br>

- [**Key steps**]():
  
    [-]() Exchanges real-valued messages between data points.
  
    [-]() Determines exemplars based on similarities.
      
    [-]() Forms clusters around exemplars.



<br><br>


## [How does it differ from other clustering methods]() ?

Affinity Propagation chooses the number of clusters automatically by maximizing a global criterion. KMeans, by contrast, needs a predefined number of clusters.


<br><br>


## [Unsupervised vs. Supervised Learning]()

[**Unsupervised learning** algorithms are designed to identify patterns or groupings in datasets without labeled responses. The model explores the input data to find structure (like clustering or association).

<br>

- [**Supervised learning**]() uses labeled data to train predictive models for regression or classification.

- [**Unsupervised learning**]() (like Affinity Propagation, KMeans, Hierarchical Clustering) finds patterns without explicit feedback.


<br><br>

| [Criteria]() | [Supervised Learning]() | [Unsupervised Learning]() |
| :-- | :-- | :-- |
| [Labeled data]() | Yes | No |
| [Tasks]() | Classification, Regression | Clustering, Association |
| [Example Algorithms]() | Decision Tree, SVM | KMeans, Affinity Propagation |



<br><br>


## [Silhouette Score: Evaluating Clustering]()

<br>

The [**Silhouette Score**]() evaluates how well an object lies within its cluster compared to other clusters. It ranges from -1 to 1:

[-]() Close to [**1**](): sample is well matched to its own cluster.

[-]() Close to [**0**](): sample is on or very close to the decision boundary between two clusters.

[-]() Close to [**-1**](): sample might have been assigned to the wrong cluster.

<br>

#### *The Silhouette Score \$S\$ for a sample is*:

<br>

\$S = \frac{b - a}{\max(a, b)}\$ 

<br>


#### [Where]():

<br>

[-]() \$a\$ [=]() mean intra-cluster distance for a sample (mean distance to all other samples in the same cluster).

[-]() \$b\$ [=]() mean nearest-cluster distance (lowest average distance to samples of another cluster).


<br><br>


## [Correlation Matrix]() 

A **Correlation Matrix** shows the statistical relationship (correlation) between pairs of variables. It helps to identify whether variables move together (correlate) and how strongly.

<br>

- [**Diagonal values**](): always 1 (a variable's correlation with itself).

  <br>

- [**Off-diagonal values**](): range from -1 to 1.
    
    - [**1**](): Perfect positive correlation.
   
    - [**0**](): No linear correlation.
    
    - [**-1**](): Perfect negative correlation.


<br>


### - [*Positive Correlation*]()

Two variables have [**positive correlation**]() if they increase in tandem.<br>

*Example: Height and weight in humans typically show positive correlation.*


<br>


### - [*Negative Correlation*]()

[**Negative correlation**]() occurs when one variable increases while the other decreases, in an inversely proportional way.<br>

*Example: The amount of time spent watching TV and academic grades may have a negative correlation.*


<br><br>















<br><br>
<br><br>
<br><br>
<br><br>
<br><br>
<br><br>
<br><br>
<br><br>
<br><br>
<br><br>
<br><br>
<br><br>


<!-- ========================== [Bibliographr ====================  -->

<br><br>


## [Bibliography]()

[1](). **Castro, L. N. & Ferrari, D. G.** (2016). *Introduction to Data Mining: Basic Concepts, Algorithms, and Applications*. Saraiva.

[2](). **Ferreira, A. C. P. L. et al.** (2024). *Artificial Intelligence – A Machine Learning Approach*. 2nd Ed. LTC.

[3](). **Larson & Farber** (2015). *Applied Statistics*. Pearson.


<br>

### [Complementary Bibliography]()

- THOMAS, C. *Data Mining*. IntechOpen, 2018.  
- HUTTER, F.; KOTTHOFF, L.; VANSCHOREN, J. *Automated Machine Learning: Methods, Systems, Challenges*. Springer Nature, 2019.  
- NETTO, A.; MACIEL, F. *Python para Data Science e Machine Learning Descomplicado*. Alta Books, 2021.  
- RUSSELL, S. J.; NORVIG, P. *Artificial Intelligence: A Modern Approach*. GEN LTC, 2022.  
- SUD, K.; ERDOGMUS, P.; KADRY, S. *Introduction to Data Science and Machine Learning*. IntechOpen, 2020.




<br><br>

      
<!-- ======================================= Bibliography Portugues ===========================================  -->

<!--

## [Bibliography]()


[1](). **Castro, L. N. & Ferrari, D. G.** (2016). *Introdução à mineração de dados: conceitos básicos, algoritmos e aplicações*. Saraiva.

[2](). **Ferreira, A. C. P. L. et al.** (2024). *Inteligência Artificial - Uma Abordagem de Aprendizado de Máquina*. 2nd Ed. LTC.

[3](). **Larson & Farber** (2015). *Estatística Aplicada*. Pearson.


<br><br>
-->

<!-- ======================================= Start Footer ===========================================  -->


<br><br>


## 💌 [Let the data flow... Ping Me !](mailto:fabicampanari@proton.me)

<br><br>



#### <p align="center">  🛸๋ My Contacts [Hub](https://linktr.ee/fabianacampanari)


<br>

### <p align="center"> <img src="https://github.com/user-attachments/assets/517fc573-7607-4c5d-82a7-38383cc0537d" />




<br><br><br>

<p align="center">  ────────────── 🔭⋆ ──────────────


<p align="center"> ➣➢➤ <a href="#top">Back to Top </a>

<!--
<p align="center">  ────────────── ✦ ──────────────
-->



<!-- Programmers and artists are the only professionals whose hobby is their profession."

" I love people who are committed to transforming the world "

" I'm big fan of those who are making waves in the world! "

##### <p align="center">( Rafael Lain ) </p>   -->

#

###### <p align="center"> Copyright 2025 Quantum Software Development. Code released under the [MIT License license.](https://github.com/Quantum-Software-Development/Math/blob/3bf8270ca09d3848f2bf22f9ac89368e52a2fb66/LICENSE)


















