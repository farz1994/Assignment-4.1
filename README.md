1. Histogram for all variables in a dataset mtcars. Write a program to create histograms for all columns.

library(ggplot2)
library(tidyr)

mtcars %>% gather() %>% head()

d = ggplot(gather(mtcars), aes(value))+ geom_histogram(bins = 10, fill = 'green', col='blue', alpha = 0.2)+ facet_wrap(~key, scales = "free_x")
d

2. Check the probability distribution of all variables in mtcars


3. Write a program to create boxplot for all variables.
