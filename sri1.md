# Data Analysis on Iris Flowers
Sridhar  
7 January 2018  

## Load the data


```r
head(iris)
```

```
##   Sepal.Length Sepal.Width Petal.Length Petal.Width Species
## 1          5.1         3.5          1.4         0.2  setosa
## 2          4.9         3.0          1.4         0.2  setosa
## 3          4.7         3.2          1.3         0.2  setosa
## 4          4.6         3.1          1.5         0.2  setosa
## 5          5.0         3.6          1.4         0.2  setosa
## 6          5.4         3.9          1.7         0.4  setosa
```

## Scatterplot

By using scatterplots,we can find how much the parameters are correlated

<!--html_preserve--><div id="plot_id915001661-container" class="ggvis-output-container">
<div id="plot_id915001661" class="ggvis-output"></div>
<div class="plot-gear-icon">
<nav class="ggvis-control">
<a class="ggvis-dropdown-toggle" title="Controls" onclick="return false;"></a>
<ul class="ggvis-dropdown">
<li>
Renderer: 
<a id="plot_id915001661_renderer_svg" class="ggvis-renderer-button" onclick="return false;" data-plot-id="plot_id915001661" data-renderer="svg">SVG</a>
 | 
<a id="plot_id915001661_renderer_canvas" class="ggvis-renderer-button" onclick="return false;" data-plot-id="plot_id915001661" data-renderer="canvas">Canvas</a>
</li>
<li>
<a id="plot_id915001661_download" class="ggvis-download" data-plot-id="plot_id915001661">Download</a>
</li>
</ul>
</nav>
</div>
</div>
<script type="text/javascript">
var plot_id915001661_spec = {
  "data": [
    {
      "name": ".0",
      "format": {
        "type": "csv",
        "parse": {
          "Sepal.Length": "number",
          "Sepal.Width": "number"
        }
      },
      "values": "\"Species\",\"Sepal.Length\",\"Sepal.Width\"\n\"setosa\",5.1,3.5\n\"setosa\",4.9,3\n\"setosa\",4.7,3.2\n\"setosa\",4.6,3.1\n\"setosa\",5,3.6\n\"setosa\",5.4,3.9\n\"setosa\",4.6,3.4\n\"setosa\",5,3.4\n\"setosa\",4.4,2.9\n\"setosa\",4.9,3.1\n\"setosa\",5.4,3.7\n\"setosa\",4.8,3.4\n\"setosa\",4.8,3\n\"setosa\",4.3,3\n\"setosa\",5.8,4\n\"setosa\",5.7,4.4\n\"setosa\",5.4,3.9\n\"setosa\",5.1,3.5\n\"setosa\",5.7,3.8\n\"setosa\",5.1,3.8\n\"setosa\",5.4,3.4\n\"setosa\",5.1,3.7\n\"setosa\",4.6,3.6\n\"setosa\",5.1,3.3\n\"setosa\",4.8,3.4\n\"setosa\",5,3\n\"setosa\",5,3.4\n\"setosa\",5.2,3.5\n\"setosa\",5.2,3.4\n\"setosa\",4.7,3.2\n\"setosa\",4.8,3.1\n\"setosa\",5.4,3.4\n\"setosa\",5.2,4.1\n\"setosa\",5.5,4.2\n\"setosa\",4.9,3.1\n\"setosa\",5,3.2\n\"setosa\",5.5,3.5\n\"setosa\",4.9,3.6\n\"setosa\",4.4,3\n\"setosa\",5.1,3.4\n\"setosa\",5,3.5\n\"setosa\",4.5,2.3\n\"setosa\",4.4,3.2\n\"setosa\",5,3.5\n\"setosa\",5.1,3.8\n\"setosa\",4.8,3\n\"setosa\",5.1,3.8\n\"setosa\",4.6,3.2\n\"setosa\",5.3,3.7\n\"setosa\",5,3.3\n\"versicolor\",7,3.2\n\"versicolor\",6.4,3.2\n\"versicolor\",6.9,3.1\n\"versicolor\",5.5,2.3\n\"versicolor\",6.5,2.8\n\"versicolor\",5.7,2.8\n\"versicolor\",6.3,3.3\n\"versicolor\",4.9,2.4\n\"versicolor\",6.6,2.9\n\"versicolor\",5.2,2.7\n\"versicolor\",5,2\n\"versicolor\",5.9,3\n\"versicolor\",6,2.2\n\"versicolor\",6.1,2.9\n\"versicolor\",5.6,2.9\n\"versicolor\",6.7,3.1\n\"versicolor\",5.6,3\n\"versicolor\",5.8,2.7\n\"versicolor\",6.2,2.2\n\"versicolor\",5.6,2.5\n\"versicolor\",5.9,3.2\n\"versicolor\",6.1,2.8\n\"versicolor\",6.3,2.5\n\"versicolor\",6.1,2.8\n\"versicolor\",6.4,2.9\n\"versicolor\",6.6,3\n\"versicolor\",6.8,2.8\n\"versicolor\",6.7,3\n\"versicolor\",6,2.9\n\"versicolor\",5.7,2.6\n\"versicolor\",5.5,2.4\n\"versicolor\",5.5,2.4\n\"versicolor\",5.8,2.7\n\"versicolor\",6,2.7\n\"versicolor\",5.4,3\n\"versicolor\",6,3.4\n\"versicolor\",6.7,3.1\n\"versicolor\",6.3,2.3\n\"versicolor\",5.6,3\n\"versicolor\",5.5,2.5\n\"versicolor\",5.5,2.6\n\"versicolor\",6.1,3\n\"versicolor\",5.8,2.6\n\"versicolor\",5,2.3\n\"versicolor\",5.6,2.7\n\"versicolor\",5.7,3\n\"versicolor\",5.7,2.9\n\"versicolor\",6.2,2.9\n\"versicolor\",5.1,2.5\n\"versicolor\",5.7,2.8\n\"virginica\",6.3,3.3\n\"virginica\",5.8,2.7\n\"virginica\",7.1,3\n\"virginica\",6.3,2.9\n\"virginica\",6.5,3\n\"virginica\",7.6,3\n\"virginica\",4.9,2.5\n\"virginica\",7.3,2.9\n\"virginica\",6.7,2.5\n\"virginica\",7.2,3.6\n\"virginica\",6.5,3.2\n\"virginica\",6.4,2.7\n\"virginica\",6.8,3\n\"virginica\",5.7,2.5\n\"virginica\",5.8,2.8\n\"virginica\",6.4,3.2\n\"virginica\",6.5,3\n\"virginica\",7.7,3.8\n\"virginica\",7.7,2.6\n\"virginica\",6,2.2\n\"virginica\",6.9,3.2\n\"virginica\",5.6,2.8\n\"virginica\",7.7,2.8\n\"virginica\",6.3,2.7\n\"virginica\",6.7,3.3\n\"virginica\",7.2,3.2\n\"virginica\",6.2,2.8\n\"virginica\",6.1,3\n\"virginica\",6.4,2.8\n\"virginica\",7.2,3\n\"virginica\",7.4,2.8\n\"virginica\",7.9,3.8\n\"virginica\",6.4,2.8\n\"virginica\",6.3,2.8\n\"virginica\",6.1,2.6\n\"virginica\",7.7,3\n\"virginica\",6.3,3.4\n\"virginica\",6.4,3.1\n\"virginica\",6,3\n\"virginica\",6.9,3.1\n\"virginica\",6.7,3.1\n\"virginica\",6.9,3.1\n\"virginica\",5.8,2.7\n\"virginica\",6.8,3.2\n\"virginica\",6.7,3.3\n\"virginica\",6.7,3\n\"virginica\",6.3,2.5\n\"virginica\",6.5,3\n\"virginica\",6.2,3.4\n\"virginica\",5.9,3"
    },
    {
      "name": "scale/fill",
      "format": {
        "type": "csv",
        "parse": {}
      },
      "values": "\"domain\"\n\"setosa\"\n\"versicolor\"\n\"virginica\""
    },
    {
      "name": "scale/x",
      "format": {
        "type": "csv",
        "parse": {
          "domain": "number"
        }
      },
      "values": "\"domain\"\n4.12\n8.08"
    },
    {
      "name": "scale/y",
      "format": {
        "type": "csv",
        "parse": {
          "domain": "number"
        }
      },
      "values": "\"domain\"\n1.88\n4.52"
    }
  ],
  "scales": [
    {
      "name": "fill",
      "type": "ordinal",
      "domain": {
        "data": "scale/fill",
        "field": "data.domain"
      },
      "points": true,
      "sort": false,
      "range": "category10"
    },
    {
      "name": "x",
      "domain": {
        "data": "scale/x",
        "field": "data.domain"
      },
      "zero": false,
      "nice": false,
      "clamp": false,
      "range": "width"
    },
    {
      "name": "y",
      "domain": {
        "data": "scale/y",
        "field": "data.domain"
      },
      "zero": false,
      "nice": false,
      "clamp": false,
      "range": "height"
    }
  ],
  "marks": [
    {
      "type": "symbol",
      "properties": {
        "update": {
          "size": {
            "value": 50
          },
          "fill": {
            "scale": "fill",
            "field": "data.Species"
          },
          "x": {
            "scale": "x",
            "field": "data.Sepal\\.Length"
          },
          "y": {
            "scale": "y",
            "field": "data.Sepal\\.Width"
          }
        },
        "ggvis": {
          "data": {
            "value": ".0"
          }
        }
      },
      "from": {
        "data": ".0"
      }
    }
  ],
  "legends": [
    {
      "orient": "right",
      "fill": "fill",
      "title": "Species"
    }
  ],
  "axes": [
    {
      "type": "x",
      "scale": "x",
      "orient": "bottom",
      "layer": "back",
      "grid": true,
      "title": "Sepal.Length"
    },
    {
      "type": "y",
      "scale": "y",
      "orient": "left",
      "layer": "back",
      "grid": true,
      "title": "Sepal.Width"
    }
  ],
  "padding": null,
  "ggvis_opts": {
    "keep_aspect": false,
    "resizable": true,
    "padding": {},
    "duration": 250,
    "renderer": "svg",
    "hover_duration": 0,
    "width": 672,
    "height": 480
  },
  "handlers": null
};
ggvis.getPlot("plot_id915001661").parseSpec(plot_id915001661_spec);
</script><!--/html_preserve-->

