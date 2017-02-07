# rmarkdownweek3
title: "R Markdown Presentation"author: "F. Janga"
date: "7 februari 2017"
output: ioslides_presentation
---
## Introduction
- Dataset cars
- Exploring the data
- An interactive plot with plotly
## Loading data
```{r}
library(plotly)
summary(cars)
```
## An interactive plot
```{r, echo=FALSE}
plot_ly(cars, x = speed, y = dist, type ='scatter', mode = 'lines' %>% layout(xaxis = x, yaxis = y))
```
