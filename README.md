1. The Player (Head)

1] Create a 2D Sprite (square) to represent the head.

2] Attach the SnakeController script to it.

3] Add a Rigidbody 2D component. Set Gravity Scale to 0.

4] Add a Box Collider 2D. Ensure Is Trigger is checked.

5] Set the Tag of this object to Player.

2. The Body Segment (Prefab)
Create another Sprite (square) to be the body.

1] Add a Box Collider 2D. check Is Trigger.

2] Crucial: Set the Tag of this object to Obstacle.

3] Drag this object from the Hierarchy into your Project folder to create a Prefab.

4] Delete the original from the scene.

Click your Player (Head) and drag the Body Prefab into the Segment Prefab slot in the script inspector.

3. The Food
1] Create a Sprite for the food.

2] Add a Box Collider 2D. Check Is Trigger.

3] Create a new Tag called Food and assign it to this object.

4. The Walls
1] Create 4 cubes/sprites around the screen borders.

2] Give them Box Colliders (Is Trigger = True).

3] Tag them as Obstacle.

4] Controlling Speed
Because this uses FixedUpdate, the snake moves every physics frame (usually 50 times a second), which is too fast for a retro game. To slow it down:

Go to Edit > Project Settings > Time.

Change Fixed Timestep to 0.06 (Fast) or 0.1 (Normal speed).