The Sepal Length and Sepal width are some what correlated but not that much,we can see that the setosa,
is completely separated since they have small sepal length and small sepal width than other species.But 
the real problem is that the virgincia,versicolor species were mixed apart.Hence we move to the next parameters.


```r
iris %>% ggvis(~Petal.Length,~Petal.Width,fill = ~Species) %>% layer_points()
```

<!--html_preserve--><div id="plot_id544732520-container" class="ggvis-output-container">
<div id="plot_id544732520" class="ggvis-output"></div>
<div class="plot-gear-icon">
<nav class="ggvis-control">
<a class="ggvis-dropdown-toggle" title="Controls" onclick="return false;"></a>
<ul class="ggvis-dropdown">
<li>
Renderer: 
<a id="plot_id544732520_renderer_svg" class="ggvis-renderer-button" onclick="return false;" data-plot-id="plot_id544732520" data-renderer="svg">SVG</a>
 | 
<a id="plot_id544732520_renderer_canvas" class="ggvis-renderer-button" onclick="return false;" data-plot-id="plot_id544732520" data-renderer="canvas">Canvas</a>
</li>
<li>
<a id="plot_id544732520_download" class="ggvis-download" data-plot-id="plot_id544732520">Download</a>
</li>
</ul>
</nav>
</div>
</div>
<script type="text/javascript">
var plot_id544732520_spec = {
  "data": [
    {
      "name": ".0",
      "format": {
        "type": "csv",
        "parse": {
          "Petal.Length": "number",
          "Petal.Width": "number"
        }
      },
      "values": "\"Species\",\"Petal.Length\",\"Petal.Width\"\n\"setosa\",1.4,0.2\n\"setosa\",1.4,0.2\n\"setosa\",1.3,0.2\n\"setosa\",1.5,0.2\n\"setosa\",1.4,0.2\n\"setosa\",1.7,0.4\n\"setosa\",1.4,0.3\n\"setosa\",1.5,0.2\n\"setosa\",1.4,0.2\n\"setosa\",1.5,0.1\n\"setosa\",1.5,0.2\n\"setosa\",1.6,0.2\n\"setosa\",1.4,0.1\n\"setosa\",1.1,0.1\n\"setosa\",1.2,0.2\n\"setosa\",1.5,0.4\n\"setosa\",1.3,0.4\n\"setosa\",1.4,0.3\n\"setosa\",1.7,0.3\n\"setosa\",1.5,0.3\n\"setosa\",1.7,0.2\n\"setosa\",1.5,0.4\n\"setosa\",1,0.2\n\"setosa\",1.7,0.5\n\"setosa\",1.9,0.2\n\"setosa\",1.6,0.2\n\"setosa\",1.6,0.4\n\"setosa\",1.5,0.2\n\"setosa\",1.4,0.2\n\"setosa\",1.6,0.2\n\"setosa\",1.6,0.2\n\"setosa\",1.5,0.4\n\"setosa\",1.5,0.1\n\"setosa\",1.4,0.2\n\"setosa\",1.5,0.2\n\"setosa\",1.2,0.2\n\"setosa\",1.3,0.2\n\"setosa\",1.4,0.1\n\"setosa\",1.3,0.2\n\"setosa\",1.5,0.2\n\"setosa\",1.3,0.3\n\"setosa\",1.3,0.3\n\"setosa\",1.3,0.2\n\"setosa\",1.6,0.6\n\"setosa\",1.9,0.4\n\"setosa\",1.4,0.3\n\"setosa\",1.6,0.2\n\"setosa\",1.4,0.2\n\"setosa\",1.5,0.2\n\"setosa\",1.4,0.2\n\"versicolor\",4.7,1.4\n\"versicolor\",4.5,1.5\n\"versicolor\",4.9,1.5\n\"versicolor\",4,1.3\n\"versicolor\",4.6,1.5\n\"versicolor\",4.5,1.3\n\"versicolor\",4.7,1.6\n\"versicolor\",3.3,1\n\"versicolor\",4.6,1.3\n\"versicolor\",3.9,1.4\n\"versicolor\",3.5,1\n\"versicolor\",4.2,1.5\n\"versicolor\",4,1\n\"versicolor\",4.7,1.4\n\"versicolor\",3.6,1.3\n\"versicolor\",4.4,1.4\n\"versicolor\",4.5,1.5\n\"versicolor\",4.1,1\n\"versicolor\",4.5,1.5\n\"versicolor\",3.9,1.1\n\"versicolor\",4.8,1.8\n\"versicolor\",4,1.3\n\"versicolor\",4.9,1.5\n\"versicolor\",4.7,1.2\n\"versicolor\",4.3,1.3\n\"versicolor\",4.4,1.4\n\"versicolor\",4.8,1.4\n\"versicolor\",5,1.7\n\"versicolor\",4.5,1.5\n\"versicolor\",3.5,1\n\"versicolor\",3.8,1.1\n\"versicolor\",3.7,1\n\"versicolor\",3.9,1.2\n\"versicolor\",5.1,1.6\n\"versicolor\",4.5,1.5\n\"versicolor\",4.5,1.6\n\"versicolor\",4.7,1.5\n\"versicolor\",4.4,1.3\n\"versicolor\",4.1,1.3\n\"versicolor\",4,1.3\n\"versicolor\",4.4,1.2\n\"versicolor\",4.6,1.4\n\"versicolor\",4,1.2\n\"versicolor\",3.3,1\n\"versicolor\",4.2,1.3\n\"versicolor\",4.2,1.2\n\"versicolor\",4.2,1.3\n\"versicolor\",4.3,1.3\n\"versicolor\",3,1.1\n\"versicolor\",4.1,1.3\n\"virginica\",6,2.5\n\"virginica\",5.1,1.9\n\"virginica\",5.9,2.1\n\"virginica\",5.6,1.8\n\"virginica\",5.8,2.2\n\"virginica\",6.6,2.1\n\"virginica\",4.5,1.7\n\"virginica\",6.3,1.8\n\"virginica\",5.8,1.8\n\"virginica\",6.1,2.5\n\"virginica\",5.1,2\n\"virginica\",5.3,1.9\n\"virginica\",5.5,2.1\n\"virginica\",5,2\n\"virginica\",5.1,2.4\n\"virginica\",5.3,2.3\n\"virginica\",5.5,1.8\n\"virginica\",6.7,2.2\n\"virginica\",6.9,2.3\n\"virginica\",5,1.5\n\"virginica\",5.7,2.3\n\"virginica\",4.9,2\n\"virginica\",6.7,2\n\"virginica\",4.9,1.8\n\"virginica\",5.7,2.1\n\"virginica\",6,1.8\n\"virginica\",4.8,1.8\n\"virginica\",4.9,1.8\n\"virginica\",5.6,2.1\n\"virginica\",5.8,1.6\n\"virginica\",6.1,1.9\n\"virginica\",6.4,2\n\"virginica\",5.6,2.2\n\"virginica\",5.1,1.5\n\"virginica\",5.6,1.4\n\"virginica\",6.1,2.3\n\"virginica\",5.6,2.4\n\"virginica\",5.5,1.8\n\"virginica\",4.8,1.8\n\"virginica\",5.4,2.1\n\"virginica\",5.6,2.4\n\"virginica\",5.1,2.3\n\"virginica\",5.1,1.9\n\"virginica\",5.9,2.3\n\"virginica\",5.7,2.5\n\"virginica\",5.2,2.3\n\"virginica\",5,1.9\n\"virginica\",5.2,2\n\"virginica\",5.4,2.3\n\"virginica\",5.1,1.8"
    },
    {
      "name": "scale/fill",
      "format": {
        "type": "csv",
        "parse": {}
      },
      "values": "\"domain\"\n\"setosa\"\n\"versicolor\"\n\"virginica\""
    },
    {
      "name": "scale/x",
      "format": {
        "type": "csv",
        "parse": {
          "domain": "number"
        }
      },
      "values": "\"domain\"\n0.705\n7.195"
    },
    {
      "name": "scale/y",
      "format": {
        "type": "csv",
        "parse": {
          "domain": "number"
        }
      },
      "values": "\"domain\"\n-0.02\n2.62"
    }
  ],
  "scales": [
    {
      "name": "fill",
      "type": "ordinal",
      "domain": {
        "data": "scale/fill",
        "field": "data.domain"
      },
      "points": true,
      "sort": false,
      "range": "category10"
    },
    {
      "name": "x",
      "domain": {
        "data": "scale/x",
        "field": "data.domain"
      },
      "zero": false,
      "nice": false,
      "clamp": false,
      "range": "width"
    },
    {
      "name": "y",
      "domain": {
        "data": "scale/y",
        "field": "data.domain"
      },
      "zero": false,
      "nice": false,
      "clamp": false,
      "range": "height"
    }
  ],
  "marks": [
    {
      "type": "symbol",
      "properties": {
        "update": {
          "size": {
            "value": 50
          },
          "fill": {
            "scale": "fill",
            "field": "data.Species"
          },
          "x": {
            "scale": "x",
            "field": "data.Petal\\.Length"
          },
          "y": {
            "scale": "y",
            "field": "data.Petal\\.Width"
          }
        },
        "ggvis": {
          "data": {
            "value": ".0"
          }
        }
      },
      "from": {
        "data": ".0"
      }
    }
  ],
  "legends": [
    {
      "orient": "right",
      "fill": "fill",
      "title": "Species"
    }
  ],
  "axes": [
    {
      "type": "x",
      "scale": "x",
      "orient": "bottom",
      "layer": "back",
      "grid": true,
      "title": "Petal.Length"
    },
    {
      "type": "y",
      "scale": "y",
      "orient": "left",
      "layer": "back",
      "grid": true,
      "title": "Petal.Width"
    }
  ],
  "padding": null,
  "ggvis_opts": {
    "keep_aspect": false,
    "resizable": true,
    "padding": {},
    "duration": 250,
    "renderer": "svg",
    "hover_duration": 0,
    "width": 672,
    "height": 480
  },
  "handlers": null
};
ggvis.getPlot("plot_id544732520").parseSpec(plot_id544732520_spec);
</script><!--/html_preserve-->
Check this,this scatterplot is pretty good,which separates the species and forms a perfect correlation
line.

