### Install packages if not installed
```{r}
list.of.packages <- c("tidytext",
                      "tm",
                      "mnormt", 
                      "psych", 
                      "SnowballC",
                      "janitor")
                      
new.packages <- list.of.packages[!(list.of.packages %in% installed.packages()[,"Package"])]
if(length(new.packages)) install.packages(new.packages)
```