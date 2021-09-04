# EnemyAIwithPathfinding
 Enemy patrol, pursuiving player and pathfinding system at the same time !

1. Import Astar Pathfinding.

2. New Empty "A*".

3. Add component "Pathfinder".

/ Graphs Tab  /

/Grid graph category/

4.  Check 2D.

5. Check "2D Physics".

6. Select your tilemap with collisions in the Hierarchy, and give it a tag.

7. Go back in A*, and (still in Grid Graph) set Obstacle Layer Mask to the layer of your collision tilemap.

8. Collider type : Circle.

9. Diameter : 0.2.

10. Resize you Pathfinding Grid in the Scene view to your environment.

11. Now, click "Scan". 
>You may have an incorrect scan, and it can be due to the diameter size, or that the red dots aren't placed on each tile but between.


We will make an enemy now. You may use yours and skip this part.
---------------------------------------------------------------------------
12. Make a new 2D Object which will be a square and name it "Enemy".

13. Add a Box Collider 2D & Rigidbody 2D.

14. Rigidbody 2D :
    - Gravity Scale : 0
    - Constraits/Freeze Rotation Z : checked.
---------------------------------------------------------------------------

15. Create a new Physics Material 2D (Create/2D/Physics Material 2D).

16. Friction : 0.

17. Give this Physics Material 2D to your Enemy (In Rigidbody/Material).

18. Mass : 5.

19. Add component "Seeker".