## Correlations
Let's check the numerical correlations of the parameters

```r
print(cor(iris$Sepal.Length,iris$Sepal.Width))
```

```
## [1] -0.1175698
```

```r
print(cor(iris$Petal.Length,iris$Petal.Width))
```

```
## [1] 0.9628654
```
## Correlation matrix

For each property the correlations are identified for different species i.e, sentosa,versicolor,virginica

```r
type <- levels(iris$Species)
print(type[1])
```

```
## [1] "setosa"
```

```r
cor(iris[iris$Species==type[1],1:4])
```

```
##              Sepal.Length Sepal.Width Petal.Length Petal.Width
## Sepal.Length    1.0000000   0.7425467    0.2671758   0.2780984
## Sepal.Width     0.7425467   1.0000000    0.1777000   0.2327520
## Petal.Length    0.2671758   0.1777000    1.0000000   0.3316300
## Petal.Width     0.2780984   0.2327520    0.3316300   1.0000000
```

```r
print(type[2])
```

```
## [1] "versicolor"
```

```r
cor(iris[iris$Species==type[3],1:4])
```

```
##              Sepal.Length Sepal.Width Petal.Length Petal.Width
## Sepal.Length    1.0000000   0.4572278    0.8642247   0.2811077
## Sepal.Width     0.4572278   1.0000000    0.4010446   0.5377280
## Petal.Length    0.8642247   0.4010446    1.0000000   0.3221082
## Petal.Width     0.2811077   0.5377280    0.3221082   1.0000000
```

