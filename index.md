---
title       : Datasets Explorer
subtitle    : presentation about the shiny app
author      : 
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
ext_widgets : {rCharts: [libraries/nvd3]}
widgets     : [bootstrap, quiz, shiny, interactive]
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---
<style>
.title-slide {background-color: #FFF}
</style>

## Datasets Explorer - Overview

![width] (assets/img/shinyApp.png)

--- .class #id

## More about the app - Datasets

This app allows users to choose a dataset from a pre-selected set of datasets and view a plot of that dataset. Users can also specify the number of observations to view from the chosen dataset.

The three datasets are:
- pressure
- rock
- cars

--- .class #id 

## Demo

Live demonstration of one of the charts used in the app.
- Scatter chart illustrates the relationship between the stopping distance and the speed in the cars dataset.

<!-- ScatterChart generated in R 3.1.2 by googleVis 0.5.7 package -->
<!-- Sat Jan 24 15:52:04 2015 -->


<!-- jsHeader -->
<script type="text/javascript">
 
// jsData 
function gvisDataScatterChartID7e24ddb9fac () {
var data = new google.visualization.DataTable();
var datajson =
[
 [
 4,
2 
],
[
 4,
10 
],
[
 7,
4 
],
[
 7,
22 
],
[
 8,
16 
],
[
 9,
10 
],
[
 10,
18 
],
[
 10,
26 
],
[
 10,
34 
],
[
 11,
17 
],
[
 11,
28 
],
[
 12,
14 
],
[
 12,
20 
],
[
 12,
24 
],
[
 12,
28 
],
[
 13,
26 
],
[
 13,
34 
],
[
 13,
34 
],
[
 13,
46 
],
[
 14,
26 
],
[
 14,
36 
],
[
 14,
60 
],
[
 14,
80 
],
[
 15,
20 
],
[
 15,
26 
],
[
 15,
54 
],
[
 16,
32 
],
[
 16,
40 
],
[
 17,
32 
],
[
 17,
40 
],
[
 17,
50 
],
[
 18,
42 
],
[
 18,
56 
],
[
 18,
76 
],
[
 18,
84 
],
[
 19,
36 
],
[
 19,
46 
],
[
 19,
68 
],
[
 20,
32 
],
[
 20,
48 
],
[
 20,
52 
],
[
 20,
56 
],
[
 20,
64 
],
[
 22,
66 
],
[
 23,
54 
],
[
 24,
70 
],
[
 24,
92 
],
[
 24,
93 
],
[
 24,
120 
],
[
 25,
85 
] 
];
data.addColumn('number','speed');
data.addColumn('number','dist');
data.addRows(datajson);
return(data);
}
 
// jsDrawChart
function drawChartScatterChartID7e24ddb9fac() {
var data = gvisDataScatterChartID7e24ddb9fac();
var options = {};
options["allowHtml"] = true;
options["title"] = "Scatter Chart for datasets";
options["hAxis"] = {title:'speed(mph'};
options["vAxis"] = {title:'dist(ft)'};
options["legend"] = "top";
options["width"] =    600;
options["height"] =    400;

    var chart = new google.visualization.ScatterChart(
    document.getElementById('ScatterChartID7e24ddb9fac')
    );
    chart.draw(data,options);
    

}
  
 
// jsDisplayChart
(function() {
var pkgs = window.__gvisPackages = window.__gvisPackages || [];
var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
var chartid = "corechart";
  
// Manually see if chartid is in pkgs (not all browsers support Array.indexOf)
var i, newPackage = true;
for (i = 0; newPackage && i < pkgs.length; i++) {
if (pkgs[i] === chartid)
newPackage = false;
}
if (newPackage)
  pkgs.push(chartid);
  
// Add the drawChart function to the global list of callbacks
callbacks.push(drawChartScatterChartID7e24ddb9fac);
})();
function displayChartScatterChartID7e24ddb9fac() {
  var pkgs = window.__gvisPackages = window.__gvisPackages || [];
  var callbacks = window.__gvisCallbacks = window.__gvisCallbacks || [];
  window.clearTimeout(window.__gvisLoad);
  // The timeout is set to 100 because otherwise the container div we are
  // targeting might not be part of the document yet
  window.__gvisLoad = setTimeout(function() {
  var pkgCount = pkgs.length;
  google.load("visualization", "1", { packages:pkgs, callback: function() {
  if (pkgCount != pkgs.length) {
  // Race condition where another setTimeout call snuck in after us; if
  // that call added a package, we must not shift its callback
  return;
}
while (callbacks.length > 0)
callbacks.shift()();
} });
}, 100);
}
 
// jsFooter
</script>
 
<!-- jsChart -->  
<script type="text/javascript" src="https://www.google.com/jsapi?callback=displayChartScatterChartID7e24ddb9fac"></script>
 
<!-- divChart -->
  
<div id="ScatterChartID7e24ddb9fac" 
  style="width: 600; height: 400;">
</div>
--- .class #id 
## URL of the Shiny App
Access the Shiny App Course Project at:
[Datasets Explorer] (https://melbadri.shinyapps.io/datasetsExplorer/)

--- .class #id 

## URL to the Shiny App
Access the Shiny App Course Project at:
[Datasets Explorer] (https://melbadri.shinyapps.io/datasetsExplorer/)
