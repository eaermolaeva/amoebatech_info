### Datasets

1. **data_eu** - full dataset of samples from Amesbury et al., 2016
2. **complexes** - species lumped into complexes with a scale for each complex
3. **traita** - *to be added later*

### How to use:

```markdown
How to install and use my package:

# install the package

# install.packages("remotes")
remotes::install_github("eaermolaeva/amoebatech")

#------------------------------------------------
# load the package
library(amoebatech)

#explore the datasets
data(package = 'amoebatech')

data_eu <- data_eu
complexes <- complexes

# check out documentations
?amoebatech
?data_eu
?complexes

#------------------------------------------------
# explore the data_eu dataset
library(tidyverse)
data_eu %>%
  count(person)

data_eu %>%
  group_by(person) %>%
  summarize(across(c(wtd, ph), max, na.rm = F))


```

