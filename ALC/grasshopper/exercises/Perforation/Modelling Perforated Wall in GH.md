**Level:** Beginner
**What you learn:** working with lists, lists of lists (2D Arrays) and data trees.

![[grasshopper/exercises/Perforation/illustrations/resulta.png]]
### Steps

1. Make a wall that would serve as a base for perforations. Keep it 2D for now.
   
> [!abstract]- Illustration
> ![[grasshopper/exercises/Perforation/illustrations/1a_step.png]]
   
  > [!tip]- 👀 Hint
> _Hint I: we need to create a plane first. This plane can later be extruded as a wall._
> _Hint II: a plane can be constructed from a line and a point._

   > [!success]- ⚙️Solution
> ![[grasshopper/exercises/Perforation/illustrations/1_solution.png]]
> ![[grasshopper/exercises/Perforation/illustrations/1a_solution.png]]

2. Find points on one axis that would be centers of the perforation circles
   
> [!abstract]- Illustration
> ![[grasshopper/exercises/Perforation/illustrations/2_step.png]]
 
> [!tip]- 👀 Hint
> _Hint: divide the line into a number of segments._
   
> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Perforation/illustrations/5_solution.png]]

3. Propagate these centers along the second axis
   
> [!abstract]- Illustration
> ![[grasshopper/exercises/Perforation/illustrations/3_step.png]]
   
> [!tip]- 👀 Hint
> _Hint: You need to propagate **each list** along the axis. Check List of lists and [Graft](https://modelab.gitbooks.io/grasshopper-primer/content/1-foundations/1-5/3_creating-data-trees.html) option in Grasshopper._
   
> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Perforation/illustrations/3_solution.png]]

4. Create a shape for your perforation. We can start with a circle.    
   
> [!abstract]- Illustration
> ![[grasshopper/exercises/Perforation/illustrations/5_step.png]]
   
> [!tip]- 👀 Hint
> _Hint: you likely want this shape to lie in the same plane as the wall._
   
> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Perforation/illustrations/5_solution.png]]
> 

5. Place the perforation in the defined cetner points.
   
> [!abstract]- Illustration
> ![[grasshopper/exercises/Louvers/illustrations/5_step.png]]
   
> [!tip]- 👀 Hint
> _Hint: you can use the points defined in step 3 as centers of the circles (or the amount of translation)._
   
> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Perforation/illustrations/5_solution.png]]

6. Change the size of the perforation holes. Implement three different strategies:
	- assign same radius to all the perforations
	- assign random radius to all the perforations
	- create a sphere in the scene, change radius of the holes based on their distance to the sphere (*e.g. more distant -> smaller radius*)
	  
> [!abstract]- Illustration
> ![[grasshopper/exercises/Perforation/illustrations/6a_step.png]]
> ![[grasshopper/exercises/Perforation/illustrations/6b_step.png]]
> ![[grasshopper/exercises/Perforation/illustrations/6c_step.png]]

> [!tip]- 👀 Hint
> _Hint: there is an inbuilt block to calculate distance between two points. Center of the sphere can be the first one._

> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Perforation/illustrations/6a_solution.png]]
> ![[grasshopper/exercises/Perforation/illustrations/6b_solution.png]]
> ![[grasshopper/exercises/Perforation/illustrations/6c_solution.png]]

7. Time to perforate the wall! Let's first extrude the holes.
   
> [!abstract]- Illustration
> ![[grasshopper/exercises/Perforation/illustrations/7_step.png]]
   
> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Perforation/illustrations/7_solution.png]]

8. Let's subtract one surface from another
   
> [!abstract]- Illustration
> ![[grasshopper/exercises/Perforation/illustrations/8_step.png]]
   
> [!tip]- 👀 Hint
> _Hint: look through functions under Intersect / Shape._
   
> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Perforation/illustrations/8_solution.png]]

9. 🎢 **Bonus:** Add rotating circular panels in the middle of the holes. These panels can have a random rotation or be rotated versus the sphere.
   
   
![[grasshopper/exercises/Perforation/illustrations/result.png]]

Check out the [full script](/grasshopper/exercises/scripts/Perforation.gh) if you get stuck! 

_______
_This exercise has been developed under the workshop for [Umeå universitetet](https://www.umu.se/)for the course of [Elena Vazquez](https://www.umu.se/personal/elena-vazquez/) Architectural Design Studio HT23-24._