```r
print(type[3])
```

```
## [1] "virginica"
```

```r
cor(iris[iris$Species==type[3],1:4])
```

```
##              Sepal.Length Sepal.Width Petal.Length Petal.Width
## Sepal.Length    1.0000000   0.4572278    0.8642247   0.2811077
## Sepal.Width     0.4572278   1.0000000    0.4010446   0.5377280
## Petal.Length    0.8642247   0.4010446    1.0000000   0.3221082
## Petal.Width     0.2811077   0.5377280    0.3221082   1.0000000
```
## Knowing the data


```r
head(iris)
```

```
##   Sepal.Length Sepal.Width Petal.Length Petal.Width Species
## 1          5.1         3.5          1.4         0.2  setosa
## 2          4.9         3.0          1.4         0.2  setosa
## 3          4.7         3.2          1.3         0.2  setosa
## 4          4.6         3.1          1.5         0.2  setosa
## 5          5.0         3.6          1.4         0.2  setosa
## 6          5.4         3.9          1.7         0.4  setosa
```
## Structure of the data


```r
str(iris)
```

```
## 'data.frame':	150 obs. of  5 variables:
##  $ Sepal.Length: num  5.1 4.9 4.7 4.6 5 5.4 4.6 5 4.4 4.9 ...
##  $ Sepal.Width : num  3.5 3 3.2 3.1 3.6 3.9 3.4 3.4 2.9 3.1 ...
##  $ Petal.Length: num  1.4 1.4 1.3 1.5 1.4 1.7 1.4 1.5 1.4 1.5 ...
##  $ Petal.Width : num  0.2 0.2 0.2 0.2 0.2 0.4 0.3 0.2 0.2 0.1 ...
##  $ Species     : Factor w/ 3 levels "setosa","versicolor",..: 1 1 1 1 1 1 1 1 1 1 ...
```
## Tabulations


