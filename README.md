# Graphing with altair
Altair is an open source graphing library which can create interactive graphs.


## Graph content
The following functionalities are present in the final graph: 
* Using tooltips and other basic functionalities
* Higlight datapoints based on proximity
* Datapoints can be toggled
* Show upper and lower (expected) bounds of data when a line is clicked
* Show vertical rules on certain dates

## Input
The final cleaned data has 3 levels of indexes and 3 mandatory columns ('value', 'UPPER': upper bound and 'LOWER':lower bound). The 1st level of index has no purpose (it could serve as another level of toggling since it's a higher level of categorisation for the next indexing layer). The last index is the date.

For reference, the final dataset looks like this

```
                                        Value       Interpolated value       Upper limit       Lower limit

Category       Subcategory       Date
```

# References
* add selector in one part and filter in another: https://altair-viz.github.io/user_guide/transform/filter.html#selection-predicates\n
* rulers: https://altair-viz.github.io/gallery/bar_chart_with_mean_line.html\n
* highlighting: https://altair-viz.github.io/gallery/multiline_highlight.html\n
* toggling: https://github.com/altair-viz/altair/issues/954\n
* rulers, sliders and buttons: https://altair-viz.github.io/gallery/multiple_interactions.html

