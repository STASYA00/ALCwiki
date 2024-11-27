---
banner_icon: 
title: Intro to Graphical Programming 24
draft: false
description: Learnings from Umeå Graphical Programming workshop | 24
permalink: /activities/igp24
banner: "![[gh_umeå_results_summary.png]]"
---

**Site:** [Umeå Universitet](https://www.umu.se/)
**Professor:** [Elena Vazquez Peña](https://www.umu.se/personal/elena-vazquez/)
**Course:** [Architectural Project II](https://www.umu.se/utbildning/kurser/arkitekturprojekt-21/), [Architectural Project III](https://www.umu.se/utbildning/kurser/arkitekturprojekt-31/)
**Period:** November 2024
**Mode:** #workshop
**Class:** 40 people


<div><img src="https://storage.googleapis.com/upplys_assets/activities/umu_igp24/output/gh_ume%C3%A5_results_summary.png"></img></div>

### ⚙️  Setup

During this workshop we tried out a [recipe methodology](https://umu.diva-portal.org/smash/record.jsf?language=sv&pid=diva2%3A1819075&dswid=-8563) widely used when teaching programming and software development but hardly applied within architectural field.

<div id="my_dataviz"></div>
The workshop was organized in the following way:

 * Short introduction to [[Graphical Programming]] + gh UI
 * Full day following the step-by step [[GH exercises]]
 * Preparing a model or a concept drawing implementing parametric design in their own architectural projects
 * Short presentation of the results and discussion
 * 🍪 Fika :)

Each step consisted of 4 parts: 
- Instruction
- Illustration of the result (collapsable)
- Hint (collapsable)
- Solution (collapsable)

### 🎓 Learnings

* <mark class="hltr-white_trans"> setup with steps, hints and solutions was well-accepted :)</mark>
* Such workshops should take <mark class="hltr-cyan">at least **2.5-3** days:</mark>
	* *1st day - exercises*
	* *2nd day - applying new skills to the students' own project*
	* *3rd day - presentation of the results and discussion*
* <mark class="hltr-cyan">Working in pairs</mark> is the preferred way for this activity type
* UI and general principles explanation should be kept <mark class="hltr-cyan">as short and simple as possible</mark>
* One suggestion that we received on UI explanation was showing how to create a box. A simple exercise that demonstrates basic working principles.
* Tutorials should have more steps for the #beginner level

* Hints could have the images or the names of the blocks from grasshopper
* <mark class="hltr-cyan">Highlighting the difference</mark> in the solution image after each step
* Separately explain how each of the components work (with a clickable link)


###  💫 Feedback
##### How was the overall experience?

<div id="my_dataviz"></div>
<div>
<script> // set the dimensions and margins of the graph const margin = {top: 30, right: 30, bottom: 30, left: 50}, width = 460 - margin.left - margin.right, height = 400 - margin.top - margin.bottom; // append the svg object to the body of the page const svg = d3.select("#my_dataviz") .append("svg") .attr("width", width + margin.left + margin.right) .attr("height", height + margin.top + margin.bottom) .append("g") .attr("transform", `translate(${margin.left},${margin.top})`); // get the data d3.csv("https://raw.githubusercontent.com/holtzy/D3-graph-gallery/master/DATA/data_doubleHist.csv").then( function(data) { data=[{type: "variable 1", value: "5"},{type: "variable 1", value: "5"},{type: "variable 1", value: "5"},{type: "variable 1", value: "5"},{type: "variable 1", value: "5"},{type: "variable 1", value: "5"}, {type: "variable 1", value: "10"}, {type: "variable 1", value: "1"},{type: "variable 1", value: "2"}, {type: "variable 1", value: "2"} ]; // add the x Axis const x = d3.scaleLinear() .domain([0,10]) .range([0, width]); svg.append("g") .attr("transform", `translate(0, ${height})`) .call(d3.axisBottom(x)); // add the y Axis const y = d3.scaleLinear() .range([height, 0]) .domain([0, 0.15]); svg.append("g") .call(d3.axisLeft(y)); // Compute kernel density estimation const kde = kernelDensityEstimator(kernelEpanechnikov(7), x.ticks(60)) const density1 = kde( data .filter( function(d){return d.type === "variable 1"} ) .map(function(d){ return d.value; }) ) // Plot the area svg.append("path") .attr("class", "mypath") .datum(density1) .attr("fill", "#69b3a2") .attr("opacity", ".6") .attr("stroke", "#000") .attr("stroke-width", 1) .attr("stroke-linejoin", "round") .attr("d", d3.line() .curve(d3.curveBasis) .x(function(d) { return x(d[0]); }) .y(function(d) { return y(d[1]); }) ); }); // Handmade legend svg.append("circle").attr("cx",300).attr("cy",30).attr("r", 6).style("fill", "#69b3a2") svg.append("circle").attr("cx",300).attr("cy",60).attr("r", 6).style("fill", "#404080") svg.append("text").attr("x", 320).attr("y", 30).text("variable A").style("font-size", "15px").attr("alignment-baseline","middle") // Function to compute density function kernelDensityEstimator(kernel, X) { return function(V) { return X.map(function(x) { return [x, d3.mean(V, function(v) { return kernel(x - v); })]; }); }; } function kernelEpanechnikov(k) { return function(v) { return Math.abs(v /= k) <= 1 ? 0.75 * (1 - v * v) / k : 0; }; } </script>
</div>

```chart
type: line
id: overall
legend: false
layout: rows
width: 100%
beginAtZero: false
fill: true
tension: 0.3
xDisplay: false
yDisplay: false
xTickDisplay: false
yTickDisplay: false
transparency: 0.4
```
_Unbearable_                                                                                                                           _Fantastic_                                                                                                                        
##### How easy is it to follow the tutorials and coding examples?

```chart
type: line
id: easytofollow
layout: rows
width: 80%
beginAtZero: false
fill: true
tension: 0.3
legend: false
xDisplay: false
yDisplay: false
xTickDisplay: false
yTickDisplay: false
transparency: 0.15
```
_Extremely hard_                                                        _Just right_                                            _Super easy_   

##### How user-friendly is the setup?
```chart
type: line
id: userfriendly
layout: rows
width: 80%
beginAtZero: false
fill: true
tension: 0.3
legend: false
xDisplay: false
yDisplay: false
xTickDisplay: false
yTickDisplay: false
transparency: 0.15

```
_Not user-friendly at all_                                                                                   _Very user-friendly_           

##### How well were you able to understand the instructions presented in the tutorials?
```chart
type: line
id: understanding
layout: rows
width: 80%
beginAtZero: false
fill: true
tension: 0.3
legend: false
xDisplay: false
yDisplay: false
xTickDisplay: false
yTickDisplay: false
transparency: 0.15
```
_Didn't understand anything_                                                                  _Everything was crystal clear_           
##### How do you estimate the difficulty level of the exercises?
```chart
type: line
id: difficulty
layout: rows
width: 100%
beginAtZero: false
fill: true
tension: 0.3
legend: false
xDisplay: false
yDisplay: false
xTickDisplay: false
yTickDisplay: false
transparency: 0.15
```
_Too easy, I want something more challenging_    _Just right_                _Too hard, I want something easier_           


____

### 📃 Source data

<details><summary>Expand</summary>

|                                                             | 1 - extremely hard | 2.  | 3.  | 4.  | 5.  | 6 - just right | 7.  | 8.  | 9.  | 10 - super easy |
| ----------------------------------------------------------- | ------------------ | --- | --- | --- | --- | -------------- | --- | --- | --- | --------------- |
| How easy it is to follow the tutorials and coding examples? | 0                  | 0   | 0   | 1   | 4   | 4              | 5   | 1   | 0   | 0               |

^easytofollow



|                                 | 1 - not user-friendly at all | 2.  | 3.  | 4.  | 5.  | 6.  | 7.  | 8.  | 9.  | 10 - very user-friendly |
| ------------------------------- | ---------------------------- | --- | --- | --- | --- | --- | --- | --- | --- | ----------------------- |
| How user-friendly is the setup? | 0                            | 0   | 0   | 0   | 3   | 2   | 3   | 4   | 1   | 2                       |

^userfriendly


|                                                                                   | 1 - didn't understand anything | 2.  | 3.  | 4.  | 5.  | 6.  | 7.  | 8.  | 9.  | 10 - everything was crystal clear |
| --------------------------------------------------------------------------------- | ------------------------------ | --- | --- | --- | --- | --- | --- | --- | --- | --------------------------------- |
| How well were you able to understand the instructions presented in the tutorials? | 0                              | 0   | 0   | 0   | 3   | 4   | 1   | 4   | 1   | 2                                 |

^understanding


|                                                            | 1 - too easy, I want something more challenging | 2.  | 3.  | 4.  | 5 -  just right | 6.  | 7.  | 8.  | 9.  | 10 - too hard, I need something easier |
| ---------------------------------------------------------- | ----------------------------------------------- | --- | --- | --- | --------------- | --- | --- | --- | --- | -------------------------------------- |
| How do you estimate the difficulty level of the exercises? | 0                                               | 0   | 0   | 0   | 7               | 4   | 4   | 4   | 0   | 0                                      |

^difficulty


|                                 | 1 - undearable | 2.  | 3.  | 4.  | 5.  | 6.  | 7.  | 8.  | 9.  | 10 - fantastic |
| ------------------------------- | -------------- | --- | --- | --- | --- | --- | --- | --- | --- | -------------- |
| How was the overall experience? | 0              | 0   | 0   | 0   | 0   | 0   | 6   | 1   | 6   | 2              |

^overall

</details>