```r
table(iris$Species)
```

```
## 
##     setosa versicolor  virginica 
##         50         50         50
```


```r
round(prop.table(table(iris$Species)) * 100, digits = 1)
```

```
## 
##     setosa versicolor  virginica 
##       33.3       33.3       33.3
```


```r
summary(iris)
```

```
##   Sepal.Length    Sepal.Width     Petal.Length    Petal.Width   
##  Min.   :4.300   Min.   :2.000   Min.   :1.000   Min.   :0.100  
##  1st Qu.:5.100   1st Qu.:2.800   1st Qu.:1.600   1st Qu.:0.300  
##  Median :5.800   Median :3.000   Median :4.350   Median :1.300  
##  Mean   :5.843   Mean   :3.057   Mean   :3.758   Mean   :1.199  
##  3rd Qu.:6.400   3rd Qu.:3.300   3rd Qu.:5.100   3rd Qu.:1.800  
##  Max.   :7.900   Max.   :4.400   Max.   :6.900   Max.   :2.500  
##        Species  
##  setosa    :50  
##  versicolor:50  
##  virginica :50  
##                 
##                 
## 
```

```r
summary(iris[c("Petal.Width","Sepal.Width")])
```

```
##   Petal.Width     Sepal.Width   
##  Min.   :0.100   Min.   :2.000  
##  1st Qu.:0.300   1st Qu.:2.800  
##  Median :1.300   Median :3.000  
##  Mean   :1.199   Mean   :3.057  
##  3rd Qu.:1.800   3rd Qu.:3.300  
##  Max.   :2.500   Max.   :4.400
```
## Normalization

