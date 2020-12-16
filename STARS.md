---
output: html_document
---
## This is the analysis of Stars and Galaxies
```{r}
library(ggplot2)
```
```{r}
g+geom_point()+geom_smooth(method = "lm")
ggplot(data1,aes(u,r,shape = class))+geom_point(col="pink")+geom_smooth(method = "lm")
```
```{r}
ggplot(data1,aes(u,r))+geom_point(mapping = aes(shape = class),col="Gray")+geom_smooth(method = "lm",col="brickred")
```
```{r}
ggplot(data1,aes(u,r))+geom_point(mapping = aes(shape = class),col="Gray")+geom_smooth(method = "lm",col="red")
ggplot(data1,aes(u,r))+geom_point(mapping = aes(shape = class),col="Bright yellow")+geom_smooth(method = "lm",col="red")
```
```{r}
ggplot(data1,aes(u,r))+geom_point(mapping = aes(shape = class),col="yellow")+geom_smooth(method = "lm",col="red")
```
```{r}
ggplot(data1,aes(u,r))+geom_point(mapping = aes(shape = class),col="yellow")+geom_smooth(method = "lm",col="red")+facet_wrap(~class,nrow = 20)
```
```{r}
ggplot(data1,aes(u,r))+geom_point(mapping = aes(shape = class),col="yellow")+geom_smooth(method = "lm",col="red")+facet_wrap(field~class)
```
```{r}
ggplot(data1,aes(u,r))+geom_point(mapping = aes(shape = class),col="yellow")+geom_smooth(method = "lm",col="red")+facet_wrap(field~class~camcol)
```
