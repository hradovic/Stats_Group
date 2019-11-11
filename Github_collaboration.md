---
title: "GitHub for Collaboration"
output: 
  html_document:
   keep_md: yes
---




```r
library(tidyverse)
library(fivethirtyeight)
library(dplyr)
```



```r
bad_drivers %>% 
  ggplot() +
  geom_jitter(aes(x = perc_alcohol, y = insurance_premiums))
```

![](Github_collaboration_files/figure-html/unnamed-chunk-2-1.png)<!-- -->


```r
bad_drivers %>% 
  ggplot() + 
  geom_jitter(aes(x = perc_alcohol, y = losses))
```

![](Github_collaboration_files/figure-html/unnamed-chunk-3-1.png)<!-- -->



```r
steak_survey %>% 
  ggplot() + 
  geom_bar(aes(x = steak_prep, fill = steak_prep))+
  facet_wrap(~region)
```

![](Github_collaboration_files/figure-html/unnamed-chunk-4-1.png)<!-- -->


```r
steak_survey %>% 
  ggplot() + 
  geom_bar(aes(x = steak_prep, fill = steak_prep), )+
  facet_wrap(~hhold_income)
```

![](Github_collaboration_files/figure-html/unnamed-chunk-5-1.png)<!-- -->


```r
steak_survey %>% 
  ggplot() + 
  geom_bar(aes(x = steak_prep, fill = steak_prep) )
```

![](Github_collaboration_files/figure-html/unnamed-chunk-6-1.png)<!-- -->