The normalization/feature scaling is not necessary but still,it improves the accuracy of this classification system.Here normalization process makes all the columns to be in the range of 0 to 1.


```r
library(class)
normalize <- function(x) {
num <- x - min(x)
denom <- max(x) - min(x)
return (num/denom)
}


iris_norm <- as.data.frame(lapply(iris[1:4], normalize))


summary(iris_norm)
```

```
##   Sepal.Length     Sepal.Width      Petal.Length     Petal.Width     
##  Min.   :0.0000   Min.   :0.0000   Min.   :0.0000   Min.   :0.00000  
##  1st Qu.:0.2222   1st Qu.:0.3333   1st Qu.:0.1017   1st Qu.:0.08333  
##  Median :0.4167   Median :0.4167   Median :0.5678   Median :0.50000  
##  Mean   :0.4287   Mean   :0.4406   Mean   :0.4675   Mean   :0.45806  
##  3rd Qu.:0.5833   3rd Qu.:0.5417   3rd Qu.:0.6949   3rd Qu.:0.70833  
##  Max.   :1.0000   Max.   :1.0000   Max.   :1.0000   Max.   :1.00000
```
## Training and Testing sets

The dataset is divided into two parts
1) Training set : To train the classifier,it contains 2/3 of the dataset.
2) Testing set : To test the classifier,it contains 1/3 of the dataset.

