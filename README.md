# Academic Project for STAT 627 (Statistical Machine Learning)

<!-- PROJECT LOGO -->
<br />
  <a href="https://github.com/Karene123/Women_in_the_labor_force">
    <img src="https://github.com/Karene123/Women_in_the_labor_force/assets/70621033/3cbbaccc-345f-452e-acf3-24b4e0c07304" alt="Logo" width="1500" height="500">
  </a>
  
<!-- TABLE OF CONTENTS -->
### Table of Contents

1. [Project Overview](#Project-Overview)
2. [Getting Started](#Getting-Started)
3. [Prerequisites](#Prerequisites)
4. [Utilized Python Libraries](#Utilized-Python-Libraries)
5. [Installation](#Installation)
6. [Challenges](#Challenges)
7. [Summary of Results and Methods Used](#Summary-of-Results-and-Methods-Used)
8. [Contributions](#Contributions)
9. [Acknowledgments](#Acknowledgments)
10. [Graphs](#Graphs)

# Women, Business, and Law (WBL) from the World Bank 

<!-- Project Overview -->
## About The Project

It was reported by the World Bank that approximately 2.4 billion women do not possess the same
economic opportunity as their male counterparts. As part of this number, we count 178 countries
preventing women from fully participating in the labor force, 86 countries restricting certain jobs
to women, and 95 countries where equal pay is not guaranteed (“Nearly 2.4 Billion”, 2022).
Those data were made available by the World Bank through their Women, Business, and Law (WBL)
project. The goal behind this initiative was to inform and provide “data on the laws and regulations
that affect women’s economic opportunity”(“About Us”). Since 2009, they have been collecting
data and researching how to improve women’s economic opportunities and empowerment. Our
study was conducted using their dataset published in 2021.

(1) We were first interested in knowing if we could predict a country’s WBL (Women, Business and
the Law) Index based on:
- the length of paid maternity leave
-  the retirement age
-  the country’s gross domestic product (GDP)
-  the percentage of females in the population
-   total population.

(2) We additionally wanted to classify whether a woman can work in an industrial job in the same way
a man can, based on:
- a country’s income level
- the length of paid paternity leave
- the length of paid maternity leave
- the WBL Index
- the retirement age
- the percentage of females in the population.

<!-- GETTING STARTED -->
## Getting Started

All the datapoints were downloaded from [Women, Business, And The Law](https://datacatalog.worldbank.org/search/dataset/0038489). 
This link leads directly to the website.

### Prerequisites

[R-4.3.2](https://cran.r-project.org/bin/windows/base/)

Install and Import those libraries in order to access the project.

### Utilized Python Libraries:

* [Haven](https://cran.r-project.org/web/packages/haven/index.html)
* [Tidyr](https://cran.r-project.org/web/packages/tidyr/index.html)
* [Dplyr](https://dplyr.tidyverse.org/)
* [Class](https://cran.r-project.org/web/packages/class/index.html)
* [Mass](https://cran.r-project.org/web/packages/MASS/index.html)

### Installation

* Haven
  ```sh
  install.packages("haven")
  ```
* Tidyr
  ```sh
  install.packages("tidyr")
  ```
* Dplyr
  ```sh
  install.packages("dplyr")
  ```
* Class
  ```sh
  install.packages("class")
  ```
* Mass
  ```sh
  install.packages("mass")
  ```

    <p align="right">(<a href="#readme-top">back to top</a>)</p>

## Summary of Results
  
We concluded that the ridge regression was able to best predict a country’s WBL while logistic regression had the highest classification rate for our second research question. We decided
to include all predictors variables in our ridge and logistic regression models.

![WIL3](https://github.com/Karene123/Women_in_the_labor_force/assets/70621033/10b785fc-aae2-4c54-9f2f-31535ace80ec)

![WIL2](https://github.com/Karene123/Women_in_the_labor_force/assets/70621033/7e307f5b-b4c4-4cef-bec1-8e9ccb17c11e)

![W](https://github.com/Karene123/Women_in_the_labor_force/assets/70621033/3d6cc85d-60d2-4e4f-9be4-c1b8f76b6d23)



