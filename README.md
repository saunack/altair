# Graphing with altair
Altair is an open source graphing library which can create interactive graphs. This repository uses Altair to create such graphs for medical data (lab reports)


## Graph content
The following functionalities are present in the final graph: 
* Using tooltips and other basic functionalities
* Higlight datapoints based on proximity
* Datapoints can be toggled
* Show upper and lower (expected) bounds of data when a line is clicked
* Show vertical rules on certain dates

## Input
A sample input.csv file has been provided for direct usage in graph.ipynb. Otherwise, a raw ods file (xlsx/csv also works) has also been provided which needs to be processed via clean.ipynb

The final cleaned data has 3 levels of indexes and 3 mandatory columns ('value', 'UPPER': upper bound and 'LOWER':lower bound). The 1st level of index has no purpose (it could serve as another level of toggling since it's a higher level of categorisation for the next indexing layer). The last index is the date.

For reference, the final dataset looks like this

```
                                        Value       Interpolated value       Upper limit       Lower limit

Category       Subcategory       Date
```

## Usage
Run graph.ipynb directly, which uses input.csv. Otherwise, use clean.ipynb to create the input csv file from the raw ods file and then run the main notebook.

# References
* add selector in one part and filter in another: https://altair-viz.github.io/user_guide/transform/filter.html#selection-predicates\n
* rulers: https://altair-viz.github.io/gallery/bar_chart_with_mean_line.html\n
* highlighting: https://altair-viz.github.io/gallery/multiline_highlight.html\n
* toggling: https://github.com/altair-viz/altair/issues/954\n
* rulers, sliders and buttons: https://altair-viz.github.io/gallery/multiple_interactions.html