So for the division purpose we need random rows,that's why we are using seed() method.

```r
set.seed(1234)
ind <- sample(2, nrow(iris), replace=TRUE, prob=c(0.67, 0.33))
ind
```

```
##   [1] 1 1 1 1 2 1 1 1 1 1 2 1 1 2 1 2 1 1 1 1 1 1 1 1 1 2 1 2 2 1 1 1 1 1 1
##  [36] 2 1 1 2 2 1 1 1 1 1 1 2 1 1 2 1 1 2 1 1 1 1 2 1 2 2 1 1 1 1 2 1 1 1 1
##  [71] 1 2 1 2 1 1 1 1 1 1 2 1 1 1 1 2 1 1 1 2 1 2 1 1 1 1 1 1 1 2 1 1 1 1 1
## [106] 1 1 1 1 1 2 1 2 1 1 2 2 1 1 2 2 2 2 2 1 1 1 1 1 1 2 1 1 1 2 1 2 1 1 2
## [141] 1 2 1 1 1 1 2 1 2 1
```


```r
iris.training <- iris[ind==1, 1:4]

head(iris.training)
```

```
##   Sepal.Length Sepal.Width Petal.Length Petal.Width
## 1          5.1         3.5          1.4         0.2
## 2          4.9         3.0          1.4         0.2
## 3          4.7         3.2          1.3         0.2
## 4          4.6         3.1          1.5         0.2
## 6          5.4         3.9          1.7         0.4
## 7          4.6         3.4          1.4         0.3
```

```r
iris.test <- iris[ind==2, 1:4]

head(iris.test)
```

```
##    Sepal.Length Sepal.Width Petal.Length Petal.Width
## 5           5.0         3.6          1.4         0.2
## 11          5.4         3.7          1.5         0.2
## 14          4.3         3.0          1.1         0.1
## 16          5.7         4.4          1.5         0.4
## 26          5.0         3.0          1.6         0.2
## 28          5.2         3.5          1.5         0.2
```
Here the data is being separated!with the above found random possibilities.

```r
iris.trainLabels <- iris[ind==1,5]

print(iris.trainLabels)
```

```
##   [1] setosa     setosa     setosa     setosa     setosa     setosa    
##   [7] setosa     setosa     setosa     setosa     setosa     setosa    
##  [13] setosa     setosa     setosa     setosa     setosa     setosa    
##  [19] setosa     setosa     setosa     setosa     setosa     setosa    
##  [25] setosa     setosa     setosa     setosa     setosa     setosa    
##  [31] setosa     setosa     setosa     setosa     setosa     setosa    
##  [37] setosa     setosa     versicolor versicolor versicolor versicolor
##  [43] versicolor versicolor versicolor versicolor versicolor versicolor
##  [49] versicolor versicolor versicolor versicolor versicolor versicolor
##  [55] versicolor versicolor versicolor versicolor versicolor versicolor
##  [61] versicolor versicolor versicolor versicolor versicolor versicolor
##  [67] versicolor versicolor versicolor versicolor versicolor versicolor
##  [73] versicolor versicolor versicolor versicolor virginica  virginica 
##  [79] virginica  virginica  virginica  virginica  virginica  virginica 
##  [85] virginica  virginica  virginica  virginica  virginica  virginica 
##  [91] virginica  virginica  virginica  virginica  virginica  virginica 
##  [97] virginica  virginica  virginica  virginica  virginica  virginica 
## [103] virginica  virginica  virginica  virginica  virginica  virginica 
## [109] virginica  virginica 
## Levels: setosa versicolor virginica
```

```r
iris.testLabels <- iris[ind==2, 5]

print(iris.testLabels)
```

```
##  [1] setosa     setosa     setosa     setosa     setosa     setosa    
##  [7] setosa     setosa     setosa     setosa     setosa     setosa    
## [13] versicolor versicolor versicolor versicolor versicolor versicolor
## [19] versicolor versicolor versicolor versicolor versicolor versicolor
## [25] virginica  virginica  virginica  virginica  virginica  virginica 
## [31] virginica  virginica  virginica  virginica  virginica  virginica 
## [37] virginica  virginica  virginica  virginica 
## Levels: setosa versicolor virginica
```

