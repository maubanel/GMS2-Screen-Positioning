<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

### Screen Positioning III

<sub>[previous](../positioning-text-2/README.md#user-content-screen-positioning-ii) • [home](../README.md#user-content-gms2-screen-positioning) • [next](../)</sub>

<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

Lets take a closer look at how we position text, objects and other items on screen.

<br>

---

##### `Step 1.`\|`MTP`|:small_blue_diamond:

Press the <kbd>Add Event</kbd> button and select a **Create** event.

![Add Create event to obj_square](images/AddCreateEventToSquare.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 2.`\|`FHIU`|:small_blue_diamond: :small_blue_diamond: 

In this case we want the middle of the room and we can divide the `room_width` variable by `2` (or multiply by `0.5`). The **y** value will be the same as `obj_square`.

![Center square on x axis in script](images/CreateScriptSquareInitial.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 3.`\|`MTP`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now *press* the <kbd>Play</kbd> button in the top menu bar to launch the game. We notice that it has the same problem that it is positioned based on it's top left corner.

![Run game and square is not positioned correctly](images/squareTooLowGame.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 4.`\|`MTP`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now there are other reason's besides positioning the sprite to adjust the origin.  Another consideration is when we want to rotate the sprite.  

We will be using a different event type to rotate the object.  Since this is not just happening on one frame we need to rotate it every frame.  This is the perfect time to use our second event type a Step event.  Press the <kbd>Add Event</kbd> button and select **Step | Steps** from the menu.

![Add step event to square object](images/AddStepToSquareObject.png)


<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 5.`\|`MTP`| :small_orange_diamond:

To rotate the player there is a variable that is used to determine the angle the player is facing at.  The variable is called **[image_angle](https://manual.yoyogames.com/GameMaker_Language/GML_Reference/Asset_Management/Sprites/Sprite_Instance_Variables/image_angle.htm)**.

`image_angle` is set by changing its angle in degrees.	To rotate counter-clockwise we add degrees *positively* then we rotate clockwise by *subtracting* degrees.  You can see below that a round trip is 360 degrees.

![Illustration of 360 degrees representing rotation in gamemaker](images/RotationsUsingImageAngle.png)


<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 6.`\|`MTP`| :small_orange_diamond: :small_blue_diamond:

We will start by rotating counter-clockwise.  We will add 5 degrees every frame.  The level defaults to 30 frames a second so it will be rotating 5 * 30 = 150 degrees per second. To alter the `image_angle` variable we will add 5 degrees to itself.  So it starts at 0, goes to 5 in the second frame, 10 in the third frame, 15 in the fourth frame etc...

![Add 5 degrees per frame to image_angle in step event](images/RotateSquareStep.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 7.`\|`MTP`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Now *press* the <kbd>Play</kbd> button in the top menu bar to launch the game. Notice that the axis the sprite rotates around is its origin.  This is at the top left corner.  

![Square sprite in game rotating around it top left corner where the origin is located](images/RotatingCube1.gif)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 8.`\|`MTP`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now lets prove that changing the origin will alter the point of rotation.  If this is the case the triangle should rotate on its center.  Lets *add* a **Step | Step** event to `obj_triangle` by pressing the **Add Event** button.

![Add setp event to obj_triangle](images/AddStepToTriangle.gif)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 9.`\|`MTP`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Lets rotate the triangle clockwise so we will subtract by 5 each frame. So it starts at 0, goes to -5 in the second frame, -10 in the third frame, -15 in the fourth frame etc... Add the following script to obj_triangle.

![Subtract 5 degrees per frame for image_angle in obj_triangle](images/TriangleStepRotate.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 10.`\|`MTP`| :large_blue_diamond:

Now *press* the <kbd>Play</kbd> button in the top menu bar to launch the game. Notice that the triangle rotates on the axis whose origin is centered horizontally and vertically wihin the sprite:

![Triangle rotates clockwise around its middle center origin](images/RotatingTriangle1.gif)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 11.`\|`MTP`| :large_blue_diamond: :small_blue_diamond: 

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>


##### `Step 12.`\|`MTP`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: 

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 13.`\|`MTP`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 14.`\|`MTP`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 15.`\|`MTP`| :large_blue_diamond: :small_orange_diamond: 

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 16.`\|`MTP`| :large_blue_diamond: :small_orange_diamond:   :small_blue_diamond: 

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 17.`\|`MTP`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 18.`\|`MTP`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 19.`\|`MTP`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 20.`\|`MTP`| :large_blue_diamond: :large_blue_diamond:

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 21.`\|`MTP`| :large_blue_diamond: :large_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

___


<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

<img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Screen Positioning III">

<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

|[previous](../positioning-text-2/README.md#user-content-screen-positioning-ii)| [home](../README.md#user-content-gms2-screen-positioning) | [next](../)|
|---|---|---|

