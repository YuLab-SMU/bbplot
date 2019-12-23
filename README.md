<!-- README.md is generated from README.Rmd. Please edit that file -->

# proof of concept for implementing grammar of graphics in base plot

``` r
library(bbplot)

p = bbplot(mtcars, list(x='mpg', y='disp'))
p1 = p %>% ly_point
p2 = p %>% ly_lm
p3 = p %>% ly_point %>% ly_lm(col='blue')
par(mfrow=c(2,2))
p; p1; p2; p3
```

![](README_files/figure-gfm/unnamed-chunk-1-1.png)<!-- -->
