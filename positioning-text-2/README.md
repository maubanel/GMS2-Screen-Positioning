<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

### Screen Positioning II

<sub>[previous](../positioning-text-1/README.md#user-content-screen-positioning-i) • [home](../README.md#user-content-gms2-screen-positioning) • [next](../)</sub>

<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

Lets take a closer look at how we position text, objects and other items on screen.

<br>

---

##### `Step 1.`\|`MTP`|:small_blue_diamond:

Repeat this one last time for a sprite called `spr_circle`.  Press **Edit Sprite** and select the *green* color and the bottom right of the **Draw Circle** tool and draw a nice green circle.  Make sure it fills the entire 64 b6 64 frame and is symmetrial in all four corners.

![Create a green circle sprite](images/CreateCircleSprite.gif)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 2.`\|`FHIU`|:small_blue_diamond: :small_blue_diamond: 

We can't place a sprite in the room we have to bind it to an game object. *Right click* on **Object** and select **Create | Object**.  Call this object `obj_triangle`.  Press the button that says <kbd>No Sprite</kbd> and pick the `spr_triangle` **sprite** from the drop down menu.

![Create obj_triangle game object and assign spr_triangle](images/ObjTriangle.gif)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 3.`\|`MTP`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now lets create an object for the square. *Right click* on **Object** and select **Create | Object**.  *Call* this object `obj_square`.  Press the button that says <kbd>No Sprite</kbd> and pick the `spr_square` sprite from the drop down menu.

![Create obj_square game object](images/ObjSquare.gif)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 4.`\|`MTP`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now lets create an object for the circle. *Right click* on *Object* and select **Create | Object**.  Call this object `obj_circle`.  *Press* the button that says <kbd>No Sprite</kbd> and pick the `spr_circle` sprite from the drop down menu.

![Create obj_circle game object](images/ObjCircle.gif)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 5.`\|`MTP`| :small_orange_diamond:

Please note a consistency here.  We are naming all objects with prefix obj_ and all sprites spr_.  This is because we can't have two files with the same name.  We might have various different types of assets with the name circle (for example). This allows us to share a name but not have a problem with collision on two game items with the exact same name.  It also makes it easier to figure out which sprite goes with which objects.  In a small object like this it is simple, but if we had 200 sprites and objects this would be harder to tell without following a consistent naming convention.

*Double left click* **rm_position_objects]** and drag the triangle, circle and square into the room around where you think line 25 lies by eye.

![Drag three newly created game objects into room and guess location under previous text](images/dragThreeShapesInRoom.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 6.`\|`MTP`| :small_orange_diamond: :small_blue_diamond:

Now *press* the <kbd>Play</kbd> button in the top menu bar to launch the game. We should see the three shapes and through trial and error want them to be on the center of the line.

![Run the game and position three objects until they are on the line](images/ThreeShapesAlongLine.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 7.`\|`MTP`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

*Double left click* **obj_triangle** and we need to add a variable to this object.  *Press* the **Variable Definition** button on the game object. 

![Press variable definition button on obj_triangle](images/AddVariableToObjTriangle.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 8.`\|`MTP`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Press the <kbd>Add</kbd> button and call the variable `line_height` and set the **Default** value to `22`.  Make sure the **Type** is a `Integer`.

![add line_height variable set to 22 to obj_triangle](images/AddLineHeightTriangle.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 9.`\|`MTP`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 10.`\|`MTP`| :large_blue_diamond:

![alt_text](images/.png)

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

<img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - ADD NEXT TMTPE">

<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

|[previous](../positioning-text-1/README.md#user-content-screen-positioning-i)| [home](../README.md#user-content-gms2-screen-positioning) | [next](../)|
|---|---|---|

