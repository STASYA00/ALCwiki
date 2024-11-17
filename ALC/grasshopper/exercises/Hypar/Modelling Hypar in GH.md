---
title: Modelling hypar in Grasshopper
draft: false
description: An exercise on modelling hypar-like shapes in grasshopper.
permalink: /gh_hypar_exercise
aliases: Hypar, hypar, gh-hypar
tags:
  - grasshopper
  - AEC
  - graphical programming
  - parametric
  - hypar
  - beginner
---

**Level:** Beginner
**What you learn:** basic primitives, basic operations, loft, arrays, surface operations.

![[result_4.png]]
### Steps

1. Create a number of points in a straight line that would define our curve. The distance between these points does not matter.


> [!abstract]- Illustration
> ![[grasshopper/exercises/Hypar/illustrations/1_step.png]]

> [!tip]- 👀 Hint
> _Hint: You can divide a line into a number of points. Alternatively you can copy a point multiple times on a certain axis._
 
> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Hypar/illustrations/1_solution.png]]

   
2. Move the points along Z-axis on a _different_ amount of units, so that they create a _sinusoid curve_.
   
   
> [!abstract]- Illustration
> ![[grasshopper/exercises/Hypar/illustrations/2_step.png]]

> [!tip]- 👀 Hint
> _Hint: you can use a module called Graph Mapper and choose the type of curve by right-clicking on it. This module takes in a Range parameter, defining the lower and the upper bounds of the curve._
  
> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Hypar/illustrations/2_solution.png]]

3. Create one more curve, with the same number of points as a previous one but with a different curvature. You can choose another curve type (e.g. Gaussian) or modify the parameters of the previous one, making it lower/higher or tighter / wider.

> [!abstract]- Illustration
> ![[grasshopper/exercises/Hypar/illustrations/3_step.png]]

> [!tip]- 👀 Hint
> _Hint: you can copy the modules used to shift the points and choose a different curve type._

> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Hypar/illustrations/3_solution.png]]

4. Move the new curve some distance (span) from the first one.
   
> [!abstract]- Illustration
> ![[grasshopper/exercises/Hypar/illustrations/4_Step.png]]

> [!tip]- 👀 Hint
> _Hint: move the points of the second curve along Y-axis._

> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Hypar/illustrations/4_solution.png]]

5. Connect these points with the lines. These lines can be straight or curved, based on the type of shape that you want to achieve.
    
> [!abstract]- Illustration
> ![[grasshopper/exercises/Hypar/illustrations/5_step.png]]

> [!tip]- 👀 Hint
> _Hint: If you want to connect several arcs and make a smoother surface you would want to use curved connectors. This can be achieved with the Interpolate module._

> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Hypar/illustrations/5_solution.png]]


6. Let's add a third curve beside the previous two and connect the points of all the three.

> [!abstract]- Illustration
> ![[grasshopper/exercises/Hypar/illustrations/6_step.png]]

> [!tip]- 👀 Hint
> _Hint: take a look at Interpolate module. You can use the same module for all the three curves_

> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Hypar/illustrations/6_solution.png]]

7. Bridge the gap between the adjacent lines by creating small surfaces between them.
   
> [!abstract]- Illustration
>  ![[grasshopper/exercises/Hypar/illustrations/7_step.png]]

> [!tip]- 👀 Hint
> _Hint: one of the ways to achieve it is by using the Loft module._

> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Hypar/illustrations/7_solution.png]]
> 

8. The surface is ready! Let's add some supporting constructions to carry it. Create beams that are flat on the bottom side and follow the surface's curvature on the top. 
  
> [!abstract]- Illustration
   > ![[grasshopper/exercises/Hypar/illustrations/8_step.png]]
   
> [!tip]- 👀 Hint
> _Hint I: you can translate or project (module Project) already created geometry on the bottom plane. 

> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Hypar/illustrations/8_solution.png]]

9. Let's create the rails that carry our surface. Give volume to the initial three curves (the longitudinal ones). Check Surface/Freeform tab.
   
> [!abstract]- Illustration
>  ![[grasshopper/exercises/Hypar/illustrations/9_step.png]]

> [!tip]- 👀 Hint
> _Hint: take a look at Pipe module._

> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Hypar/illustrations/9_solution.png]]
> 

10. Give volume to the perpendicular curves as well.
   
> [!abstract]- Illustration
>  ![[grasshopper/exercises/Hypar/illustrations/10_step.png]]

> [!tip]- 👀 Hint
> _Hint: you can use the Pipe module._

> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Hypar/illustrations/10_solution.png]]
> 

![[grasshopper/exercises/Hypar/illustrations/result.png]]

![[result_1.png]]

![[grasshopper/exercises/Hypar/illustrations/result_2.png]]

Check out the [full script](/grasshopper/exercises/scripts/Hypar.gh) if you get stuck! 

________
_This exercise has been developed under the workshop for [Umeå universitetet](https://www.umu.se/)for the course of [Elena Vazquez Peña](https://www.umu.se/personal/elena-vazquez/) Architectural Design Studio HT23-24._

