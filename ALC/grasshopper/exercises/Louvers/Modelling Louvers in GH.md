
**Level:** Beginner
**What you learn:** basic primitives, basic operations, modelling volume from a shape.

![[grasshopper/exercises/Louvers/illustrations/resulta.png]]

### Steps

1. Create a line that the louvers will be placed onto. This line will be the lower bound of the louvers, the **base line**.
   🎢 **Bonus:** create a curved line

> [!abstract]- Illustration
> ![[grasshopper/exercises/Louvers/illustrations/1_step.png]]

> [!tip]- 👀 Hint
> _Hint: line can be composed of two points. Create them first, then join them into a line._
 
> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Louvers/illustrations/1_solution.png]]

   
2. Create the line that limits the louvers from the top. This line will be the upper bound of the louvers.
   🎢 **Bonus:** lines can differ in length (e.g. lower line could be 1 meter and the upper one could be 1.5)
   
> [!abstract]- Illustration
> ![[grasshopper/exercises/Louvers/illustrations/2_step.png]]

> [!tip]- 👀 Hint
> _Hint: you can make a new line or move the base line to some distance._
  
> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Louvers/illustrations/2_solution.png]]

3. Get 10 points from the lower line. At these points we will place the louvers later.

> [!abstract]- Illustration
> ![[grasshopper/exercises/Louvers/illustrations/3_step.png]]

> [!tip]- 👀 Hint
> _Hint: you only need to divide the line into segments, there is no need to actually create points for that._

> [!success]- ⚙️Solution
> ![[3_solution.png]]

4. Get 10 corresponding points from the top line and connect them to the base line points.
   
> [!abstract]- Illustration
> ![[grasshopper/exercises/Louvers/illustrations/4_Step.png]]

> [!tip]- 👀 Hint
> _Hint: you can reuse the previous division operator. Then the segments of both lines will have the same proportions._

> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Louvers/illustrations/4_solution.png]]

5. Now we have the base for our louvers! Great! The only part left is to make 3D shapes out of existing lines. First, let's _extrude_ each line and create a _plane_ out of it.
    🎢 **Bonus:** lines can be extruded along another line. It means that your louvers can have a more complex profile than a simple rectangle. Try to make it curved.
    
> [!abstract]- Illustration
> ![[grasshopper/exercises/Louvers/illustrations/5_step.png]]

> [!tip]- 👀 Hint
> _Hint: you likely want the extrusion to happen perpendicular to the base line and the louver plane._

> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Louvers/illustrations/5_solution.png]]
> More flexible solution:
> ![[5a_solution.png]]

6. Our louvers are getting more shape now, time to give them _volume_ and convert from 2D planes into 3D forms. Let's extrude the planes into 3D boxes (parallelepipeds).

> [!abstract]- Illustration
> ![[6_step.png]]

> [!tip]- 👀 Hint
> _Hint: you likely want this extrusion to happen along the base line of the louvers. You can reuse this line as a vector direction or the module you have used in step 5._

> [!success]- ⚙️Solution
> ![[6_solution.png]]

7. Depending on how your louvers attach to the window construction you might want to _move_ them. One common way to attach the louvers is by the center point. Let's move our newly created parallelepipeds in a way that their center point lies on the base line.
   
> [!abstract]- Illustration
> _Note: the red points are situated in the center of the boxes._
>  ![[grasshopper/exercises/Louvers/illustrations/7_step.png]]

> [!tip]- 👀 Hint
> _Hint: you can reuse the first extrusion direction._

> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Louvers/illustrations/7_solution.png]]
> 

8. Louvers are ready! Now let's rotate them, as that's the main idea with having louvers :) 
   
   🎢 **Bonus:** assign different rotation angle to different parallelepipeds.
   ![[8_bonus.png]] ![[8a_bonus.png]]
   
> [!abstract]- Illustration
   > ![[grasshopper/exercises/Louvers/illustrations/8_step.png]]
   > Now you can control each module separately and change the profile shape by adding one module:
   > ![[8a_step.png]]

> [!tip]- 👀 Hint
> _Hint I: check the units the rotation module uses. 
> Hint II: you can reuse the points that we've got by dividing the base line into segments._

> [!success]- ⚙️Solution
> ![[grasshopper/exercises/Louvers/illustrations/8_solution.png]]
   
![[grasshopper/exercises/Louvers/illustrations/result.png]]

Check out the [full script](/grasshopper/exercises/scripts/Louvers.gh) if you get stuck! 

________
_This exercise has been developed under the workshop for [Umeå universitetet](https://www.umu.se/)for the course of [Elena Vazquez Peña](https://www.umu.se/personal/elena-vazquez/) Architectural Design Studio HT23-24._