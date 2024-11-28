---
draft: true
---

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




_______________
#### Setup diagrams

```chart
type: pie
id: groups
legend: true
legendPosition: right
layout: rows
width: 80%
beginAtZero: false
fill: true
tension: 0.3
xDisplay: true
yDisplay: true
xTickDisplay: true
yTickDisplay: true
transparency: 0.4
```

```chart
type: radar
id: learning
legend: false
layout: rows
width: 100%
beginAtZero: false
fill: true
tension: 0.3
xDisplay: true
yDisplay: false
xTickDisplay: true
yTickDisplay: false
transparency: 0.4
```

```chart
type: radar
id: resources
legend: false
layout: rows
width: 100%
beginAtZero: false
fill: true
tension: 0.3
xDisplay: true
yDisplay: false
xTickDisplay: true
yTickDisplay: false
transparency: 0.4
```


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



### 📃 Source data : setup

<details><summary>Expand</summary>




|                                                      | Books | Articles (more informal, like Medium) | Short videos (2 - 10 minutes) | Video tutorials (e.g. showing coding while recording the screen) | Long video explanations (10 - 40 minutes) | Online courses (datacamp, coursera ...) | Podcasts |
| ---------------------------------------------------- | ----- | ------------------------------------- | ----------------------------- | ---------------------------------------------------------------- | ----------------------------------------- | --------------------------------------- | -------- |
| **In which form do you prefer the resources to be?** | 0     | 3                                     | 14                            | 7                                                                | 2                                         | 4                                       | 0        |

^resources



|                             | Having a predefined exercise with a set of instructions (and someone helping in case I am stuck) | Making an exercise applied directly to my project | Someone shows me the steps on a big screen and I follow ✌🏻 | I watch video tutorials on my own and follow the steps in my own pace | Reading instructions from an article |
| --------------------------- | ------------------------------------------------------------------------------------------------ | ------------------------------------------------- | ----------------------------------------------------------- | --------------------------------------------------------------------- | ------------------------------------ |
| How do you prefer to learn? | 11                                                                                               | 2                                                 | 1                                                           | 1                                                                     | 0                                    |

^learning


|   | working alone is best during such workshops | working in pairs was cool  | I prefer bigger groups with more discussions and interactions (3-4 people) |
| --------- | ------------------------------ | --- | --- | --- | 
| Groups or no groups? | 0  | 15 | 0   | 

^groups


|                                                            | 1 - too easy, I want something more challenging | 2.  | 3.  | 4.  | 5 -  just right | 6.  | 7.  | 8.  | 9.  | 10 - too hard, I need something easier |
| ---------------------------------------------------------- | ----------------------------------------------- | --- | --- | --- | --------------- | --- | --- | --- | --- | -------------------------------------- |
| How do you estimate the difficulty level of the exercises? | 0                                               | 0   | 0   | 0   | 7               | 4   | 4   | 4   | 0   | 0                                      |

^difficulty


|                                 | 1 - undearable | 2.  | 3.  | 4.  | 5.  | 6.  | 7.  | 8.  | 9.  | 10 - fantastic |
| ------------------------------- | -------------- | --- | --- | --- | --- | --- | --- | --- | --- | -------------- |
| How was the overall experience? | 0              | 0   | 0   | 0   | 0   | 0   | 6   | 1   | 6   | 2              |

^overall

</details>