## Classification

Here the k-Nearest Neighbour Classification is applied,with the training set and the testing set and the 
species were predicted.The knn() method does a good job by predicting the species based on the training 
set and they were tested by the testing set.


```r
iris_pred <- knn(train = iris.training, test = iris.test, cl = iris.trainLabels, k=3)
iris_pred
```

```
##  [1] setosa     setosa     setosa     setosa     setosa     setosa    
##  [7] setosa     setosa     setosa     setosa     setosa     setosa    
## [13] versicolor versicolor versicolor versicolor versicolor versicolor
## [19] versicolor versicolor versicolor versicolor versicolor versicolor
## [25] virginica  virginica  virginica  virginica  versicolor virginica 
## [31] virginica  virginica  virginica  virginica  virginica  virginica 
## [37] virginica  virginica  virginica  virginica 
## Levels: setosa versicolor virginica
```

## Comparison
 We need to make sure that our classifier has classified the species correctly,in order to do that we merge the real species name and the predicted name.As a result we find something unsual.


```r
irisTestLabels <- data.frame(iris.testLabels)

merge <- data.frame(iris_pred, iris.testLabels)

names(merge) <- c("Predicted Species", "Observed Species")

merge
```

```
##    Predicted Species Observed Species
## 1             setosa           setosa
## 2             setosa           setosa
## 3             setosa           setosa
## 4             setosa           setosa
## 5             setosa           setosa
## 6             setosa           setosa
## 7             setosa           setosa
## 8             setosa           setosa
## 9             setosa           setosa
## 10            setosa           setosa
## 11            setosa           setosa
## 12            setosa           setosa
## 13        versicolor       versicolor
## 14        versicolor       versicolor
## 15        versicolor       versicolor
## 16        versicolor       versicolor
## 17        versicolor       versicolor
## 18        versicolor       versicolor
## 19        versicolor       versicolor
## 20        versicolor       versicolor
## 21        versicolor       versicolor
## 22        versicolor       versicolor
## 23        versicolor       versicolor
## 24        versicolor       versicolor
## 25         virginica        virginica
## 26         virginica        virginica
## 27         virginica        virginica
## 28         virginica        virginica
## 29        versicolor        virginica
## 30         virginica        virginica
## 31         virginica        virginica
## 32         virginica        virginica
## 33         virginica        virginica
## 34         virginica        virginica
## 35         virginica        virginica
## 36         virginica        virginica
## 37         virginica        virginica
## 38         virginica        virginica
## 39         virginica        virginica
## 40         virginica        virginica
```
The classifier did a small mistake i.e, instead of versicolor,it predicted as virginica.
This k-NN classification is not 100 % percent accurate.

## Proper summary


```r
library(gmodels)
CrossTable(x = iris.testLabels, y = iris_pred, prop.chisq=FALSE)
```

```
## 
##  
##    Cell Contents
## |-------------------------|
## |                       N |
## |           N / Row Total |
## |           N / Col Total |
## |         N / Table Total |
## |-------------------------|
## 
##  
## Total Observations in Table:  40 
## 
##  
##                 | iris_pred 
## iris.testLabels |     setosa | versicolor |  virginica |  Row Total | 
## ----------------|------------|------------|------------|------------|
##          setosa |         12 |          0 |          0 |         12 | 
##                 |      1.000 |      0.000 |      0.000 |      0.300 | 
##                 |      1.000 |      0.000 |      0.000 |            | 
##                 |      0.300 |      0.000 |      0.000 |            | 
## ----------------|------------|------------|------------|------------|
##      versicolor |          0 |         12 |          0 |         12 | 
##                 |      0.000 |      1.000 |      0.000 |      0.300 | 
##                 |      0.000 |      0.923 |      0.000 |            | 
##                 |      0.000 |      0.300 |      0.000 |            | 
## ----------------|------------|------------|------------|------------|
##       virginica |          0 |          1 |         15 |         16 | 
##                 |      0.000 |      0.062 |      0.938 |      0.400 | 
##                 |      0.000 |      0.077 |      1.000 |            | 
##                 |      0.000 |      0.025 |      0.375 |            | 
## ----------------|------------|------------|------------|------------|
##    Column Total |         12 |         13 |         15 |         40 | 
##                 |      0.300 |      0.325 |      0.375 |            | 
## ----------------|------------|------------|------------|------------|
## 
## 
```
